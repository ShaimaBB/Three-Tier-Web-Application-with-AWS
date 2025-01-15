# Build a Three-Tier Web Application with AWS

This project taught me how to set up a three-tier web application using AWS services. It showcases the integration of the **presentation tier**, **logic tier**, and **data tier** to create a fully functional web application.

---


## Overview

### Project Objectives
- Implement a three-tier architecture:
  1. **Presentation Tier**: Frontend display and distribution of the website.
  2. **Logic Tier**: Backend logic using AWS Lambda and API Gateway.
  3. **Data Tier**: Database setup using DynamoDB.
- Connect the tiers for seamless data flow and user interaction.

### Time Taken
- Approximately 2.5 hours, including debugging and testing.

---

## Technologies Used

- **Amazon S3**: For storing and serving frontend files.
- **Amazon CloudFront**: For secure website distribution.
- **AWS Lambda**: For backend logic and handling API requests.
- **Amazon API Gateway**: For managing API endpoints.
- **Amazon DynamoDB**: For storing and querying user data.

---

## Architecture

![Three-Tier Architecture](https://github.com/ShaimaBB/AWS-projects/blob/a9512282dbf6a207c0351aab1e20c2824dd3f1d2/images/Screenshot%202025-01-14%20204905.png)

---

## Setup Steps

### 1. Presentation Tier
- **Tools Used**: Amazon S3, CloudFront.
- **Steps**:
  - Store the website files in an S3 bucket.
  - Set up CloudFront for secure distribution of the website.
  - Configure origin access control to restrict S3 access to CloudFront only.

### 2. Logic Tier
- **Tools Used**: AWS Lambda, API Gateway.
- **Steps**:
  - Create a Lambda function to handle user requests and interact with DynamoDB.
  - Use API Gateway to define endpoints for the Lambda function.
  - Ensure the Lambda function retrieves user data using the AWS SDK.

### 3. Data Tier
- **Tools Used**: Amazon DynamoDB.
- **Steps**:
  - Set up a DynamoDB table with `userId` as the partition key.
  - Store sample user data for testing.
  - Connect DynamoDB to the Lambda function.

---

## Error Handling

### CORS Errors
- **Issue**: API Gateway and Lambda by default block requests from CloudFront due to CORS restrictions.
- **Solution**:
  - Enable CORS in API Gateway for the `/user` resource.
  - Add `Access-Control-Allow-Origin` headers in Lambda function responses.
  - Reference the CloudFront domain in API Gateway’s settings.

---

## Testing

- **Steps**:
  1. Visit the CloudFront distribution URL.
  2. Enter a `userId` to test data retrieval.
  3. Verify JSON responses in the browser.

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

**Author:** Shaima Bashar
