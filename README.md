
# ABC-QA-Automation (Java - Appium)

This repository contains Appium automation scripts in Java for the ABC Company mobile app.
It includes two main flows:
- Attendance Report Search
- Check-IN & Leave Application

## Prerequisites
- Java 11+
- Maven
- Appium Server
- Android SDK & adb
- Connected Android device or emulator

## Setup
1. Start Appium server:
   appium
2. Build project dependencies:
   mvn clean compile

## Run scripts
Replace placeholder IDs (resource-ids/xpaths) in the source files under `src/main/java/com/abc/qa` before running.
Run AttendanceSearch:
mvn exec:java -Dexec.mainClass="com.abc.qa.AttendanceSearch"

Run CheckInLeave:
mvn exec:java -Dexec.mainClass="com.abc.qa.CheckInLeave"

## Notes
- Update `appPackage`, `appActivity`, and element locators to match the app under test.
- Screenshots captured will be saved to `/screenshots`.

