
Créer le projet:
- lien : https://symfony.com/doc/current/setup.html
composer create-project symfony/website-skeleton nomProjet


Security
lien : https://symfony.com/doc/current/security.html
    using Symfony Flex
- composer require symfony/security-bundle

    Create your User Class
- php bin/console make:user

    Installer ORM-Fixture
-composer require orm-fixtures --dev 

    Ajouter un utilisateur
- php bin/console make:fixtures

    Créer la methode d'ajout de l'utilisateur
- utliser : src/DataFixtures/UserFixtures.php

    Ajouter l'utilisateur dans la DB
 - php bin/console doctrine:fixtures:load


    Configurer securité d'accès
    config/packages/security.yaml

    Generating the Login Form
- php bin/console make:auth


 	// Créer une entity
	php bin/console make:entity User

	php bin/console make:migration

	php bin/console doctrine:migrations:migrate



