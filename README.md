# Infrastructure

<p align="center"><img src="assets/docker_logo.svg" width="300" alt="This project uses Docker" /></p>

## About

This repository is a part of a _show off_ project named "**King of the Lunch**"
("Rei do Lanche" em Português).

Every day there will be an election for applicants for the title "King of the Lunch". Such an election is open for voting between 10:00 am and 12:00 pm. Then at 12:01 pm, the votes are counted, and a new King is elected (although one can be elected King more than once).

A given applicant must apply for the elections by registering his **name** and **e-mail** (only one applicant per e-mail is permitted).

## Project Structure

```
+-KotL Project
| +-kotl-docker(Infrastructure Repo, this project)
|     assetd
|     |-{files referenced in README.md}
|
|     mysql
|     |-{config files for DB}
|
|     nginx
|     |- { config files for NGINX }
|
|     php
|     |- { config files for PHP }
|
| +-kotl-api-php (Api Repo)
| +-kotl-web (Web App Repo)
| +-kotl-mobile-android (Android Mobile App Repo*)
| +-kotl-mobile-ios (iOS Mobile App Repo*)
```

**✱** Those are stretch goals that I'll try to achieve if I do have time and patience to do so

To develop the project, you must create a folder for it and then subfolders with the repositories.

### PHP
Once this project is UP, it is already running PHP on port 80 ([localhost](http://localhost)), so just edit the PHP files you want and it's ready to go! Meaning: there is no need to run something like 

```bash
php artisan serve --port=80
```

### MySQL

Also, there is a MySQL Instance on port 3306, already running.

### Redis

Redis is operating in its respective usual port (6379).

### Frontends

The main frontend project is **Webapp**.

For further information, please take a moment to check their respective repositories.

### Future features

* Configure application if it should open voting in now workdays.
* Ask for some id (email, Facebook id,...) to prevent the same user to vote more than once.

## Running the project

As aforementioned, this project uses Docker.

### Requirements

A computer - Any machine capable of running **docker**, **php** and **mysql** will do.

[Docker](https://docs.docker.com/) - make sure it is installed and running.

[Sendgrid](https://sendgrid.com/docs/api-reference) API Key - set it on "_kotl-api/**.env**_" file.

#### Set .env

On **this project** folder, copy .env.example file to .env

```bash
cp .env.example .env
```

Set parameters **WEB_APP_DIR** and **WEB_API_DIR** to correspond to *kotl-web-app* and *kotl-api-php* directories paths, relative to *docker-compose* file.

##### Raise the instances for API, Redis and MySQL

```bash

```

## License

This project is open-sourced software licensed under the [MIT license](https://opensource.org/licenses/MIT).

## Made with

<p align="center"><a href="https://code.visualstudio.com/" target="_blank"><img src="assets/vscode_icon.svg"/></a></p>

## Learning Docker

You may lear a lot by taking a peek at **[docker documentation](https://docs.docker.com/)** and video tutorials on youtube, making it a breeze to get started with it.
