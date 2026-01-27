
# 📘 Education System (JPA Mapping)

A Java backend application that demonstrates effective **Java Persistence API (JPA)** usage with relational mappings for an educational domain. The project highlights how entities (e.g., students, courses, teachers) are mapped to database tables using JPA annotations, enabling clean data persistence and retrieval. ([GitHub][1])

---

## 🧩 Overview

This project implements an **education system backend** that explores:

* Object-Relational Mapping (ORM) using JPA
* Entity relationships (such as one-to-one, one-to-many, etc.)
* Persistent storage of Java objects in a relational database
* Basic CRUD operations for key entities

The goal is to show how JPA can model complex relationships between domain objects and ensure efficient database persistence. ([GitHub][1])

---

## 🚀 Key Features

* ✔ Mapping of entities to database tables using JPA annotations
* ✔ Demonstration of JPA relationships between domain models
* ✔ CRUD operations for main entities
* ✔ Persistent storage configuration with JPA provider (e.g., Hibernate)

---

## 🛠 Technologies Used

* **Java**
* **Java Persistence API (JPA)**
* **Hibernate** (ORM implementation)
* **Maven**
* **MySQL** 
* **IDE**: IntelliJ 

---

## 📂 Project Structure

```
education_system-jpa-mapping
├── src
│   ├── main
│   │   ├── java
│   │   │   ├── model         # JPA entities
│   │   │   ├── repository    # JPA repositories / DAOs
│   │   │   └── service       # Business logic services
│   │   └── resources
│   │       └── persistence.xml / application.properties 
├── .gitignore
├── pom.xml                   # Maven configuration
└── README.md
```

---

## ⚙️ Setup & Installation

### 1. Clone Repository

```bash
git clone https://github.com/Abdelrhaman0/education_system-jpa-mapping-.git
```

### 2. Open in IDE

Import the project in **IntelliJ IDEA**, **Eclipse**, or **NetBeans** as a **Maven project**.

### 3. Configure Database

Update the database connection settings in `persistence.xml` or `application.properties`:

```
spring.datasource.url=jdbc:mysql://localhost:3306/your_db
spring.datasource.username=your_username
spring.datasource.password=your_password
spring.jpa.hibernate.ddl-auto=update
```

### 4. Build & Run

If a main class exists:

```bash
mvn clean install
mvn spring-boot:run
```

If not using Spring Boot, run via your IDE or the JPA utility class that starts the persistence context.

---

## 📌 Typical JPA Mapping Concepts Included

* **Entity Annotation (@Entity)** – Marks a Java class as a persistent entity. ([GeeksforGeeks][2])
* **Relationships** such as:

  * `@OneToOne` – Single object relationship. ([GeeksforGeeks][3])
  * `@OneToMany` / `@ManyToOne` – One entity to many related entities. ([GeeksforGeeks][4])
* **Primary Key Mapping** with `@Id` and generated values. ([GeeksforGeeks][2])

---

## 🧪 Usage

Use an API tool (**Postman**) or database client to:

* Insert new records (students, courses, etc.)
* Retrieve stored entities
* Update existing entities
* Delete records from the database


