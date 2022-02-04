<p align="center">
    Laravel Boilerplate with
    <a href="https://www.laravel.com">
        <img src="https://raw.githubusercontent.com/MagicalStrangeQuark/MagicalStrangeQuark/master/assets/laravel.svg" width="10%">
    </a>
    <a href="https://www.mysql.com">
        <img src="https://raw.githubusercontent.com/MagicalStrangeQuark/MagicalStrangeQuark/master/assets/mysql.svg" width="10%">
    </a>
    <a href="https://www.nginx.com">
        <img src="https://raw.githubusercontent.com/MagicalStrangeQuark/MagicalStrangeQuark/master/assets/nginx.svg" width="10%">
    </a> with 👉<a href="https://www.docker.com">Docker</a>👈
</p>

<p align="center">
    <a href="#">
        <img alt="License" src="https://img.shields.io/github/license/Whopag/DockerLaravelMySQL">
    </a>
    <a href="#">
        <img alt="Languages" src="https://img.shields.io/github/languages/count/Whopag/DockerLaravelMySQL">
    </a>
    <a href="#">
        <img alt="Last Commit" src="https://img.shields.io/github/last-commit/Whopag/DockerLaravelMySQL">
    </a>
    <a href="#">
        <img alt="Followers" src="https://img.shields.io/github/followers/Whopag?style=social">
    </a>
</p>

<h5 align="center">Setup a Laravel application</h5>

<h6 align="center">Remove the existing one</h6>

```bash
    sudo rm -Rf html
```

<h6 align="center">Create an empty Laravel application</h6>

```bash
    composer create-project laravel/laravel html
```

<p align="center">After create a new project or using yours, configure the environment variables</p>

```bash
    DB_CONNECTION=mysql
    DB_HOST=laravelmysql_mysql_1
    DB_PORT=3306
    DB_DATABASE=laravel
    DB_USERNAME=root
    DB_PASSWORD=secret
```

<p align="center">Now you have to build the image from <em>Docker</em> image</p>

```bash
    docker-compose up -d --build
```

<p align="center">Run Laravel migrations</p>

```bash
    docker-compose run --rm artisan migrate:fresh --seed
```

<p align="center">Create an Laravel application key</p>

```bash
    docker-compose run --rm artisan key:generate
```

<h4 align="center">Topics</h4>

<h6 align="center">🚀 Docker</h6>

<p>If necessary, you can remove all images using <strong>docker system prune -a --volumes</strong></p>

<h4 align="center">Questions</h4>

<p>Any questions or suggestions regarding the project, please contact me on 📧 <strong>wesleyfloresterres@gmail.com</strong></p>