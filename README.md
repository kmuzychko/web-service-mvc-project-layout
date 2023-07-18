
# Web Service MVC project layout

This repository presents a suggested project structure for developing web applications using frameworks with flexible structure e.g. FastaPI, Flask in Python or Express, and Fastify in Javascript/Typescript, it also can be used with Chi in Go, but with some modifications due to Golang Project Layout recommendations. It offers a well-organized folder structure that is particularly recommended for medium to big size projects, where handling and ordering the application logic becomes crucial. By adopting this structure, developers can benefit from a modular and scalable architecture that promotes code reusability, maintainability, and collaboration among team members.

The proposed project structure follows the Model-View-Controller (MVC) design pattern, which promotes a clear separation of concerns.  This separation lets developers easily navigate and modify specific application components, facilitating teamwork and reducing code conflicts.

Moreover, this project structure proposal includes directories like "dao" or "repository" for storing persistent layer logic. "ci" to store common utility functions which can be useful for build, deploy, or test purposes, "tests" to house unit, integration or functional tests for the application, and "config" to hold configuration files. These directories help streamline development, testing, and configuration processes, making maintaining and extending the project in the long run easier.

In summary, this project structure proposal provides a solid foundation for organizing the logic of medium to big size web applications. However, it can also be beneficial for smaller projects that have the potential to grow rapidly. By adopting this structure, developers can ensure scalability, maintainability, and codebase organization, enabling them to build robust and efficient applications.

---

Please view `README.md` in each directory for more info.

## Project root directories

`/ci`

CI related files like build, deployment and test related scripts

`/project_package`

Main project package. Contains project essential packages

## Project package directories

`/api`

All API documentation related files

`/assets`

Project related assets e.g. templates, images, etc.

`/clients`

Project specific API clients for third party APIs.

`/config`

Config files and config related logic

`/controller`

MVC Controllers package
 
`/dao` (optional)

> For projects which adopts this pattern

 DAO packages. 

`/di` (optional)

> For projects which adopts this pattern

Dependency injection configurations. 

`/middleware`

API middlewares

`/model`

MVC Model package.

`/repository` (optional)

> For projects which adopts this pattern

Repository pattern contracts and sources implementations.

`/router`

API routers package.

`/tests`

Packages with different types of tests