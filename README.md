# 🚀 API Automation Testing Portfolio: FakeStore Project
[![Postman](https://img.shields.io/badge/Postman-FF6C37?style=for-the-badge&logo=postman&logoColor=white)](https://www.postman.com/)
[![Node.js](https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white)](https://nodejs.org/)
[![Testing](https://img.shields.io/badge/QA-Automation-green?style=for-the-badge)](https://www.istqb.org/)

## 📌 Project Overview
This repository showcases a professional-grade API Automation Testing Framework using **Postman** and **Newman**. By simulating an End-to-End (E2E) testing lifecycle for an E-commerce platform (FakeStoreAPI), this project demonstrates advanced test automation logic and engineering best practices.

### 🎯 Key Engineering Objectives
- **Authentication Security**: Validating JWT-based Bearer Token authorization flows.
- **Dynamic Data Chaining**: Extracting runtime variables (e.g., Product IDs) from responses and passing them as dependencies to subsequent requests.
- **Contract Testing**: Implementing **JSON Schema Validation** to ensure API responses strictly adhere to defined data structures and types.
- **Resilience Strategy**: Handling non-persistent mock server behaviors with robust assertion logic to ensure CI/CD pipeline stability.

---

## 🛠 Tech Stack
- **Tooling**: Postman (Scripting via JavaScript / Chai.js)
- **CLI Runner**: Newman
- **CI/CD Readiness**: Compatible with Jenkins and GitHub Actions integration
- **Standards**: Designed based on **ISTQB CTFL** test design principles

---

## 📂 Repository Structure
- `FakeStore_API_Collection.json`: The core test suite containing Login and CRUD operation logic.
- `FakeStore_Environment.json`: Environment template (Sanitized/De-sensitized; includes Base URL only).

---

## 🚀 Execution Guide (Local Setup)

1. **Install Newman**:
   ```bash
   npm install -g newman
2. Run Tests via CLI:
   newman run "FakeStore_API_E2E_Automation.postman_collection.json" -e "FakeStore_Environment.json" --reporters cli
