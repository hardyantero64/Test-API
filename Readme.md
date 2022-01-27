//Api using Symfony and Swagger//
//Instruction also available from https://digitalfortress.tech/tutorial/rest-api-with-symfony-and-api-platform//

$ composer create-project symfony/skeleton api

$ composer require symfony/maker-bundle --dev         // enable entity maker//

$ composer require doctrine/annotations

$ composer require symfony/orm-pack

$ composer require doctrine/doctrine-bundle

$ npm install -g swagger          //api through swagger//

$ npm install -g npm@8.3.2   //version//

in .env file, alter database url to approrpiate settings

DATABASE_URL="mysql://root:password@127.0.0.1:3306/name_of_your_new_database"

//To create: //

$ php bin/console doctrine:database:create

// Database should be created after this command. If drivers not found, check that php.ini files are updated with drivers//

//after database created: 

$ php bin/console make:entity --regenerate App   // generate Entity//


$ php bin/console doctrine:schema:update --dump-sql   //check the raw sql query before executing//
 
 
$ php bin/console doctrine:schema:update --force   //To execute the SQL query//


//output should be: [OK] Database schema updated successfully!//


//Test api Response body on your Api using "Post" function as visible at //Instruction also available from https://digitalfortress.tech/tutorial/rest-api-with-symfony-and-api-platform//



