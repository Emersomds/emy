## Projeto web python e mysql

## Requisitos

* Python 3 ou superior - Conferir a versão: python --version
* Django 5 ou superior - Conferir a versão: django-admin --version

## Sequencia para criar o projeto

Instalar o Django.
```
pip install Django
```

Criar o projeto com Django.
```
django-admin startproject admin .
```

Rodar o projeto.
```
python manage.py runserver
```

criar o banco de dados
```
create database emy character set utf8mb4 collate utf8mb4_unicode_ci;
```

Alterar no arquivo "settings.py" as credenciais do Banco de Dados<br>
````
````
'ENGINE': 'django.db.backends.mysql',
'NAME': 'nomeBanco',
'USER': 'usuário',
'PASSWORD': 'senhaBanco',
'HOST': 'localhost',
'PORT': 3306,
````


Instalar o conector Mysql.
```
pip install mysqlclient
```

Executa as migration.
```
python manage.py migrate
```

Criar um super usuário.
````
python manage.py createsuperuser
````
````
Usuário (leave blank to use 'emymatos'): admin
Endereço de email: matoss393@gmail.com
Password: 123456A#
Password (again): 123456A#
````

Acessar o sistema administrativo padrão.
````
http://127.0.0.1:8000/admin
````
