# 🚗 SmartPark Enterprise

### Intelligent Parking Management System for Enterprises

<p align="center">
  <img src="Screenshot 2026-06-18 202909.png" alt="SmartPark Enterprise" width="100%"/>
</p>

<p align="center">
  <b>Oracle VBCS + Oracle Integration Cloud + Oracle Fusion HCM</b><br>
  Enterprise-grade Smart Parking Management Solution
</p>

---

## 📌 Project Overview

SmartPark Enterprise is a cloud-based intelligent parking management system designed to automate parking slot allocation, employee verification, vehicle registration, booking management, and parking ticket generation for enterprise organizations.

The application integrates Oracle Visual Builder Cloud Service (VBCS), Oracle Integration Cloud (OIC), and Oracle Fusion HCM to provide a seamless employee parking experience.

---

## 🎯 Business Problem

Managing employee parking manually leads to:

* Parking congestion
* Duplicate slot allocation
* Poor parking visibility
* Security concerns
* Administrative overhead

SmartPark Enterprise eliminates these challenges by automating the complete parking lifecycle.

---

## 🚀 Key Features
  <img src="Screenshot 2026-06-18 202909.png" alt="SmartPark Enterprise" width="100%"/>

### 👤 Employee Authentication

* Employee registration
* Login validation
* Fusion HCM employee verification
* Role-based access control

### 🚘 Vehicle Management

* Register multiple vehicles
* Vehicle ownership validation
* Vehicle profile maintenance

### 🅿️ Smart Slot Management

* Real-time parking slot availability
* Zone-wise parking allocation
* Slot occupancy tracking

### 📅 Parking Reservation

* Book available parking slots
* Prevent duplicate bookings
* Booking history tracking

### 🎫 Parking Ticket Generation

* Auto-generated booking ticket
* Employee details
* Vehicle information
* Slot information
* Booking timestamps

### 🚪 Vehicle Exit Processing

* Exit tracking
* Automatic slot release
* Parking utilization management

### 📊 Dashboard Analytics

* Total Slots
* Available Slots
* Occupied Slots
* Registered Vehicles
* Total Bookings

---

# 🏗️ Solution Architecture

```text
Employee
    │
    ▼
Oracle VBCS UI
    │
    ▼
Action Chains
    │
    ├──────────────► Users BO
    │
    ├──────────────► Vehicles BO
    │
    ├──────────────► Bookings BO
    │
    ├──────────────► Parking Slots BO
    │
    ▼
Oracle Integration Cloud
    │
    ▼
Oracle Fusion HCM
```

---

# 🔄 End-to-End Booking Workflow

```text
Login
  │
  ▼
Fusion Employee Validation
  │
  ▼
Vehicle Selection
  │
  ▼
Available Slot Selection
  │
  ▼
Create Booking
  │
  ▼
Update Slot Status
(AVAILABLE → OCCUPIED)
  │
  ▼
Generate Parking Ticket
  │
  ▼
Dashboard Update
```

---

# 🔐 Login Validation Flow

```text
User Login
   │
   ▼
Users Business Object
   │
   ▼
Validate Email & Password
   │
   ▼
Call OIC Integration
   │
   ▼
Fusion HCM Validation
   │
   ▼
Person Number Verification
   │
   ▼
Login Success
```

---

# 🗄️ Business Objects

## Users

| Field        |
| ------------ |
| id           |
| fullName     |
| email        |
| employeeId   |
| mobileNumber |
| role         |
| status       |

---

## Vehicles

| Field         |
| ------------- |
| id            |
| vehicleNumber |
| vehicleType   |
| manufacturer  |
| model         |
| color         |
| ownerId       |

---

## ParkingSlots

| Field      |
| ---------- |
| id         |
| slotNumber |
| slotType   |
| slotStatus |
| zone       |

---

## Bookings

| Field         |
| ------------- |
| id            |
| bookingDate   |
| bookingStatus |
| vehicle       |
| user          |
| parkingSlot   |

---

# 🔧 Technology Stack

## Frontend

* Oracle Visual Builder Cloud Service (VBCS)
* Oracle JET Components
* JavaScript
* HTML5
* CSS3

## Integration Layer

* Oracle Integration Cloud (OIC)

### Integration Types

* Scheduled Integration
* App Driven Integration
* REST Integration

## Backend

* Visual Builder Business Objects

## External Systems

* Oracle Fusion HCM

---

# 📡 Integrations Implemented

### Employee Verification Integration

Fusion HCM → OIC → VBCS

Purpose:

* Employee validation
* Employee onboarding verification

---

### Employee Welcome Notification Flow

Fusion HCM
↓
OIC Scheduled Integration
↓
Filter IBM Employees
↓
Generate Welcome Message
↓
Email Notification

---

# 📈 Dashboard Metrics

The dashboard provides real-time parking analytics.

### KPIs

* Total Parking Slots
* Available Slots
* Occupied Slots
* Registered Vehicles
* Total Bookings

---

# 🎫 Parking Ticket Example

```text
================================

SMARTPARK PARKING TICKET

================================

Employee Name : Glenn Bolt

Employee ID   : 3034

Vehicle No    : HR5538X6391

Vehicle Type  : CAR

Slot Number   : A07

Status        : ACTIVE

Booking Time  : 22-Jun-2026

================================
```

---

# 📚 Documentation Deliverables

### Project Documentation

* Business Requirements
* Functional Design
* Technical Design
* Data Model Design
* Integration Design
* Security Design
* Deployment Guide
* User Guide

### Diagrams

* Solution Architecture Diagram
* Login Workflow Diagram
* Booking Workflow Diagram
* Vehicle Exit Workflow Diagram
* OIC Integration Flow Diagram
* Entity Relationship Diagram

---

# 👨‍💻 Team Members

### Vivek Tripathi

Oracle Integration Cloud & VBCS Developer

### Vishnu M S

Application Developer

### Sanket Kulkarni

Application Developer

---

# 🌟 Project Highlights

✅ Oracle Fusion HCM Integration

✅ Oracle Integration Cloud Automation

✅ Visual Builder Business Objects

✅ Real-Time Parking Availability

✅ Ticket Generation

✅ Enterprise Authentication

✅ Role-Based Security

✅ Cloud Native Architecture

---

## 📜 License

This project was developed as part of an Oracle Cloud Enterprise Application initiative and is intended for educational and demonstration purposes.

---

<p align="center">
<b>SmartPark Enterprise</b><br>
Transforming Enterprise Parking Management Through Oracle Cloud Technologies
</p>
