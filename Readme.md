# 1. Instagram Thrift Creator Store ER Diagram

This repository contains the Entity-Relationship (ER) diagram for an Instagram-based Thrift Creator Store. 

## Overview

The ER diagram visualizes the database architecture and entity relationships required to manage a thrift store operated by a creator on Instagram. It outlines the core entities representing the store's operations, which likely include users (creators/customers), products (thrift items), orders, and payments.

## Contents

- **`Instagram Thrift Creator Store.png`**: The high-resolution visual representation of the ER diagram.

## Viewing the Diagram

You can view the ER diagram directly on GitHub by clicking on the image file in the repository or by following this link:
[View the ER Diagram](./Instagram%20Thrift%20Creator%20Store.png)

## Use Cases

This diagram serves as a blueprint and can be used as a reference for:
- Understanding the database schema for a social media-based e-commerce storefront.
- Developing and setting up a relational database for a thrift store application.
- Extending or modifying the database architecture for similar creator-economy projects.

## Contributing

Feel free to fork this project, submit pull requests, or open issues if you have suggestions for improving the database design or adding new entities.

# 2. 🏋️ Fitness Management System – ER Diagram

## 📌 Overview
This project represents the **database design (ER Diagram)** for a fitness platform where trainers provide plans, clients subscribe to them, attend sessions, and track their progress over time.

The system supports real-world features like subscriptions, payments, workout sessions, and fitness tracking.

---

## 🎯 Objectives
- Manage users (trainers & clients)
- Allow trainers to create fitness plans
- Enable clients to subscribe to plans
- Track payments and sessions
- Monitor client progress and check-ins

---

## 🧱 Entities Included

### 👤 Users
Stores common user information for both trainers and clients.

### 🧑‍🏫 Trainers
Contains trainer-specific details like specialization and experience.

### 🧑 Clients
Stores client-specific data like fitness goals and activity level.

### 📋 Plans
Created by trainers, includes workout/diet plans.

### 🔁 Client Subscriptions
Links clients to plans with duration and status.

### 💳 Payments
Handles payment records for subscriptions.

### 📅 Sessions
Tracks scheduled training sessions.

### 📍 Check-ins
Logs client check-ins during training.

### 📈 Progress Logs
Tracks body metrics like weight, body fat, etc.

### 📝 Trainer Feedback
Stores trainer feedback for each check-in.

---

## 🔗 Relationships
- One user can be a trainer or client  
- One trainer can create multiple plans  
- One client can subscribe to multiple plans  
- One subscription is linked to payments  
- One subscription can have multiple sessions  
- One session leads to check-ins  
- One check-in has progress logs and feedback  

---

## 🧠 Design Highlights
- Normalized database design (no redundancy)
- Clear separation of roles (trainer vs client)
- Scalable structure for real-world usage
- Tracks complete user journey:
  Plan → Subscription → Payment → Session → Progress

---

## 🛠 Tools Used
- Eraser.io (for ER Diagram)

---

## 📷 Diagram
You can view the ER diagram directly on GitHub by clicking on the image file in the repository or by following this link:
[View the ER Diagram](./Coaching)


---

