<h1 align="center"> Django-server on python </h1>

- ### Install <a href="https://learn.microsoft.com/en-us/windows/wsl/install"> wsl 2 </a> on windows 
- ### Install <a href="https://www.docker.com/"> docker </a>

<h1 align="center"> Create .env file </h1>

- ### Copy and rename file **_.env.dist_** to **_.env_** in current directory

<h1 align="center"> Use this commands to install django-server on docker </h1> 

### Use this command if you are working in linux. It will install all dependencies to mysqlclient.
``` bash
sudo apt-get install python3-dev default-libmysqlclient-dev build-essential
```

## Don't forget about migrations
**On Linux**
``` bash
python3 manage.py makemigrations
```
``` bash
python3 manage.py migrate
``` 
**On Windows**

``` bash
py manage.py makemigrations
```

``` bash
py manage.py migrate
```

## Then use this command to up your local server
```docker-compose up -d --build```