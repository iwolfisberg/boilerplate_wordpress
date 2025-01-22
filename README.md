# Boilerplate WordPress

Bienvenue dans le projet **Boilerplate WordPress** ! Ce repository a été conçu pour vous permettre de faire vos premiers pas avec WordPress.

---

## Objectif

Ce boilerplate offre une première installation WordPress configurée pour utiliser le dossier `templating`, qui sert de base au développement de thèmes WordPress modernes. Le but est de suivre un tutoriel détaillé (voir lien ci-dessous) pour explorer :

- La mise en place et le fonctionnement d'un site WordPress.
- L'intégration d'un template basé sur **starterkit** et **TailwindCSS**.
- L'utilisation de Twig.

---

## Prérequis

Avant de commencer, assurez-vous d'avoir installé :

1. **PHP**
2. Un serveur local comme **MAMP**, ou **XAMPP**, ou tout autre outil de votre choix.

👉 [Lien vers le tutoriel Notion](https://www.notion.so/eikon-imd/1-Installation-de-l-environnement-de-travail-183709599a8180c291f0ef01674dc65f?pvs=4)

---

## Installation

### 1. Cloner le repository

```bash
git clone https://github.com/iwolfisberg/boilerplate_wordpress.git
cd boilerplate_wordpress
```

### 2. Installer les dépendances du templating

```bash
cd templating
npm install
npm run dev
```

### 3. Initialisation de WordPress

3.1. Accéder à PHPMyAdmin, une interface pour gérer vos bases de données:

- [http://localhost/phpymyadmin](http://localhost/phpymyadmin)

3.2. Créer une nouvelle base de données appelées `wp_hello_world`.

3.3. Configurer votre site en vous rendant sur `http://localhost/<nom_du_dossier>/wordpress`. L'interface vous demandera de remplir diverses informations:

- Nom de la base de données: `wp_hello_world`
- Identifiant: `root`
- Mot de passe:
- Adresse de la base de données: `localhost`
- Préfixe des tabeles: `wp_`

Si lorsque vous soumettez le formulaire, un message d'erreur apparait indiquant une impossibilité de créer le fichier `wp-config.php`, suivez [les instructions de cette page](https://www.notion.so/eikon-imd/2-Installer-WordPress-182709599a8180fba117d9dff980d733?pvs=4#182709599a8180bea6afe34685516b0e).

Une fois fait, rechargez la page et remplissez à nouveau les informations.

3.4. Ensuite, WordPress vous demandera quelques informations supplémentaires concernant votre site.

- Titre: `Hello World` ou ce que vous voulez
- Identifiant: `admin`
- Mot de passe: `admin` (-> et confirmation du mot de passe faible)
- E-mail: le votre

3.5. Suite à cela, vous devriez pouvoir vous identifier sur votre site à `http://localhost/<nom_du_dossier>/wordpress/wp-admin` avec les identifiants `admin / admin`.

## Suivre le tutoriel

Un tutoriel complet est disponible pour vous guider à travers chaque étape :

👉 [Lien vers la vidéo](https://www.youtube.com/watch?v=GSJ-Gj0AsFE&ab_channel=CyrilVernier).

## Ressources supplémentaires

- [Documentation WordPress](https://wordpress.org/documentation/)
- [Documentation TailwindCSS](https://tailwindcss.com/docs/installation)
