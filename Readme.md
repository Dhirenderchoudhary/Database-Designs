
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

# 2. Fitness Management System – ER Diagram

##  Overview
This project represents the **database design (ER Diagram)** for a fitness platform where trainers provide plans, clients subscribe to them, attend sessions, and track their progress over time.

The system supports real-world features like subscriptions, payments, workout sessions, and fitness tracking.

---

## Objectives
- Manage users (trainers & clients)
- Allow trainers to create fitness plans
- Enable clients to subscribe to plans
- Track payments and sessions
- Monitor client progress and check-ins

---

##  Entities Included

###  Users
Stores common user information for both trainers and clients.

###  Trainers
Contains trainer-specific details like specialization and experience.

###  Clients
Stores client-specific data like fitness goals and activity level.

###  Plans
Created by trainers, includes workout/diet plans.

###  Client Subscriptions
Links clients to plans with duration and status.

### Payments
Handles payment records for subscriptions.

###  Sessions
Tracks scheduled training sessions.

###  Check-ins
Logs client check-ins during training.

###  Progress Logs
Tracks body metrics like weight, body fat, etc.

### Trainer Feedback
Stores trainer feedback for each check-in.

---

##  Design Highlights
- Normalized database design (no redundancy)
- Clear separation of roles (trainer vs client)
- Scalable structure for real-world usage
- Tracks complete user journey:
  Plan → Subscription → Payment → Session → Progress


##  Diagram
You can view the ER diagram directly on GitHub by clicking the image file in the repository or by using the link below:

[View the ER Diagram](./Fitness%20Influencer%20Coaching%20Platform.png)

---

# 3. Clinic Management System – ER Diagram

## Overview

This project represents the database design (ER Diagram) for a clinic platform where patients can book appointments with doctors, attend consultations, undergo diagnostic tests, and receive reports.

The system supports real-world clinic operations like appointment scheduling, doctor consultations, diagnostic testing, report generation, and payments.

## Objectives
Manage patients and doctors
Organize appointments efficiently
Track consultations (actual visits)
Allow doctors to prescribe diagnostic tests
Generate and store test reports
Handle payments for appointments
Maintain complete patient visit history
Entities Included
Patients

Stores patient details such as name, contact information, and date of birth.

## Doctors

Contains doctor information along with their assigned specialty.

## Specialties

Defines different medical specialties (e.g., cardiology, dermatology).

## Appointments

Represents booking between a patient and a doctor at a scheduled time.
Includes status like booked, cancelled, completed, or no-show.

## Consultations

Represents the actual visit after an appointment.
Not all appointments result in consultations (e.g., no-show cases).

## Tests (Diagnostics)

Contains available diagnostic tests with description and pricing.

## Prescribed Tests

Links consultations with tests prescribed by doctors.
Tracks the status of each test.

## Reports

Stores diagnostic reports generated after tests are completed.
Each report corresponds to a prescribed test.

## Payments

Handles payment transactions related to appointments.
Includes payment method and status.


Patient → Appointment → Consultation → Prescribed Tests → Reports → Payment

# 4. Comic-Con Parking Management System – ER Diagram

##  Overview
This project represents the **database design (ER Diagram)** for a large-scale Comic-Con event parking system where thousands of vehicles enter and exit across multiple days.

The system manages vehicle entry, parking allocation, reserved zones, ticket generation, session tracking, and payment processing in a structured and scalable way.

---

##  Objectives
- Track vehicles entering the venue  
- Manage different vehicle categories (bike, car, SUV, EV, etc.)  
- Allocate parking spots efficiently  
- Support reserved parking (VIP, staff, exhibitors, cosplayers, EV charging)  
- Record entry and exit timestamps  
- Generate parking tickets  
- Track parking sessions  
- Handle payment and billing  
- Monitor parking availability across zones and floors  

---

##  Entities Included

###  Users
Stores basic user/owner details of vehicles.

### Vehicles
Represents vehicles entering the parking facility.

###  Vehicle Categories
Defines types of vehicles (bike, car, SUV, EV, etc.).

###  Parking Floors
Represents different levels in the parking structure.

###  Parking Categories
Defines reserved types of parking (VIP, staff, exhibitor, EV charging, etc.) along with pricing.

###  Parking Zones
Subdivisions within floors, mapped to parking categories.

###  Parking Spots
Individual parking spots within zones.

###  Parking Sessions
Tracks entry and exit of vehicles. Each session represents one visit.

###  Tickets
Generated when a vehicle enters the parking facility.

###  Payments
Stores payment details for each parking session.

---

##  Relationships
- One user can own multiple vehicles  
- One vehicle belongs to one category  
- One floor contains multiple parking zones  
- One zone belongs to a parking category  
- One zone contains multiple parking spots  
- One vehicle can have multiple parking sessions  
- One parking spot can be reused across multiple sessions  
- One session generates one ticket  
- One session is linked to a payment

# 4. Comic-Con Parking Management System 

##  Overview
This project represents the **database design (ER Diagram)** for a large-scale **event parking system** used in venues like Comic-Con India.

The system is designed to manage **high-volume, multi-day parking operations** involving different types of vehicles, reserved parking categories, and real-time parking allocation.

It supports structured parking with **zones, levels, and categorized spots**, along with tracking **sessions, tickets, and payments**.

---

##  Objectives
- Manage different types of vehicles (bike, car, SUV, EV, etc.)
- Organize parking into zones and levels
- Allocate parking spots based on availability and category
- Track vehicle entry and exit (sessions)
- Generate parking tickets
- Handle payments and pricing
- Support reserved categories (VIP, staff, exhibitors, etc.)
- Maintain real-time parking availability

---

## Entities Included

###  Visitors
Stores visitor details such as name, email, and role.
Roles include: `cosplayer`, `exhibitor`, `creator`, `staff`, `VIP`, `general`.

---

###  Vehicles
Stores vehicle information and links to:
- Vehicle type (bike, car, etc.)
- Owner (visitor)

---

###  Vehicle Types
Defines categories of vehicles.

---

###  Levels
Represents different parking levels (floors).

---

###  Zones
Each level contains multiple zones for better organization.

---

###  Parking Spots
Represents individual parking slots.
Tracks:
- Zone
- Category
- Availability status

---

###  Spot Categories
Defines types of parking spots (e.g., general, VIP, EV charging).

---

###  Spot-Vehicle Mapping
Handles compatibility between vehicle types and spot categories.

---

###  Parking Sessions
Tracks actual parking activity:
- Entry time
- Exit time
- Assigned spot
- Status (active/completed)

---

### Tickets
Generated when a vehicle enters the parking facility.
Linked to parking sessions.

---

### Payments
Handles payment transactions for each parking session:
- Amount
- Payment method
- Payment status

---

###  Pricing
Defines parking rates based on vehicle type.






