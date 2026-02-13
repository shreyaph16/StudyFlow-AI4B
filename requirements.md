#  StudyFlow – System Requirements Document (SRD)

## 1.  Introduction

### 1.1 Purpose
This document defines the functional and non-functional requirements for **StudyFlow**, an AI-powered exam preparation and well-being platform designed for high-pressure competitive exams such as JEE and NEET.

### 1.2 Scope
StudyFlow integrates:
- Intelligent syllabus planning
- Machine learning-based performance prediction
- Adaptive test generation
- Personalized health and wellness management
- Mental health monitoring and support systems

The goal is to ensure academic excellence without compromising physical or mental health.

---

# 2. Functional Requirements

## 2.1 User Management

- FR-1: Users must be able to register and log in securely.
- FR-2: Users must be able to update their academic profile (exam type, subjects, syllabus progress).
- FR-3: Users must be able to input health metrics (weight, height, activity level).
- FR-4: Role-based access (Student, Admin, Mentor – future scope).

---

## 2.2 Study Planning Module

- FR-5: Users must be able to upload or select a syllabus.
- FR-6: The system must generate a structured study plan based on:
  - Remaining topics
  - Completed topics
  - Available study hours
- FR-7: The system must dynamically reschedule tasks if the user misses a session.
- FR-8: Weekly and daily study plans must be generated automatically.

---

## 2.3 Adaptive Testing Module

- FR-9: The system must generate topic-based tests.
- FR-10: Difficulty must adapt based on previous performance.
- FR-11: The system must store test history.
- FR-12: Users must receive performance analytics after each test.

---

## 2.4 Performance Prediction (ML)

- FR-13: The system must analyze topic-wise accuracy.
- FR-14: The system must predict improvement trends.
- FR-15: Weak areas must be highlighted automatically.
- FR-16: The system must recommend focus topics based on prediction models.

---

## 2.5 Diet & Health Module

- FR-17: The system must calculate TDEE based on user input.
- FR-18: Personalized meal plans must be generated.
- FR-19: Activity sessions (Yoga, meditation, exercise) must be scheduled.
- FR-20: Users must be able to track daily health compliance.

---

## 2.6 Mental Health Monitoring

- FR-21: Weekly psychological assessments must be conducted.
- FR-22: The system must detect early stress indicators.
- FR-23: Users must have access to therapist contact support.
- FR-24: Emergency grievance helplines must be visible in high-risk cases.

---

## 2.7 Notifications & Alerts

- FR-25: Reminders for study sessions.
- FR-26: Alerts for missed tasks.
- FR-27: Wellness check reminders.
- FR-28: Burnout risk notifications (future ML feature).

---

# 3.  Non-Functional Requirements

## 3.1 Performance

- NFR-1: API response time < 500ms under normal load.
- NFR-2: System must support at least 10,000 concurrent users (scalable architecture).

---

## 3.2 Security

- NFR-3: Secure authentication using JWT.
- NFR-4: Encrypted storage of sensitive user data.
- NFR-5: Role-based access control.
- NFR-6: Compliance with student data privacy standards.

---

## 3.3 Reliability

- NFR-7: 99% uptime target.
- NFR-8: Automated backup of user data.
- NFR-9: Error logging and monitoring system.

---

## 3.4 Scalability

- NFR-10: Horizontal scalability using containerized deployment.
- NFR-11: Modular AI agents for independent scaling.

---

## 3.5 Usability

- NFR-12: Mobile-first design.
- NFR-13: Clean and distraction-free UI.
- NFR-14: Simple onboarding process (<5 minutes).

---

# 4.  AI Agent Requirements

## 4.1 Test Generator Agent
- Must create balanced tests across topics.
- Must adjust difficulty dynamically.

## 4.2 Score Prediction Agent
- Must use Gradient Boosting models.
- Must retrain periodically with new data.

## 4.3 Diet Recommender Agent
- Must rank meals based on caloric needs and preferences.

## 4.4 Scheduling Agent
- Must generate conflict-free schedules.
- Must adapt to missed sessions automatically.

---

# 5.  System Constraints

- Must run on:
  - React Native frontend
  - FastAPI backend
  - PocketBase (SQLite) database
- Must support integration with Gemini API.
- Must operate with minimal latency in AI inference.

---


# 7.  Acceptance Criteria

StudyFlow will be considered complete when:

- All core modules (Planning, Testing, Prediction, Health Monitoring) function end-to-end.
- AI predictions demonstrate measurable accuracy improvement.
- Users can maintain both academic and wellness tracking seamlessly.
- System passes security and load testing benchmarks.

---

#  Conclusion

StudyFlow aims to redefine exam preparation by combining:

> Academic Intelligence + Health Intelligence

This requirements document ensures that student well-being remains as critical as academic performance.
