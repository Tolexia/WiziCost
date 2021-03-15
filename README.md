Welcome to WiziCost !

It is a 52hours-hackathon project which consists in an interactive formular to simulate a price (false one for development) of a resource that could propose a farmer to another one, in a spirit of mutual aid.

If you want to download and run it, make sure you have PHP, mySQL or postgreSQL, composer and yarn installed of your computer, and follow these few steps :
(if you don't have symfony installed on your computer, replace "symfony console" by "php bin/console" for commands in the next lines)

* git clone the project
* run composer install
* run yarn install
* copy .env file that is in the root folder of the project and name it .env.local
* One this file, there is an uncommented line with a sql system, following your own sql system comment the bad one and uncomment the good one. After that, replace the default connexion informations by your own : username, password, host and database name.
* return to your terminal and run symfony console doctrine:database:create
* run symfony console doctrine:migrations:migrate
* run symfony console doctrine:fixtures:load
* run yarn encore dev
* run "symfony server:start" or "php -S localhost:8000" if you don't have symfony installed on your computer

 ** Enjoy !**
