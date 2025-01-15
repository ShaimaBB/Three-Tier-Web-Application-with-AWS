# Build a Three-Tier Web Application with AWS

This project taught me how to set up a three-tier web application using AWS services by integration of the **presentation tier**, **logic tier**, and **data tier** to create a fully functional web application.
Documentation of this entire project is here
---


## Overview

### Project Objectives
- Implement a three-tier architecture:
  1. **Presentation Tier**: Frontend display and distribution of the website.
  2. **Logic Tier**: Backend logic using AWS Lambda and API Gateway.
  3. **Data Tier**: Database setup using DynamoDB.
- Connect the tiers for seamless data flow and user interaction.

---

## Features

- **Amazon S3**: For storing and serving frontend files.
- **Amazon CloudFront**: For secure website distribution.
- **AWS Lambda**: For backend logic and handling API requests.
- **Amazon API Gateway**: For managing API endpoints.
- **Amazon DynamoDB**: For storing and querying user data.

---

## Architecture

![Three-Tier Architecture](https://github.com/ShaimaBB/AWS-projects/blob/a9512282dbf6a207c0351aab1e20c2824dd3f1d2/images/Screenshot%202025-01-14%20204905.png)

---

- **Expected Output**:
  - User data is successfully retrieved and displayed on the web app.

---

## Lessons Learned

1. **CORS Challenges**:
   - Configuring CORS is crucial for integrating the presentation and logic tiers.
2. **End-to-End Testing**:
   - Testing individual components ensures smooth integration.
3. **AWS SDK**:
   - Simplifies interaction with AWS services like DynamoDB.

---
## Resources
- [NextWork Projects](https://community.nextwork.org/c/i-have-a-question?automatic_login=true)
- 
**Author:** Shaima Bashar
