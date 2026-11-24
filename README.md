# Serverless AI Cloud Fun Facts Generator

A serverless web application built on AWS that dynamically generates and serves cloud computing fun facts using the **Google Gemini API** and **Python AWS Lambda**.

## Architecture Flow
`User Browser (AWS Amplify)` → `Amazon API Gateway (REST API)` → `AWS Lambda (Python)` → `Google Gemini API` & `Amazon DynamoDB`

## Tech Stack
* **Frontend:** HTML, CSS, JavaScript (`index.html`), hosted on AWS Amplify
* **Backend:** Python (AWS Lambda)
* **API & Database:** Amazon API Gateway, Amazon DynamoDB (NoSQL)
* **AI Integration:** Google Gemini API

## How It Works
1. The user requests a cloud fun fact from the web interface hosted on **AWS Amplify**.
2. **Amazon API Gateway** routes the incoming request to a **Python AWS Lambda** function.
3. **Lambda** queries **Amazon DynamoDB** for stored facts or calls the **Google Gemini API** to generate a fresh fact, saves it in DynamoDB, and returns the JSON response to the frontend.

*(Note: Live AWS resources were torn down after demonstration to avoid ongoing cloud billing. Full walkthrough screenshots and presentation slides are included in this repository.)*

---

## Live Website Preview

### Fun Fact Generator UI
![Fun Fact Generator UI 1](AWS%206.png)
![Fun Fact Generator UI 2](AWS%207.png)

---

## AWS Cloud Infrastructure & Implementation

### 1. Frontend Hosting — AWS Amplify
![AWS Amplify](AWS%201.png)

### 2. API Routing — Amazon API Gateway
![Amazon API Gateway](AWS%202.png)

### 3. Serverless Backend — AWS Lambda (Python)
![AWS Lambda](AWS%203.png)

### 4. NoSQL Storage — Amazon DynamoDB
![Amazon DynamoDB Table](AWS%204.png)
![Amazon DynamoDB Items](AWS%205.png)
