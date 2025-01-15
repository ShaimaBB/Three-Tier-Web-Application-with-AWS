# Connect a Web App to Amazon Aurora

This project demonstrates how to connect a web application to Amazon Aurora, an AWS relational database service. It highlights the integration process, backend and frontend interactions, and database functionality.
                      

---

## Introduction

Amazon Aurora is an AWS relational database service optimized for high performance and scalability. This project involves:
- Setting up a web application using PHP and MariaDB.
- Integrating the application with Amazon Aurora for real-time data updates.
- Observing how backend database changes reflect on the frontend.

  ![Architectue](https://github.com/ShaimaBB/AWS-projects/blob/be89b88d6f5bd587881b371f938351d5c3fbe28c/images/Aurora%20Architectural%20diagram.png)


---

## Technologies Used

- **AWS Services:** Amazon Aurora, EC2
- **Backend:** PHP, MariaDB
- **Web Server:** Apache
- **Database Client:** MySQL CLI
- **Development Tools:** SSH, Key Pair for EC2 connection

---

## Features

- Integration of a web application with an Amazon Aurora database.
- Ability to submit and view data via a web interface.
- Real-time reflection of backend database changes on the frontend.

---

## How It Works

- The web application interacts with the Amazon Aurora database through the configured EC2 instance.
- A backend script processes form submissions and updates the Aurora database.
- Changes in the database are reflected in the frontend table, demonstrating the real-time connection.

---

## Testing

- Install MySQL CLI to test database queries.
- Run SQL commands to validate that the database contains the expected data.
- Verify that changes made through the web interface are accurately reflected in the database.

---

## Conclusion

This project provided me with a hands-on experience in connecting a web application to Amazon Aurora.

---


- [AWS Amazon Aurora Documentation](https://aws.amazon.com/rds/aurora/)

---

