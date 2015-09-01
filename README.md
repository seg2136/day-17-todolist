# To-Do List

##### Updated To-Do List with many-to-many database relationships, 1 September 2015

#### By Stephany Garcia

## Description

This is a Java app that allows users to create tasks and list them out. It also has the ability to have multiple categories with a tasks method that returns all the tasks in a particular list. Users can also mark tasks as done without deleting them, so that they can view all of their completed tasks later.


## Setup

For Database--
Make sure you have postgreSQL installed. Then open a new terminal and run $psql.
After, type the following command in your terminal:
CREATE DATABASE to_do;
/c to_do;
CREATE TABLE categories (id serial PRIMARY KEY, name varchar);
CREATE TABLE tasks (id serial PRIMARY KEY, description varchar);
CREATE TABLE categories_tasks (id serial PRIMARY KEY, category_id int, task_id int);

For Java app--
Clone this repository.
Using the command line, navigate to the top level of the cloned directory.
Make sure you have gradle installed. Then run the following command in your terminal:
gradle run
Go to localhost:4567.
Make your own to-do list!


## Technologies Used

* Java
* Spark
* Velocity
* Gradle
* JUnit
* FluentLenium
* PostgreSQL


### Legal

Copyright (c) 2015 Stephany Garcia

This software is licensed under the MIT license.

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.
