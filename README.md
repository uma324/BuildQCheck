# 🏗️ BuildQCheck (BuildZone QA Monitor)

## 📖 About the Project

BuildQCheck is an Android application developed to simplify **construction site monitoring and quality assurance**.
The idea behind this app is to help **site engineers, supervisors, and field workers** manage construction activities efficiently without relying on manual paperwork.

tracking quality checks, reporting issues, and maintaining site data can be time-consuming and error-prone. This app solves that problem by providing a **centralized, digital solution** where users can monitor site progress, perform quality inspections, and report issues in real time.

The application is fully integrated with **Firebase**, enabling secure authentication and real-time database updates.

---

## ✨ Key Features

### 🔐 User Authentication

The app provides a secure authentication system using Firebase:

* Email and password login/signup
* Password recovery functionality
* Email verification for added security

---

### 🏠 Dashboard

The home screen is designed with simplicity in mind:

* Clean grid layout for easy navigation
* Quick access to core modules like site management, feedback, and materials info

---

### 📋 Site Management

Users can manage multiple construction sites efficiently:

* Add new site details (type, budget, materials, timeline)
* View all registered sites in a structured list
* Update site progress and status

Supports different types of projects:

* Residential
* Commercial
* Industrial

---

### ✅ Quality Inspection System

A unique feature of the app is the built-in **quality assessment module**:

* Interactive radio-based questionnaire
* Covers key construction components such as:

  * Bricks
  * Steel
  * Concrete
  * Waterproofing
  * Wiring
  * Plaster
  * Fire safety

This helps ensure that construction standards are being followed consistently.

---

### ⚠️ Issue Reporting

Users can quickly report any problems observed on-site:

* Select issue category (safety/quality)
* Add detailed description
* Data is stored in Firebase Firestore

This enables better tracking and accountability.

---

### 📊 Site Details & Status Tracking

Each site includes a detailed overview with clear status indicators:

* 🟢 Active
* 🔵 Completed
* 🟡 To Start

This helps users quickly understand project progress at a glance.

---

### 📚 Material Standards Reference

The app also includes a reference section for construction standards:

* IS 456:2000 (Concrete standards)
* NBC 2016 guidelines

These are displayed through simple popup windows for quick access during inspections.

---

### 💬 Feedback System

Users can provide feedback directly within the app:

* Star-based rating system
* Optional text comments
* Stored in Firebase for analysis

---

### 👤 User Profile

Basic profile management features include:

* View account information
* Logout
* Delete account

---

## 🗂️ Application Flow

```text
Home Screen
│
├── Add Site → Register new construction site
├── Site List → View all sites
│   └── Site Details → Detailed site information
│       ├── Quality Check → Perform inspection
│       └── Report Issue → Log problems
│
├── Material Info → View construction standards
├── Feedback → Submit user feedback
├── About → App information
└── Profile → Account management
```

---

## 🛠️ Tech Stack

This project is built using modern Android development tools:

* **Language:** Kotlin
* **UI Design:** XML layouts with View Binding
* **Architecture:** Activity + Fragment-based structure
* **Backend:** Firebase

  * Firebase Authentication
  * Cloud Firestore

Additional components used:

* RecyclerView for lists
* Spinner (ArrayAdapter) for dropdowns
* PopupWindow for material info
* Toast messages for user feedback

---

## 🚀 Getting Started

### 🔧 Requirements

* Android Studio (Flamingo or newer)
* Android SDK 24+
* Firebase project setup

---


## 📁 Project Structure

```text
app/src/main/java/com/example/bqc/
├── Authentication (SignIn, SignUp, ForgotPassword)
├── MainActivity & Navigation
├── Home & Fragments
├── Site Management (AddSite, SiteList, SiteDetails)
├── Quality & Reporting (QualityQuiz, ReportIssues)
└── Feedback & About
```

---

## 🔥 Firebase Database Design

The app uses structured Firestore collections:

* **sites** → Stores all site-related information
* **feedback** → Stores user ratings and comments
* **report** → Stores reported issues

---

## 💡 What I Learned

While building this project, I gained hands-on experience in:

* Designing real-world Android applications
* Working with Firebase Authentication & Firestore
* Structuring multi-screen apps using Activities & Fragments
* Implementing user-friendly UI/UX for practical use cases

---







