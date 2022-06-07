# buzzfeed

This is a REST API used for querying and retrieving scoped news and information. There are news/articles/posts that are available to all employees without navigating into any department, and others that are housed/classified within departments.

#### By  Diana Kieru

## Setup/Installation Requirements
* You need to have Java, IntelliJ, gradle, Junit, Jdk and sdk installed.
* Clone the repository
* Build (gradle build)
* Run the App (maven))
* Navigate to localhost:4567 on your browser
* In PSQL:
```
CREATE DATABASE buzzfeed;
 CREATE TABLE news (id serial PRIMARY KEY, post varchar);
 CREATE TABLE department (id serial PRIMARY KEY, name varchar, numberofemployees int, description varchar);
 CREATE TABLE users (id serial PRIMARY KEY, position varchar, name varchar, departmentid int, role varchar);

```
```
end points
On postman localhost:4567
 post (/department/new)
 post("/departments/:departmentId/news/:newsId")
 get("/departments/:id/news")
 get("/news/:id/departments")
  post("/departments/:departmentId/users/new")
  post("/news/new")
  get("/departments")
   get("/departments/:id")
    get("/departments/:id/users")
    get("/news")
    get("/users")
    post("/department/new")


```
## Known Bugs
There are no known bugs. Incase you experience any errors using this website kindly contact me at dianakieru1@gmail.com
## Technologies Used
* Java
* Spark

## Support and contact details
email: dianakieru1@gmail.com


### License
[MIT License](./LICENSE)

Copyright (c) [2022] [Diana Kieru]
