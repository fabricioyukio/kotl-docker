# Infrastructure

<p align="center"><img src="img/docker_logo.svg" width="300" alt="This project user Dockerx" /></p>

## About

This repository is a part of a _show off_ project named "**King of the Lunch**"
("Rei do Lanche" em Português).

Every day there will be an election for applicants for the title "King of the Lunch". Such an election is open for voting between 10:00 am and 12:00 pm. Then at 12:01 pm the votes are counted, and a new King is elected (although one can be elected King more than once).

A given applicant must apply for the elections by registering his **name** and **e-mail** (only one applicant per e-mail is permitted).

## Project Structure

```
+-KotL Project
| +-Infrastructure Repo
|     img
|     |-{image files to illustrate README.md}
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
|
| +-Api Repo
| +-Web App Repo
| +-Android Mobile App Repo*
| +-iOS Mobile App Repo*
```

**✱** Those are stretch goals if I do have time and patience to do so

To develop the project, you mut creat a folder for it and then subfolders with the other repositories.

### Future features

* Configure application if it should open voting in now work days.
* Ask for some id (email, Facebook id,...) to prevent the same user to vote more than once.


## License

This project is open-sourced software licensed under the [MIT license](https://opensource.org/licenses/MIT).

## Made with

<p align="center"><img src="img/vscode_icon.svg?raw=true"/></p>

<p align="center">
<a href="https://packagist.org/packages/laravel/framework"><img src="https://poser.pugx.org/laravel/framework/license.svg" alt="License"></a>
</p>

## Learning Docker

You may lear a lot by taking a peek at **[docker documentation](https://docs.docker.com/)** and video tutorials on youtube, making it a breeze to get started with it.
