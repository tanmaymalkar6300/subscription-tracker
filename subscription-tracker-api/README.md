
<div align="center">
  <br />
    <a href="https://youtu.be/rOpEN1JDaD0?si=WfOjLV57WfR9x6QK" target="_blank">
      <img src="https://i.ibb.co/xtTbHkfs/Readme-Thumbnail.png" alt="Project Banner">
    </a>
  <br />

  <div>
    <img src="https://img.shields.io/badge/node.js-339933?style=for-the-badge&logo=Node.js&logoColor=white" alt="Node.js" />
    <img src="https://img.shields.io/badge/express.js-000000?style=for-the-badge&logo=express&logoColor=white" alt="Express.js" />
    <img src="https://img.shields.io/badge/mongodb-13aa52?style=for-the-badge&logo=mongodb&logoColor=white" alt="MongoDB" />
  </div>

  <h3 align="center">Subscription Management API</h3>

  <div align="center">
    A backend service for handling subscription data, user authentication, reminders, and more — built using Node.js, Express, and MongoDB.
  </div>
</div>

---

## 📌 Table of Contents

1. [Overview](#overview)
2. [Tech Stack](#tech-stack)
3. [Features](#features)
4. [Getting Started](#getting-started)
5. [Code Snippet](#code-snippet)
6. [External Services](#external-services)
7. [Extras](#extras)

---

## 🤖 Overview

This project is a backend API for managing subscriptions — ideal for SaaS platforms or any product offering recurring services. It covers key areas such as:

- User authentication via JWT
- Secure subscription data handling
- Automated email reminders
- Error handling, logging, and more

It’s inspired by a video tutorial and restructured to deepen backend development understanding by working with real-world use cases like bot protection, request rate limiting, and cloud-based workflows.

[📺 Tutorial Reference](https://youtu.be/rOpEN1JDaD0?si=WfOjLV57WfR9x6QK)

---

## ⚙️ Tech Stack

- **Node.js** – runtime environment  
- **Express.js** – backend framework  
- **MongoDB** – NoSQL database  
- **Mongoose** – ODM for MongoDB

---

## 🔋 Features

- ✅ **JWT-Based Authentication** for user sign-up and session control  
- ✅ **Subscription Management** with CRUD operations  
- ✅ **Advanced Rate Limiting & Bot Protection** using Arcjet  
- ✅ **Email Reminders** via Upstash workflows  
- ✅ **Centralized Error Handling** middleware  
- ✅ **Environment-based Configuration** with `.env`  
- ✅ **Code Architecture Designed for Scalability**

---

## 🚀 Getting Started

### Prerequisites

Ensure you have the following installed:

- Git  
- Node.js  
- npm  

### Steps to Run Locally

```bash
# Clone the repository
git clone https://github.com/adrianhajdin/subscription-tracker-api.git
cd subscription-tracker-api

# Install dependencies
npm install
````

### Environment Setup

Create a `.env.local` file and add:

```env
PORT=5500
SERVER_URL=http://localhost:5500
NODE_ENV=development
DB_URI=your_mongo_uri
JWT_SECRET=your_secret
JWT_EXPIRES_IN=1d
ARCJET_KEY=your_key
ARCJET_ENV=development
QSTASH_URL=http://127.0.0.1:8080
QSTASH_TOKEN=your_token
EMAIL_PASSWORD=your_email_password
```

### Run the Server

```bash
npm run dev
```

Visit [http://localhost:5500](http://localhost:5500) in Postman or browser.

---

## 🧩 Code Snippet

<details>
<summary>Sample Subscription Object</summary>

```json
{
  "name": "JavaScript Mastery Elite Membership",
  "price": 139.00,
  "currency": "USD",
  "frequency": "monthly",
  "category": "Entertainment",
  "startDate": "2025-01-20T00:00:00.000Z",
  "paymentMethod": "Credit Card"
}
```

</details>

---

## 🌐 External Services Used

* 🔐 **Arcjet** – App protection and bot filtering
* 📤 **Upstash** – Queue-based email workflows
* 📧 **Nodemailer** – For transactional emails

---

