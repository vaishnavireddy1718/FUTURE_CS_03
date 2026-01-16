# FUTURE_CS_03 – API Security Risk Analysis

## 📌 Internship Information
- Intern Name: Arra Vaishnavi Reddy  
- Domain: Cyber Security  
- Organization: Future Interns  
- Task Name: API Security Risk Analysis
- Task Number:03

## 🎯 Objective
The objective of this task is to analyze a public API endpoint and identify potential security risks related to authentication, authorization, data exposure, and access control. This task aims to build foundational knowledge of API security risks commonly observed in real-world applications.

## 🛠 Tool Used
- **Postman** – for sending API requests and analyzing responses  

## 🌐 API Tested
- **Endpoint:** https://jsonplaceholder.typicode.com/users  
- **HTTP Method:** GET  
- **Authentication:** Not implemented (Public API)  

## 🧪 Steps Performed
1. Opened the Postman application  
2. Created a new HTTP GET request  
3. Entered the public API endpoint  
4. Sent the request without authentication credentials  
5. Reviewed and analyzed the API response headers and body  

## 👀 Observations
- The API returned a successful **200 OK** response  
- User-like data such as name, email, address, and company details were visible  
- No authentication, authorization, or access restrictions were enforced  

## 🚨 Security Issues Identified

### 1. Missing Authentication
**Description:**  
The API endpoint allows access to user-related data without any authentication mechanism.

**Impact:**  
Unauthorized users can access user-like data. In real-world APIs, this could lead to data exposure, privacy violations, and misuse of personal information.

**Mitigation:**  
Implement strong authentication mechanisms such as API keys, OAuth 2.0, or JWT-based token authentication.

### 2. Excessive Data Exposure
**Description:**  
The API response exposes user-related information such as email addresses and physical address details.

**Impact:**  
Excessive data exposure increases the risk of privacy breaches, phishing attacks, and data scraping in real-world applications.

**Mitigation:**  
Limit API responses to only the required fields and avoid exposing unnecessary user information.

### 3. Lack of Access Control and Rate Limiting
**Description:**  
The API does not enforce role-based access control or restrict the number of requests per client.

**Impact:**  
Attackers can repeatedly access the endpoint, leading to potential abuse, scraping, or denial-of-service risks.

**Mitigation:**  
Apply role-based access control (RBAC) and implement rate limiting and request throttling.

## ⚠️ Risk Severity
- **Risk Level:** Medium  

**Justification:**  
Although the tested API provides mock data intended for development and testing, the absence of authentication, authorization, and rate limiting would be considered a serious security flaw if implemented in a real-world production environment.

## 📉 Risk Impact
- Unauthorized access to user-related data  
- Potential data exposure and privacy violations  
- Increased risk of automated data scraping and abuse  
- Possible non-compliance with data protection standards  

## ✅ Recommendations
- Implement strong authentication mechanisms (API keys, OAuth 2.0, JWT)  
- Enforce role-based access control (RBAC)  
- Apply rate limiting and throttling to prevent abuse  
- Restrict API responses to only necessary data fields  
- Enable logging and monitoring to detect suspicious activity  

## 📸 Screenshots
The `/screenshots` folder contains supporting screenshots of the Postman request and response to demonstrate the testing process and findings.

## 🏁 Conclusion
This task highlights the importance of securing APIs against unauthorized access and data exposure. While the tested API is designed for public testing purposes, similar security misconfigurations in real-world applications can result in serious privacy, compliance, and security risks. Implementing proper authentication, authorization, access control, and monitoring mechanisms is essential to ensure robust API security.

## 🔗 Repository Information
- **Track Code:** CS  
- **Repository Name Format:** FUTURE_CS_03  
- **Internship Program:** Future Interns Cyber Security Internship
