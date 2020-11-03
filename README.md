1. Activate MySQL server

2. create 'DB_flask' database & 'users' table
    create database DB_flask;
    use DB_flask;
    create table users (
        id int auto_increment,
        name varchar(100) not null,
        age tinyint,
        primary key (id)
        );

3. Run the server (app.py)
    $ python app.py

4. Try to request:
    Get all data =>     GET /data
    Get data by id =>   GET /data/{:id}
    Post a data =>      POST /data      => body req: {name:"KHOULOUD", age:"24"}
    Update a data =>    PUT /data/{:id} => body req: {name:"KHOULOUD", age:"25"}
    Delete a data =>    DELETE /data/{:id}
