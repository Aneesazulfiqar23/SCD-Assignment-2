# CampusConnect — Test cases

| ID | Test | Steps | Expected result |
|---|---|---|---|
| TC-01 | Load dashboard | Start application | Dashboard opens and sample records appear |
| TC-02 | Low attendance flag | Open Attendance & Fine | A subject below 75% is marked LOW |
| TC-03 | Cancel lecture | Select a lecture and click Cancel selected lecture | Status changes to Cancelled and notification is created |
| TC-04 | Change room | Select a lecture, click Change room, enter Room 20 | Room changes and notification is created |
| TC-05 | Empty room validation | Try changing room with blank input | Error message is displayed |
| TC-06 | Submit complaint | Enter category and message of 5+ characters | Complaint appears with Submitted status |
| TC-07 | Invalid complaint | Submit a message shorter than 5 characters | Validation error is displayed |
| TC-08 | Add subject note | Enter subject, title, and description | Note appears in subject material table |
| TC-09 | Persistence | Add a complaint, close and reopen app | Complaint remains saved |
| TC-10 | Observer notification | Cancel a lecture | Notification table updates automatically |

## Lightweight test harness
Compile and run:

```bash
javac -d out src/campusconnect/*.java test/campusconnect/CampusConnectTest.java
java -ea -cp out campusconnect.CampusConnectTest
```
