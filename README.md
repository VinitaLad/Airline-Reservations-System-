# Airline-Reservations-System-
-------------------------------------------------------
Execute these queries one by one in your MySQL Console
-------------------------------------------------------


1 - Create a database with name airlinemanagementsystem;

create database airlinemanagementsystem;

2 - Use the database you have just created

use airlinemanagementsystem;

3 - Create first table login inside the airlinemanagementsystem database;

create table login(username varchar(20), password varchar(20));

4 - Insert value in the login table for the admin to login

insert into login values('admin', 'admin');

5 - Create next table passenger to store user values;

create table passenger (name varchar(20), nationality varchar(20), phone varchar(15), address varchar(50), aadhar varchar(20), gender varchar(20));

6 - Create table to store flight information

create table flight(f_code varchar(20), f_name varchar(20), source varchar(40), destination varchar(40));

7 - Insert some flight information in the flight table

insert into flight values("1001", "AI-1212", "Delhi", "Mumbai");
insert into flight values("1002", "AI-1453", "Delhi", "Goa");
insert into flight values("1003", "AI-1112", "Mumbai", "Chennai");
insert into flight values("1004", "AI-3222", "Delhi", "Amritsar");
insert into flight values("1005", "AI-1212", "Delhi", "Ayodhya");


8 - Create reservation table to store user ticket booking information

create table reservation(PNR varchar(15), TICKET varchar(20), aadhar varchar(20), name varchar(20), nationality varchar(30), flightname varchar(15), flightcode varchar(20), src varchar(30), des varchar(30), ddate varchar(30));

9 - Create table cancel to store cancel tickets information

create table cancel(pnr varchar(20), name varchar(40), cancelno varchar(20), fcode varchar(20), ddate varchar(30));
