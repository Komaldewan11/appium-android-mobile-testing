# Mobile-Application-Testing with Appium
Automated mobile testing project using Appium and Android Studio. Tests were executed on an Android emulator for a messaging application, covering functional flows, UI behavior, and device-specific scenarios.

**Project Overview**

Item              Details
Tool              Appium
Platform          Android (emulator via Android Studio) 
Test type         Automated functional, UI/UX 
Application       Android Messaging Application

**What's Tested**

Messaging flows — Send and receive messages on the Android emulator
UI/UX behavior — Screen rotation handling and layout stability
State management — Mark messages as unread, verify state persists
Data operations — Delete messages and confirm removal
Device conditions — Low battery simulation for edge case coverage

**Tech Stack**

Appium — Mobile test automation framework
Android Studio — Android emulator (AVD)
Java — Test scripting language
JUnit — Test runner

**Setup & How to Run**

Prerequisites
1. Install [Android Studio](https://developer.android.com/studio) and create an AVD emulator
2. Install [Appium](https://appium.io/) globally:
bash: npm install -g appium
appium driver install uiautomator2

3. Verify setup:
bash: appium-doctor --android

Start Appium server
bash: appium

Launch Android emulator
Open Android Studio → Device Manager → Start your AVD

Run tests through the terminal:
node sendMessage.js
node receiveMessage.js

**Key Learnings**

- Set up an end-to-end mobile test environment from scratch (Appium + Android Studio)
- Automated real device interactions on an Android emulator
- Tested device-specific scenarios like orientation changes and battery state
