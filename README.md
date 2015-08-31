library_system
This application allows a user to add many books and many patrons.

By Kendra Ash

Description

This application is for learning many to many relationships and how ruby code interacts with a database. It uses postgres to provide a server for an SQL enviornment. 

Setup

clone from git hub
from terminal/command line cd to folder
run bundle
run postgres
run psql
run CREATE DATABASE library;
connect to database by \c library
CREATE TABLE books(title VARCHAR, author VARCHAR, book_id SERIAL PRIMARY KEY, patron_id INT, check_our_date TIMESTAMP, due_date TIMESTAMP);
CREATE TABLE patrons(patron_name VARCHAR, patron_id SERIAL PRIMARY KEY);
CREATE DATABASE library_test WITH TEMPLATE library
open browser and visit localhost:4567
Technologies Used

Ruby
With Gems: sinatra-contrib, sinatra/reloader, sinatra-activerecord, rake, pg, sinatra, rspec, capybara, pry

Legal

Copyright (c) 2015 Kendra Ash

Created for learning purposes.

This software is licensed under the MIT license.

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
