# CampusConnect — Project overview

## Problem addressed
University students need one place to view attendance warnings, lecture changes, classroom updates, complaint status, and subject study-material listings.

## Main modules
- **Presentation:** Java Swing interface in `MainFrame`.
- **Services:** `CampusService` and `NotificationService`.
- **Models:** `AttendanceRecord`, `Lecture`, `Complaint`, `SubjectNote`, and `NotificationItem`.
- **Persistence:** `DataManager` serializes `DataStore` to a local file.
- **Tests:** `CampusConnectTest` exercises model validation and service/notification behavior.

## SCD concepts demonstrated
- OOP through separate model and service classes.
- Encapsulation through private model fields and methods.
- Modular separation of UI, services, models, persistence, and notifications.
- Observer design pattern through `NotificationObserver` and `NotificationService`.
- Exception handling for invalid user input and file I/O.
- Basic test harness in the `test` folder.

## Prototype limitations
- Attendance figures and the 75% threshold are demonstration data, not an official university policy.
- Fine is only a warning/status; no real fine is calculated or paid.
- Study materials are catalogue entries; PDF files are not uploaded/opened by this prototype.
- Notifications are in-app only, not SMS, email, or push notifications.
- Data is saved locally, not in a shared online database.
