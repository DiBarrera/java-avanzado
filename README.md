# Advanced Java

## Advanced Java was learned at a high leve, using Object Oriented Programming applied to classes and interfaces. Applying modular programming and giving persistence across databases with JDBC

<!-- TABLE OF CONTENTS -->
<details open="open">
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#Overviwe">Overviwe</a>
    </li>
    <li>
      <a href="#getting-started">Getting Started</a>
    </li>
    <li><a href="#Topics-reviewed">Topics reviewed</a></li>
    <li><a href="#Basics">Basics</a></li>
    <li><a href="#Acquired-skills">Acquired skills</a></li>
  </ol>
</details>



<!-- Overviwe -->
## Overviwe

In this repository you will find a brief summary of what was learned in the [platzi](https://platzi.com/cursos/java-avanz) course of Java Advanced SE.

---------

Advanced Java implies the assimilation of more technical concepts and their application, an approach to lambda functions, creation of DAO interfaces, inheritance of interfaces, try and catch, among others, entering projects that can be connected to a database to offer a better user experience.

---------

This repository is divided into the following parts.
* The steps to clone the repository and be able to view it.
* The main topics seen in the course
* Some of the basics concepts taught.
* Skills acquired at the end of the course.



<!-- GETTING STARTED -->
## Getting Started

## Setup

- Fork this repo
- Clone this repo

```shell
$ mkdir advanced-java
$ cd advanced-java
$ git clone https://github.com/DiBarrera/java-avanzado.git
```

You will find the following files:

- **A main directory**, which is the name of the project developed during the course.
- **The directorys** that make the project work.
- **The src directory** containing the main files of the project development.

### For this repository, Eclipse was used as IDE.

### As a server for the development of this project, phpmyadmin was used.

### To have a phpmyadmin server, XAMPP was used.

- In the following link you can install XAMPP. https://www.apachefriends.org/es/index.html
- Follow the installation steps.
- Once installed, start the services.
- When the services are started, in a web browser we go to the following link: http://localhost/phpmyadmin/

### Creating a user and a database.

- Once inside the phpmyadmin administrator, we click on "user accounts".
- We look for the option: "Add user account".
- Then, in the "Local" option, we select the "Check" option.
- We grant all privileges.
- Click on "Continue".
- You will see that now on the left side will be the database created, select it and click on "Import".
- As a database, a file contained in the following link was used: https://drive.google.com/file/d/1uneLZrRZ0y1ASOUkVzzw7qRQwrS0Ui-d/view?usp=sharing

### Downloading connector

- In the following link, download the connector, which will link the project with the database: https://dev.mysql.com/downloads/connector/j/5.1.html

...



**Tree**

```markdown
.
├── AmazonViewer
│   ├── bin
│   │   └── com
│   │       └── anncode
│   │           ├── amazonviewer
│   │           │   ├── Main.class
│   │           │   └── model
│   │           │       ├── Book.class
│   │           │       ├── Chapter.class
│   │           │       ├── Film.class
│   │           │       ├── IVisualizable.class
│   │           │       ├── Magazine.class
│   │           │       ├── Movie.class
│   │           │       ├── Publication.class
│   │           │       └── Serie.class
│   │           └── util
│   │               └── AmazonUtil.class
│   ├── doc
│   │   ├── allclasses-index.html
│   │   ├── allclasses.html
│   │   ├── allpackages-index.html
│   │   ├── com
│   │   │   └── anncode
│   │   │       ├── amazonviewer
│   │   │       │   ├── Main.html
│   │   │       │   ├── class-use
│   │   │       │   │   └── Main.html
│   │   │       │   ├── model
│   │   │       │   │   ├── Book.html
│   │   │       │   │   ├── Chapter.html
│   │   │       │   │   ├── Film.html
│   │   │       │   │   ├── IVisualizable.html
│   │   │       │   │   ├── Magazine.html
│   │   │       │   │   ├── Movie.html
│   │   │       │   │   ├── Publication.html
│   │   │       │   │   ├── Serie.html
│   │   │       │   │   ├── class-use
│   │   │       │   │   │   ├── Book.html
│   │   │       │   │   │   ├── Chapter.html
│   │   │       │   │   │   ├── Film.html
│   │   │       │   │   │   ├── IVisualizable.html
│   │   │       │   │   │   ├── Magazine.html
│   │   │       │   │   │   ├── Movie.html
│   │   │       │   │   │   ├── Publication.html
│   │   │       │   │   │   └── Serie.html
│   │   │       │   │   ├── package-summary.html
│   │   │       │   │   ├── package-tree.html
│   │   │       │   │   └── package-use.html
│   │   │       │   ├── package-summary.html
│   │   │       │   ├── package-tree.html
│   │   │       │   └── package-use.html
│   │   │       └── util
│   │   │           ├── AmazonUtil.html
│   │   │           ├── class-use
│   │   │           │   └── AmazonUtil.html
│   │   │           ├── package-summary.html
│   │   │           ├── package-tree.html
│   │   │           └── package-use.html
│   │   ├── constant-values.html
│   │   ├── deprecated-list.html
│   │   ├── element-list
│   │   ├── help-doc.html
│   │   ├── index-files
│   │   │   ├── index-1.html
│   │   │   ├── index-10.html
│   │   │   ├── index-11.html
│   │   │   ├── index-2.html
│   │   │   ├── index-3.html
│   │   │   ├── index-4.html
│   │   │   ├── index-5.html
│   │   │   ├── index-6.html
│   │   │   ├── index-7.html
│   │   │   ├── index-8.html
│   │   │   └── index-9.html
│   │   ├── index.html
│   │   ├── jquery
│   │   │   ├── external
│   │   │   │   └── jquery
│   │   │   │       └── jquery.js
│   │   │   ├── images
│   │   │   │   ├── ui-bg_glass_55_fbf9ee_1x400.png
│   │   │   │   ├── ui-bg_glass_65_dadada_1x400.png
│   │   │   │   ├── ui-bg_glass_75_dadada_1x400.png
│   │   │   │   ├── ui-bg_glass_75_e6e6e6_1x400.png
│   │   │   │   ├── ui-bg_glass_95_fef1ec_1x400.png
│   │   │   │   ├── ui-bg_highlight-soft_75_cccccc_1x100.png
│   │   │   │   ├── ui-icons_222222_256x240.png
│   │   │   │   ├── ui-icons_2e83ff_256x240.png
│   │   │   │   ├── ui-icons_454545_256x240.png
│   │   │   │   ├── ui-icons_888888_256x240.png
│   │   │   │   └── ui-icons_cd0a0a_256x240.png
│   │   │   ├── jquery-3.5.1.js
│   │   │   ├── jquery-ui.css
│   │   │   ├── jquery-ui.js
│   │   │   ├── jquery-ui.min.css
│   │   │   ├── jquery-ui.min.js
│   │   │   ├── jquery-ui.structure.css
│   │   │   ├── jquery-ui.structure.min.css
│   │   │   ├── jszip
│   │   │   │   └── dist
│   │   │   │       ├── jszip.js
│   │   │   │       └── jszip.min.js
│   │   │   └── jszip-utils
│   │   │       └── dist
│   │   │           ├── jszip-utils-ie.js
│   │   │           ├── jszip-utils-ie.min.js
│   │   │           ├── jszip-utils.js
│   │   │           └── jszip-utils.min.js
│   │   ├── member-search-index.js
│   │   ├── member-search-index.zip
│   │   ├── overview-summary.html
│   │   ├── overview-tree.html
│   │   ├── package-search-index.js
│   │   ├── package-search-index.zip
│   │   ├── resources
│   │   │   ├── glass.png
│   │   │   └── x.png
│   │   ├── script.js
│   │   ├── search.js
│   │   ├── stylesheet.css
│   │   ├── type-search-index.js
│   │   └── type-search-index.zip
│   ├── libs
│   │   ├── makefile.jar
│   │   └── mysql-connector-java-8.0.25.jar
│   ├── reporte2018-01-26.txt
│   └── src
│       └── com
│           └── anncode
│               ├── amazonviewer
│               │   ├── Main.java
│               │   ├── dao
│               │   │   └── MovieDAO.java
│               │   ├── db
│               │   │   ├── DataBase.java
│               │   │   └── IDBConnection.java
│               │   └── model
│               │       ├── Book.java
│               │       ├── Chapter.java
│               │       ├── Film.java
│               │       ├── IVisualizable.java
│               │       ├── Magazine.java
│               │       ├── Movie.java
│               │       ├── Publication.java
│               │       └── Serie.java
│               └── util
│                   └── AmazonUtil.java
└── README.md
``` 



<!-- Topics reviewed -->
## Topics reviewed

In this repository you will find sql files that were varied exercises to practice searching for data in databases in different ways. The topics are made up of the different ways to do these searches. Topics such as a brief history of databases, the different types of databases, services, and other fundamental topics for a better general understanding about databases were also included.
This course was followed using MySQL Workbench.

### Topics

- Introduction to Advanced Java.
- Polymorphism.
- Inheritance.
- Encapsulation.
- Abstraction.
- Abstract classes.
- Abstract methods.
- Java docs.
- Implementing java docs.
- Advanced classes, nested classes.
- Local classes and methods.
- Enumerations.
- Advanced interfaces.
- Default and private methods.
- DAO (Data Access Object).
- Difference between interfaces and abstract classes.
- HashMap. LinkedHashMap. TreeMap.
- Error handling.
- Exceptions.
- Try-catch-finally / Try-with-resources.
- JDBC (Java Data Base Connectivity).
- Connecting to a database with Connector.
- Functional interfaces.
- Functional programming.
- Lambda function.
- Lambdas as a variable.
- Stream and Filter.
- Predicate and Consumer.



<!-- Basics -->
## Basics

#### Abstract classes
```markdown
public abstract class Figure {
  ...abstract void draw();
}
``` 

#### Commenting code
```markdown
// Single line comment 
 
/* Comment 
* in multiple 
* lines */ 
 
/** 
* Comment for Java Docs
* */ 
``` 

#### Java Docs for functions
```markdown
/**
 * General description of our function.
 * 
 * @param parameter1 Description of parameter 1.
 * @param parameter2 Description of parameter 2.
 * @return Description of the value that we return in the function.
 * */
 ``` 
 
 #### Implementing java docs
```markdown
/**
 * [General description]
 * <p>
 * 
 * [Large description]
 * [author, version, params, returns, throws, see, other tags]
 * [see also]
 * */
 ``` 
 
#### Nested classes
```markdown
class OutterClass {
  ...class NestedClass {
    ...
  }
}
 ``` 
 
#### Static nested class
 ```markdown
class OutterClass {
  ...static class NestedStaticClass {
  }
  class InnerClass {
  
  }
}
 ``` 
 
 #### Differences between interfaces and abstract classes
| Abstrac class      | Interface                         |
| ------------- | ------------------------------ |
| Define subclasses. Reuse methods from your super class.     | Abstract and non-abstract methods. |
| Instances cannot be used, only inheritance.     | The methods can be implemented in many families. |
| Cannot create objects.     | Focuses on the behavior that can bring to a class. |
| Only used to redefine new classes without creating new objects.     | Non-linear implementation. |

#### Static nested class
 ```markdown
Map<Integer, String> map = new HashMap<Integer, String>();
Map<Integer, String> treeMap = new TreeMap<Integer, String>();
Map<Integer, String> linkedHashMap = new LinkedHashMap<Integer, String>();
 ``` 
 
#### Try - catch
 ```markdown
try {
  
} catch (ExceptionType name) {

} catch (ExceptionType name) {

}
 ``` 
 
 #### Lambda
 ```markdown
(parameters) -> (lambda-body)
 ``` 
 
#### Streams
 ```markdown
objects.stream()
 ``` 

#### Filter
 ```markdown
objects.stream().filter()
 ``` 
 
 
 
 <!-- Acquired skills -->
## Acquired skills

- Polymorphism.
- Inheritance.
- Encapsulation.
- Abstraction.
- Java Docs.
- Nested classes.
- Handle exceptions.
- Structure and program databases with JDBC.
- Use lambda functions.
- Apply nested and abstract classes.
- Map, HashMap, TreeMap and LinkedHashMap.
- Try-catch finally / try-catch resources.
- JDBC Api.
- Connecting to a database.
