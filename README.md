# Loggin
Proyecto Loggin whit Bootstrap, POO, PDO, Singleton, Dependency Injection, DAO and VO.

## Using Docker
```
docker pull allexiusw/hub-server:latest
docker run -it-d --name hub_server -p 777:80 docker.io/allexiusw/hub-server
docker exec -it hub_server bash
```

## Legacy Installation

### Requirements
* Apache2
* PHP7.0
* MySQL
* PHPMyAdmin (Optional)
* Testing
### Step 0
```
apt install git 
```

### Step 0.5
```
cd /var/www/html/
```

### Step 1
Clone the project
```
https://github.com/allexiusw/Loggin.git
```

### Step 2
Create Database en table for project
```
mysql -u root -p 
>CREATE DATABASE Loggin; [INTRO]
>GRANT ALL PRIVILEGES ON Loggin.* TO "youruser"@localhost IDENTIFIED BY "yourpass"; [INTRO]
>FLUSH PRIVILEGES; [INTRO]
>EXIT [INTRO]
```
### Step 3
Go to PHPMyAdmin and loggin with "youruser" and "yourpass", save the User.sql in your desktop computer and import to database Loggin create in the last step. Or use mysql the next command:
```
mysql -u youruser -p Loggin < Loggin/Users.sql
```

### Step 4
```
nano Loggin/class/Connection.php 
```
change the "root" by "youruser" and "021$" by "yourpass".

### Step 5

Go to Chrome loggin with user "foo" and password "021$$"

Finish tutorial.
