# CS-360

Welcome to the CS-360 repository! This repository contains my final mobile application developed as part of Southern New Hampshire University's **CS-360: Mobile Architecture and Programming** course. Throughout this course, I learned how to design and develop Android applications with a focus on user-centered design, data persistence, application functionality, and compatibility across Android devices.

The primary project featured in this repository is **WeighPoint**, a weight-tracking Android application developed from the initial UI design through a fully functional application.

---

# About the Course

CS-360 focuses on the design and development of mobile applications for the Android platform. Throughout the course, I worked through the complete mobile development process, beginning with identifying user needs and designing the user interface before implementing the application's functionality in Android Studio.

Key topics covered include:

- User-centered mobile application design
- Android Studio development
- XML-based user interfaces
- Java application development
- Activity navigation
- SQLite database integration
- CRUD database operations
- User authentication
- Runtime permissions
- SMS functionality
- Android version compatibility
- Mobile application testing
- Application launch planning

---

# What You Will Find Here

This repository contains the completed application developed throughout the course.

## Project Three

**WeighPoint Weight Tracking Application**

WeighPoint is an Android application designed to provide users with a simple way to record their weight and monitor progress toward a personal weight goal.

The application includes:

- User account creation and login
- Weight entry creation and editing
- Weight history
- Weight entry deletion
- Goal weight tracking
- Progress calculations
- Dashboard with recent entries
- SQLite data persistence
- Optional SMS goal notifications
- Navigation between the primary application screens

The completed Project Three ZIP contains the Android Studio project, including the finalized user interface originally designed during Project Two and the functionality implemented during Project Three.

---

# User Needs and UI Design

The primary goal of WeighPoint was to create a straightforward weight-tracking application that allows users to record and monitor their progress without unnecessary complexity. Users needed an easy way to enter weight information, review previous entries, establish a goal, and quickly understand their current progress.

To support these needs, I designed separate screens for login, the main dashboard, adding and editing weight entries, weight history, goal settings, and SMS notification settings. A consistent bottom navigation system allows users to move between the major sections of the application.

The interface uses consistent colors, typography, buttons, icons, and layouts throughout the application. Important information such as current weight, goal progress, and recent entries is presented directly on the dashboard so users do not have to navigate through several screens to find their most relevant information.

Keeping the interface consistent and focused on the application's core functions helped create a user-centered design that remained easy to understand as additional functionality was introduced.

---

# Development Approach

I approached the development of WeighPoint incrementally rather than attempting to implement the entire application at once. I first established the user interface and navigation before connecting the application to its SQLite database and implementing the primary functionality.

Features were then added and tested individually, including user authentication, CRUD operations for weight records, goal tracking, progress calculations, and SMS notifications. Breaking development into smaller components made debugging easier because problems could be isolated to recently added functionality.

I also spent time reviewing and organizing the completed source code, XML layouts, resources, and comments before finalizing the project. This helped ensure that the completed application was not only functional but also understandable and maintainable.

This incremental development strategy can be applied to future software projects because it allows individual components to be tested before they become part of a larger and more complex system.

---

# Testing and Compatibility

Testing was an important part of developing WeighPoint. I tested account creation, login, navigation, adding weight records, editing and deleting records, goal calculations, database persistence, and SMS permission handling throughout development.

I also tested the application using multiple Android emulator configurations. The minimum SDK was lowered to **API 26 (Android 8.0 Oreo)**, which Android Studio indicated would allow the application to support approximately **98.4% of Android devices**.

Testing on an older Android emulator revealed an important compatibility difference. The application's core weight-tracking features continued to function correctly, but SMS notifications did not successfully send on the older emulator. SMS functionality worked correctly when tested on newer Android versions.

The application was designed so that SMS remains optional. If an SMS notification cannot be sent, the user's weight entry is still saved and the application informs the user that the notification could not be delivered.

This experience demonstrated why successful compilation alone is not enough to verify an application. Testing across different Android versions can reveal compatibility issues that may not appear in the primary development environment.

---

# Challenges and Problem Solving

One of the largest challenges during development was connecting the different parts of the application while keeping the data synchronized. A single weight entry can affect several areas of WeighPoint, including weight history, the dashboard, recent entries, goal calculations, and potentially SMS notifications.

Another challenge involved Android compatibility and SMS functionality. Rather than allowing an optional feature to prevent users from recording their weight, I separated SMS functionality from the application's core database operations. This allowed the application to continue functioning even when SMS permission was denied or a notification could not be sent.

I also had to consider differences in how information should be presented to the user. For example, weight entry dates from the current year are displayed without a year, while entries from previous years include the year. Small changes such as this helped make the application easier to read while still providing users with the information they need.

---

# Areas of Success

I was particularly successful in integrating the SQLite database with the rest of the application. WeighPoint supports creating, reading, updating, and deleting weight records while ensuring that information remains associated with the correct user account.

The database is also connected to other application features rather than functioning as an isolated component. Saved weight information is used to populate the dashboard and history screen, determine the user's current and starting weights, calculate progress toward a goal, and determine when goal-related functionality should occur.

This part of the project allowed me to demonstrate several skills together, including Java programming, Android UI development, database management, input validation, activity navigation, permissions, and user-centered design.

---

# Why This Project Matters

WeighPoint represents the complete process of turning an initial mobile application concept into a functional Android application. The project began by considering user needs and designing an appropriate interface before progressing into database development, application logic, testing, compatibility, and launch planning.

One of the most important lessons I learned was that mobile development involves more than making an application work on a single device. Developers must consider different Android versions, screen layouts, permissions, hardware capabilities, user expectations, and situations where optional functionality may not be available.

The finished application demonstrates my ability to combine these considerations into a functional mobile application while continuing to focus on the needs of the user.

---

# Future Applications

The skills developed throughout CS-360 can be applied to future mobile and software development projects. Moving forward, I plan to continue using several of the practices reinforced during this course:

- Designing software around clearly identified user needs
- Developing and testing features incrementally
- Separating optional functionality from core application features
- Testing software across multiple environments and configurations
- Maintaining organized and clearly commented code
- Considering compatibility early in the development process
- Requesting only the permissions an application actually needs
- Designing interfaces that remain consistent and easy to navigate
- Testing error conditions instead of only successful scenarios

The experience of designing, developing, testing, and preparing WeighPoint for a potential release provided a stronger understanding of the complete mobile application development lifecycle.
