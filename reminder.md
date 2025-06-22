    # for a traditional web app
    composer create-project symfony/skeleton:"6.4.*" my_project_directory
    cd my_project_directory
    composer require webapp

    # for a microservice, console application or API
    composer create-project symfony/skeleton:"6.4.0" my_project_directory

    composer require symfony/maker-bundle --dev
    composer require symfony/orm-pack

    Configure the .env file for the database

    php bin/console doctrine:database:create
    php bin/console doctrine:database:create --env=test

    php bin/console make:entity

    php bin/console make:migration
    php bin/console doctrine:migrations:migrate
    php bin/console doctrine:migrations:migrate --env=test

    composer require symfony/form
    composer require symfony/mime
    composer require symfony/validator
    composer require twig
    composer require --dev symfony/test-pack
    composer require symfony/asset

    php bin/console make:controller
    php bin/console make:test

    composer require symfony/security-bundle
    php bin/console make:user