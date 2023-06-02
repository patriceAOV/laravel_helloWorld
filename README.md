# laravel_helloWorld
### setup laravel CRUD
1. Create a new MYSQL database 
2. In env file add the newly create database to the DB_DATABASE
3. Run in your terminal: php artisan migrate:refresh
4. Run in your terminal: php artisan serve

CREATE - POST
http://127.0.0.1:8000/api/students
```
{
    "name":"pat",
    "course": "IT",
    "phone": "0923432323",
    "email": "pat@gmail.com"
}
```

READ - GET
http://127.0.0.1:8000/api/students/{id}

UPDATE - PUT
http://127.0.0.1:8000/api/students/{id}/edit
```
{
        "name": "pat update",
        "course": "IT update",
        "email": "patupdate@gmail.com",
        "phone": "0923432321"
}
```

DELETE - DELETE
http://127.0.0.1:8000/api/students/{id}/delete
