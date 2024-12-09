# 📚 Library Management System for STU

![Library Management System Overview](https://github.com/user-attachments/assets/261cea60-5a6c-463c-897b-d8ceb27cd499)

## 📑 Table of Contents
- [📖 Overview](#📖-overview)
- [✨ Features](#✨-features)
- [🛠️ Technologies](#🛠️-technologies)
- [📊 Database Model](#📊-database-model)
- [🚀 Getting Started](#🚀-getting-started)
  - [🔧 Requirements](#🔧-requirements)
  - [⚙️ Running the Application](#⚙️-running-the-application)
  - [📦 Building Packages](#📦-building-packages)
  - [🗄️ Database Management](#🗄️-database-management)
  - [✉️ Email Sending Testing](#✉️-email-sending-testing)
- [👥 Credits](#👥-credits)

## 📖 Overview

The **Library Management System** is a web application designed to manage a library. It allows users to view the library catalog and perform actions with library materials and users. 📚👥

**Project created as part of an educational seminar:**
- **Course:** IKT - Java Programming

## ✨ Features

### 👤 User Management
**Roles (basis for authorization):**
- **Administrator**
- **Librarian**
- **Reader**

**Available Operations:**
- 🆕 Create a user (add a new user)
- ✏️ Edit and update user data
- 🗑️ Delete a user
- 🔐 Authentication (login/logout)
- 👀 View all users (with search, filtering, sorting, and pagination)
- 📄 View user details for a specific user
- 🧑‍💼 View current user details (My Data)

### 📚 Manage Library Materials/Resources and Catalog

#### 🖋️ Authors
**Available Operations:**

| Operation                         | Image                                                                                              |
|-----------------------------------|----------------------------------------------------------------------------------------------------|
| ➕ Add a new author                | <img src="https://github.com/user-attachments/assets/08a97a4d-5300-40d2-9280-aeb256827765" width="50%" alt="Add Author"> |
| ✏️ Edit and update author         | <img src="https://github.com/user-attachments/assets/bfad4634-d17a-4fa9-a37d-c382e393a464" width="50%" alt="Edit Author"> |
| 🗑️ Delete author                  | <img src="https://github.com/user-attachments/assets/6d9a1fd4-c72d-45bb-bd67-c8ceee88a3ac" width="50%" alt="Delete Author"> |
| 👀 View all authors                | <img src="https://github.com/user-attachments/assets/c4f8dd5f-1592-4392-a6c9-523628dcf08c" width="50%" alt="View Authors"> |

#### 🗂️ Categories
**Available Operations:**

| Operation                           | Image                                                                                              |
|-------------------------------------|----------------------------------------------------------------------------------------------------|
| ➕ Add a new category                | <img src="https://github.com/user-attachments/assets/246accd2-1673-4287-9f16-e80530f5a025" width="50%" alt="Add Category"> |
| ✏️ Edit and update category         | <img src="https://github.com/user-attachments/assets/c19e047e-29ac-4fd7-b474-ab6421277034" width="50%" alt="Edit Category"> |
| 🗑️ Delete category                  | <img src="https://github.com/user-attachments/assets/d241ba90-394b-4713-81d7-648d72547f4c" width="50%" alt="Delete Category"> |
| 👀 View all categories               | <img src="https://github.com/user-attachments/assets/0c7a694c-b0f7-469f-b9ee-7fadc1bf1f7f" width="50%" alt="View Categories"> |

#### 📖 Works
**Available Operations:**

| Operation                             | Image                                                                                              |
|---------------------------------------|----------------------------------------------------------------------------------------------------|
| ➕ Add a new work                      | <img src="https://github.com/user-attachments/assets/a059b3e2-ab33-477c-8ed3-0a80eb4ace5c" width="50%" alt="Add Work"> |
| ✏️ Edit and update work               | <img src="https://github.com/user-attachments/assets/f69d3439-13fe-472c-8d29-d0747d149c5d" width="50%" alt="Edit Work"> |
| 🗑️ Delete work                        | <img src="https://github.com/user-attachments/assets/c0d99208-365c-400f-8a48-6a5810f6c3cb" width="50%" alt="Delete Work"> |
| 👀 View all works                      | <img src="https://github.com/user-attachments/assets/c6efb7a2-2cc3-4b9e-b267-246b637e0c8d" width="50%" alt="View Works"> |
| 📦 View all copies of a specific work | <img src="https://github.com/user-attachments/assets/bbeb797f-e026-4d05-9b57-3e70fd2757c7" width="50%" alt="View Book Copies"> |

#### 📕 Books
**Available Operations:**

| Operation                           | Image                                                                                              |
|-------------------------------------|----------------------------------------------------------------------------------------------------|
| ➕ Add a new book                     | <img src="https://github.com/user-attachments/assets/17322869-09a7-41d0-a258-6fdf34b7403d" width="30%" alt="Add Book"> |
| ✏️ Edit and update book              | <img src="https://github.com/user-attachments/assets/af9adfe8-cc7a-4258-9133-9554bb52902c" width="30%" alt="Edit Book"> |
| 🗑️ Delete book                       | <img src="https://github.com/user-attachments/assets/b7374475-4a5a-4a68-949a-c071334d5706" width="30%" alt="Delete Book"> |
| 👀 View all books                     | <img src="https://github.com/user-attachments/assets/9b939fe6-fa45-40cd-9d65-ef26fdac0686" width="30%" alt="View Books"> |

### 🔄 Resource Borrowing - Loans

| Operation                                 | Image                                                                                              |
|-------------------------------------------|----------------------------------------------------------------------------------------------------|
| 🆙 Start a loan                            | <img src="https://github.com/user-attachments/assets/7dcf260e-c53b-441f-958b-8485e316d49b" width="50%" alt="Start Loan"> |
| 🏁 Complete a loan                         | <img src="https://github.com/user-attachments/assets/002f69e4-ced9-46d8-ba1a-16a87a1ab270" width="50%" alt="Complete Loan"> |
| 📚 View all loans for a specific book      | <img src="https://github.com/user-attachments/assets/e86e8e6c-74e5-4807-ac9e-564cc8fa4ea2" width="50%" alt="View Loans for Book"> |
| 👥 View loans by reader                    | <img src="https://github.com/user-attachments/assets/8af57a67-3454-4e5b-94b3-94381af66e28" width="50%" alt="View Loans by Reader"> |

### 📧 Sending Email Notifications
- 📩 Send a "Welcome" email to the user upon account creation
- 📬 Send a "Loan Started" email to the reader when a book is borrowed
- 📥 Send a "Loan Completed" email to the reader upon book return

## 🛠️ Technologies

- **Backend:** Java, Spring Boot, Spring Security
- **Frontend:** Thymeleaf, Bootstrap, HTML5, CSS3, JavaScript, jQuery
- **Database:** Flyway, PostgreSQL
- **Containerization:** Docker
- **IDE:** IntelliJ IDEA

## 📊 Database Model

![Database Model](https://github.com/user-attachments/assets/9ed7b02b-569b-4765-95c3-d8f83b00bfbe)

The database for the Library Management System consists of the following tables and relationships between them:

### **Tables and Their Fields**

1. ### 🗂️ **category**
   | Field   | Type          | Description                          |
   |---------|---------------|--------------------------------------|
   | `id`    | integer (PK)  | Unique identifier for the category   |
   | `name`  | varchar       | Category name                        |

2. ### 🖋️ **work**
   | Field          | Type          | Description                         |
   |----------------|---------------|-------------------------------------|
   | `id`           | integer (PK)  | Unique identifier for the work      |
   | `title`        | varchar       | Work title                          |
   | `description`  | varchar       | Work description                    |

3. ### 👤 **author**
   | Field         | Type          | Description                         |
   |---------------|---------------|-------------------------------------|
   | `id`          | integer (PK)  | Unique identifier for the author    |
   | `first_name`  | varchar       | Author's first name                 |
   | `last_name`   | varchar       | Author's last name                  |

4. ### 📚 **book**
   | Field                 | Type          | Description                             |
   |-----------------------|---------------|-----------------------------------------|
   | `id`                  | integer (PK)  | Unique identifier for the book          |
   | `work_id`             | integer (FK)  | Reference to the work                   |
   | `publisher_name`      | varchar       | Publisher name                          |
   | `year_of_publishing`  | timestamp     | Year of publication                     |
   | `isbn`                | varchar       | Book ISBN                               |
   | `book_status`         | status        | Status of the book                      |
   | `available`           | boolean       | Availability of the book                |

5. ### 👥 **user**
   | Field             | Type          | Description                              |
   |-------------------|---------------|------------------------------------------|
   | `id`              | integer (PK)  | Unique identifier for the user           |
   | `first_name`      | varchar       | User's first name                        |
   | `last_name`       | varchar       | User's last name                         |
   | `password`        | varchar       | User's password                          |
   | `email`           | varchar       | User's email                             |
   | `date_of_birth`   | timestamp     | Date of birth                            |
   | `contact_number`  | varchar       | Contact number                           |
   | `enabled`         | boolean       | Activation status                        |

6. ### 📝 **loan**
   | Field            | Type          | Description                             |
   |------------------|---------------|-----------------------------------------|
   | `id`             | integer (PK)  | Unique identifier for the loan          |
   | `member_id`      | integer (FK)  | Reference to the reader                 |
   | `librarian_id`   | integer (FK)  | Reference to the librarian              |
   | `book_id`        | integer (FK)  | Reference to the book                   |
   | `date_issued`    | timestamp     | Issue date                              |
   | `date_returned`  | timestamp     | Return date                             |

7. ### 🔐 **role**
   | Field   | Type          | Description                              |
   |---------|---------------|------------------------------------------|
   | `id`    | integer (PK)  | Unique identifier for the role           |
   | `name`  | varchar       | Role name (Admin, Librarian, Member)     |

8. ### 🔗 **user_role**
   | Field      | Type          | Description                          |
   |------------|---------------|--------------------------------------|
   | `user_id`  | integer (FK)  | Reference to the user                |
   | `role_id`  | integer (FK)  | Reference to the role                |

9. ### 🔗 **work_author**
   | Field        | Type          | Description                          |
   |--------------|---------------|--------------------------------------|
   | `work_id`    | integer (FK)  | Reference to the work                 |
   | `author_id`  | integer (FK)  | Reference to the author               |

10. ### 🔗 **work_category**
    | Field          | Type          | Description                          |
    |-----------------|---------------|--------------------------------------|
    | `work_id`       | integer (FK)  | Reference to the work                 |
    | `category_id`   | integer (FK)  | Reference to the category             |

---

### 🔗 **Relationships Between Tables**

1. **work_author**:  
   - `work_id` ↔️ `work.id`  
   - `author_id` ↔️ `author.id`  

2. **work_category**:  
   - `work_id` ↔️ `work.id`  
   - `category_id` ↔️ `category.id`  

3. **book**:  
   - `work_id` ↔️ `work.id`  

4. **loan**:  
   - `member_id` ↔️ `user.id` (reader)  
   - `librarian_id` ↔️ `user.id` (librarian)  
   - `book_id` ↔️ `book.id`  

5. **user_role**:  
   - `user_id` ↔️ `user.id`  
   - `role_id` ↔️ `role.id`  

---

### 📝 **Key Points**

- **Primary Keys (PK)** ensure the uniqueness of records in each table.
- **Foreign Keys (FK)** establish relationships between tables and maintain data integrity.
- **Roles and Users** are linked through the intermediary table `user_role` to implement authorization.
- **Loans** connect books, readers, and librarians, tracking the issuance and return of books.
- **Books** are linked to works and can have multiple categories and authors through the tables `work_category` and `work_author`.

## 🚀 Getting Started

### 🔧 Requirements
You need to install the following:
- **Docker** along with **docker-compose**
- **Java Development Kit (JDK)**
- **Maven** (if not using the provided Maven Wrapper)

### ⚙️ Running the Application
Execute the following commands in the terminal:

1. **Navigate to the project folder (executed from the root directory of the repository):**
    ```bash
    cd library-management-system/
    ```
    ![Navigate to Project Folder](https://github.com/user-attachments/assets/37016f78-70c8-47ed-8381-e0ee26ef1ff2)

2. **Build the `.jar` file of the project in the `target` folder:**
    ```bash
    ./mvnw clean package -DskipTests
    ```
    ![Build Maven Project](https://github.com/user-attachments/assets/f3351b46-dfec-4263-b456-2753d52c0cda)

3. **Build and run the Docker environment and local web server:**
    ```bash
    docker-compose up
    ```
    *(Stop with `Ctrl+C`)*
    ![Run Docker Compose](https://github.com/user-attachments/assets/76c166a1-167c-4154-bb0d-7f50920e655f)

4. **Open the application in your browser:**
    [http://localhost:8080/](http://localhost:8080/)

**If you need to modify the code and apply changes:**

1. **Stop and remove Docker containers and their volumes:**
    ```bash
    docker-compose down
    ```
    ![Stop Docker Compose](https://github.com/user-attachments/assets/c6d0bdb3-7051-409a-8b25-0168b09858e3)

2. **Remove the Docker image `library-management-system.jar`:**
    ```bash
    docker rmi library-management-system.jar
    ```
    ![Remove Docker Image](https://github.com/user-attachments/assets/75961e05-d158-4a25-9c96-d4726f2b0f9c)

3. **Repeat steps 2-4.**

### 📦 Building Packages

You can create installer packages `.deb` and `.rpm` using `jpackage`. Follow these steps:

#### 📥 Prerequisites

- **To build a `.deb` package:**
  - Install `fakeroot`:
    ```bash
    sudo apt-get update
    sudo apt-get install fakeroot
    ```

- **To build a `.rpm` package:**
  - Install `rpm-build`:
    ```bash
    sudo apt-get update
    sudo apt-get install rpm
    ```

#### 🏗️ Building a `.deb` Package
Execute the following command from the root directory of the project:
```bash
jpackage --input target \
    --name LibraryManagementSystem \
    --main-jar library-management-system.jar \
    --type deb \
    --icon assets/images/icon.png \
    --dest out_dir
```
![Build .deb Package](https://github.com/user-attachments/assets/f2bd103d-8791-4944-b36f-b85de15f9903)

#### 🏗️ Building a `.rpm` Package
Execute the following command from the root directory of the project:
```bash
jpackage --input target \
    --name LibraryManagementSystem \
    --main-jar library-management-system.jar \
    --type rpm \
    --icon assets/images/icon.png \
    --dest out_dir
```
![Build .rpm Package](https://github.com/user-attachments/assets/fc2f13eb-507d-43f8-8652-43214d64e8da)

#### 🛠️ Additional Options
- `--app-version`: Specify the application version.
- `--icon`: Add an application icon (e.g., `icon.png`).
- `--dest`: Specify the directory to save the created package.

**Example with an icon:**
```bash
jpackage --input target \
    --name LibraryManagementSystem \
    --main-jar library-management-system.jar \
    --type deb \
    --icon assets/images/icon.png \
    --dest out_dir
```

**Notes:**
- Ensure you have JDK version 14 or higher installed, which includes `jpackage`.
- `jpackage` creates installer packages for the platform it is run on. To create a `.rpm` package, it is recommended to use RPM-based systems (e.g., Fedora or CentOS).

### 🗄️ Database Management
You can view the PostgreSQL database within IntelliJ IDEA's database window as follows:

1. **Navigate to:** `View -> Tool Windows -> Database`
2. **Add a new data source:**
    - Click the `+` button
    - Select `Data Source from URL` and enter the following details:

    **URL:** `jdbc:postgresql:///postgres`  
    **Driver:** `PostgreSQL`

3. **Configure connection properties:**
    - **Username:** `postgres`
    - **Password:** `postgres`
    - **Database:** `postgres`
    - **Host:** `localhost`
    - **Port:** `5432`

### ✉️ Email Sending Testing
**MailHog Web UI**, a tool for developers to test email sending, is available at: [http://localhost:8025/](http://localhost:8025/)
![MailHog Web UI](https://github.com/user-attachments/assets/5438a75d-b280-4aac-94cb-839e52d39aed)

## 👥 Credits

**Project Leader, Senior Developer, Chief Architect, Technical Director, Coffee Manager, Database Guru, Testing Engineer, Deployment Specialist, Interface Designer, Server Administrator, Chief Motivator, Meme Officer, System Oracle, Bug Master, Coding Legend, Drum Solo Performer, Commit Wizard, Production Safe Provider, Console King, Log Overlord, Lost Semicolon Finder, Merge Master, Chaos Documenter, Production Breaker (on Fridays), "It Works on My Machine" Specialist, Branch Lord, Deployment Key Keeper, Stack Trace Collector:**  
- **Aleksandr Murzin** 😘

---

**Programming in Java**  
**Faculty of Electrical Engineering and Information Technology of STU in Bratislava**

---
