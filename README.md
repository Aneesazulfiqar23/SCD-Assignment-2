# Software Construction and Development — Assignment 2

This repository organizes the submitted materials for the SCD Assignment 2.

## Project: CampusConnect
The supplied Java Swing prototype is a Smart University Student Portal. It demonstrates attendance warnings, lecture updates, complaint submission, subject notes, and in-app notifications.

## Assignment parts
- **Part 1 — Survey:** questionnaire and two respondent summary.
- **Part 2 — Analysis:** development-method, testing-tool, and challenge chart data.
- **Part 3 — Java prototype:** CampusConnect source code, project notes, and test cases.
- **Part 4 — GitHub:** feature branch, commits, pull requests, and team contribution record.
- **Part 5 — Report/demo:** prepare the final report, screenshots, source-code archive, and classroom demonstration.

## Repository structure
```
docs/
  GIT_WORKFLOW.md
  TEAM_CONTRIBUTIONS_TEMPLATE.md
  survey/
    survey-summary.md
    survey-chart-data.md
  prototype/
    prototype-design-reference.md
java-project/
  CampusConnect/
    README.md
    PROJECT_OVERVIEW.md
    TESTING.md
    src/campusconnect/*.java
    test/campusconnect/CampusConnectTest.java
```

## Run the Java prototype
Install JDK 17 or later, open a terminal in `java-project/CampusConnect`, then run:

```bash
javac -d out src/campusconnect/*.java
java -cp out campusconnect.App
```

Run the included test harness:

```bash
javac -d out src/campusconnect/*.java test/campusconnect/CampusConnectTest.java
java -ea -cp out campusconnect.CampusConnectTest
```

## Important notes before submission
- The survey summary records the information present in the supplied documents; verify the original interview records and respondent details before final submission.
- The supplied survey chart data has a few chart labels with spelling inconsistencies; these are preserved in the source note where relevant.
- The Java prototype uses local serialized-file storage, not a shared online database. Fine/payment, SMS, email, and push-payment features are not implemented.
- Screenshots in the prototype design document include design/reference screens and should not be described as screenshots of the Java Swing application unless they actually show that application.
- Record real contributor names and work only. Commits made by the repository owner remain attributed to that GitHub account; do not claim they were made by other members.
