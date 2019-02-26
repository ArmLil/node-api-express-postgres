.gitignore is taken from https://github.com/github/gitignore/blob/master/Node.gitignore

GET — / | displayHome()
GET — /users | getUsers()
GET — /users/:id | getUserById()
POST — users | createUser()
PUT — /users/:id | updateUser()
DELETE — /users/:id | deleteUser()


usfull docs

https://www.digitalocean.com/community/tutorials/how-to-install-and-use-postgresql-on-ubuntu-16-04

https://blog.logrocket.com/setting-up-a-restful-api-with-node-js-and-postgresql-d96d6fc892d8

CREATE ROLE me WITH LOGIN PASSWORD 'password';

sudo -i -u me   (switch to me account)
psql -d postgres -U me


   \q | Exit psql connection
   \c | Connect to a new database
   \dt | List all tables
   \du | List all roles
   \list | List databases

    CREATE DATABASE api;

CREATE TABLE users (
 ID SERIAL PRIMARY KEY,
 name VARCHAR(30),
 email VARCHAR(30)
);


INSERT INTO users (name, email)
VALUES ('Jerry', 'jerry@example.com'), ('George', 'george@example.com');

SELECT * FROM users;
