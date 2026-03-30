# 🏗️ BuildQCheck (BuildZone QA Monitor)

## 📖 About

BuildQCheck is a comprehensive Android application designed for construction field workers and site managers.
It enables real-time quality inspections, issue reporting, material compliance checks, and site progress tracking using Firebase Firestore.

---

## ✨ Features

### 🔐 Authentication

* Email/password login & signup
* Forgot password support
* Email verification via Firebase

### 🏠 Dashboard

* Grid-based home screen
* Quick access to Add Site, Site List, Feedback, About

### 📋 Site Management

* Add, update, and manage construction sites
* Supports Residential / Commercial / Industrial

### ✅ Quality Check

* Radio-based quality quiz
* Covers: Bricks, Steel, Concrete, Waterproofing, Wiring, Plaster, Fire Door

### ⚠️ Issue Reporting

* Log safety/quality issues
* Category dropdown + description
* Stored in Firebase

### 📊 Site Details

* Detailed site overview
* Status:

  * 🟢 Active
  * 🔵 Completed
  * 🟡 To Start

### 📚 Material Reference

* IS 456:2000
* NBC 2016

### 💬 Feedback

* Star rating + comments

### 👤 Profile

* View account
* Logout & delete account

---

## 🗂️ App Navigation

```
HomeScreen
├── AddSiteScreen
├── SiteListScreen
│   └── SiteDetailsScreen
│       ├── SiteActionsScreen
│       │   ├── CheckQualityScreen
│       │   └── ReportIssueScreen
├── MaterialInfoFragment
├── FeedbackScreen
├── AboutScreen
└── ProfileFragment
```

---

## 🛠️ Tech Stack

* Language: Kotlin
* UI: XML + View Binding
* Architecture: Activity + Fragment
* Backend: Firebase Firestore, Firebase Auth

---

## 🚀 Getting Started

### Prerequisites

* Android Studio Flamingo+
* Android SDK 24+
* Firebase project

### Firebase Setup

* Add `google-services.json` to `/app`
* Enable Authentication (Email/Password)
* Enable Firestore

---

## 📁 Project Structure

```
app/src/main/java/com/example/bqc/
├── SplashScreen.kt
├── SignIn.kt
├── SignUp.kt
├── MainActivity.kt
├── AddSite.kt
├── SiteList.kt
├── SiteDetails.kt
├── QualityQuiz.kt
├── ReportIssues.kt
└── Feedback.kt
```

---

## 🔥 Firebase Collections

```
sites/
feedback/
report/
```

---







