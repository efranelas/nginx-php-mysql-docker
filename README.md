# nginx-php-mysql-docker

Run a full dynamic PHP application inside containers linked together with easy setup.

Create a `.env` file with the command `cp .env{.example,}` and modify if you will.

Next, you are ready to run the containers with `docker-compose up -d`.

The `nginx/` folder holds files and configuration files related to the nginx service container. The same concept applies to the `php/` folder.
The `mysql/` folder will be created and in there is where the mysql data are persisted. In other words, this folder is linked to the`/var/lib/mysql/` folder inside the container, so it is not meant to be deleted.
Finally, the `src/` folder is where the PHP application source lies, and the `public` folder inside it is publicly available for the web.

