### Copy and Paste the following MYSQL commands to make a dummy database for this Project :


create database if not exists onlinestore;

use onlinestore;

create table if not exists books(barcode varchar(100) primary key, name varchar(100), author varchar(100), price int, quantity int);

create table if not exists users(username varchar(100) primary key,password varchar(100), firstname varchar(100),lastname varchar(100),address text, phone varchar(100),mailid varchar(100),usertype int);

insert into  books values('9780134190500', 'Data Structures Through C', 'G.S. Baluja', 525, 20);

insert into  books values('9780134190563','The Go Programming Language','Alan A. A. Donovan and Brian W. Kernighan',400,8);

insert into  books values('9780133053036','C++ Primer','Stanley Lippman and Josée Lajoie and Barbara Moo',976,13);


commit;
