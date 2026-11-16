# CampusConnect — Smart University Student Portal

A Java Swing desktop prototype for a centralized student portal.

## Features
1. Attendance overview and low-attendance warning.
2. Lecture schedule, lecture cancellation, and room changes.
3. Student complaint submission and status listing.
4. Subject-wise slides/notes catalogue.
5. In-app notifications generated using the Observer design pattern.

## Requirements
- JDK 17 or later (JDK 8+ may work with a compatible compiler).
- No external libraries or database setup required.

## Run on Windows
Open a terminal in this folder and execute:

```bash
javac -d out src/campusconnect/*.java
java -cp out campusconnect.App
```

## Run tests

```bash
javac -d out src/campusconnect/*.java test/campusconnect/CampusConnectTest.java
java -ea -cp out campusconnect.CampusConnectTest
```

The application stores demo data in `campusconnect-data.ser` in its working directory.
