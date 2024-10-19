# Book Management System

## Overview
The **Book Management System** is a web application designed to manage a collection of books. This project utilizes **Java**, **Hibernate** for ORM, and **MySQL** as the database. The application allows users to add, display, and manage books efficiently.

## Features
- Add new books with details such as ID, name, and price.
- Display a list of all books stored in the database.
- User-friendly interface built with **Bootstrap** for responsive design.

## Technologies Used
- **Java**: Programming language used for building the application.
- **Hibernate**: ORM framework for database interactions.
- **MySQL**: Relational database management system to store book data.
- **JSP (JavaServer Pages)**: For creating dynamic web content.
- **Maven**: Dependency management and build automation tool.
- **Bootstrap**: Frontend framework for responsive design.

## Prerequisites
Before you begin, ensure you have met the following requirements:
- **Java Development Kit (JDK)** installed (version 1.8 or higher).
- **Apache Maven** installed to manage dependencies and build the project.
- **MySQL Server** installed and running on your machine.
- An IDE like **Eclipse** or **IntelliJ IDEA** for Java development.

## Getting Started

### Clone the Repository
To get a local copy of the project, clone the repository using:
```bash
git clone https://your-repo-url.git
cd BookWebProj
```

### Setup Database
1. Create a database named `project1db` in your MySQL server.
2. Ensure you have the necessary permissions to create tables in this database.

### Update Database Configuration
Edit the `hibernate.cfg.xml` file to configure your database connection settings:
```xml
<property name="hibernate.connection.url">jdbc:mysql://localhost:3306/project1db</property>
<property name="hibernate.connection.username">root</property>
<property name="hibernate.connection.password">root</property>
```
Make sure to update the username and password to match your MySQL credentials.

### Build the Project
Navigate to the project root directory and run:
```bash
mvn clean install
```
This command will compile the project and package it into a WAR file.

### Deploy the Application
1. Deploy the generated `BookWebProj.war` file (found in the `target` directory) to a servlet container such as **Apache Tomcat**.
2. Start your Tomcat server.

### Access the Application
Open your web browser and navigate to:
```
http://localhost:8080/BookWebProj/
```
You should see the home page of the Book Management System.

## How to Use

### Adding a Book
1. Click on **Add New Book** from the navigation menu.
2. Fill in the **Book Id**, **Book Name**, and **Book Price** fields.
3. Click **Save Book** to add the book to the database.

### Displaying Books
- Click on **Display Books** from the navigation menu to view all the books stored in the database.

## Code Structure

### Key Components
- **`src/main/java`**: Contains all Java source code files.
  - **`com.book.dao`**: Data Access Objects for interacting with the database.
  - **`com.book.entity`**: Entity classes representing database tables.
  - **`com.book.utility`**: Utility classes, including Hibernate configuration.
  
- **`src/main/resources`**: Contains configuration files like `hibernate.cfg.xml`.

- **`src/main/webapp`**: Contains JSP files for the web application user interface.

### Important Files
- **`hibernate.cfg.xml`**: Hibernate configuration file containing database connection settings.
- **`web.xml`**: Deployment descriptor that defines the web application structure and configurations.
- **`pom.xml`**: Maven configuration file for managing dependencies and build settings.

## Benefits of the Application
- **Simplicity**: Easy to use interface for managing book records.
- **Efficiency**: Uses Hibernate to efficiently handle database operations.
- **Scalability**: Can be extended to include more features like user authentication, searching, and filtering books.

## Contributing
Contributions are welcome! If you have suggestions for improvements or features, feel free to create a pull request or open an issue.

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgements
- [Hibernate ORM](https://hibernate.org/orm/)
- [Bootstrap](https://getbootstrap.com/)
- [MySQL](https://www.mysql.com/)

For further assistance, feel free to contact me at your-email@example.com.
```

### Customization Tips
- Replace `your-repo-url.git` with the actual URL of your Git repository.
- Update the email in the contact section to your actual email.
- You may want to add screenshots or examples of the application in use to enhance the README further.