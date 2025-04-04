# LTUassignment


## Overview

The LTU Degree Tracker App is a mobile application designed to help students at Leeds Trinity University (LTU) and similar institutions manage their academic progress. The app provides features such as grade tracking, degree classification calculations, performance analytics, and goal setting, all within a user-friendly interface. This app addresses the common challenge students face in tracking academic progress, calculating degree classifications, and managing study goals.

### Sign-In Layout

This project includes an XML layout file (`activity_sign_in.xml`) that defines the user interface for a simple sign-in screen using `RelativeLayout`. The layout consists of:

- Email Input Field (`EditText`): Positioned at the top, with a hint "Email" and input type set to email address.
- Password Input Field (`EditText`): Positioned below the email input field with a hint "Password" and input type set to password (hidden).
- Sign-In Button (`Button`): Positioned below the password input field with a "Sign In" text, centered horizontally.

### How to Use the Sign-In Layout

1. Place `activity_sign_in.xml` in the `res/layout` directory of your Android project.
2. Link this layout to an Activity in your Java/Kotlin code using:
   ```java
   setContentView(R.layout.activity_sign_in);
   ```
3. Access UI elements in your Java/Kotlin code:
   ```java
   EditText emailEditText = findViewById(R.id.emailEditText);
   EditText passwordEditText = findViewById(R.id.passwordEditText);
   Button signInButton = findViewById(R.id.signInButton);
   ```
4. Add functionality to handle user input and authentication in your activity.

---

## Features

### 1. Sign-In
- Secure login through email, social media, or guest access, ensuring that the app's data is personalized and protected.

### 2. Main Screen
- Dashboard that offers quick navigation to key features such as Degree Classification, Grade Tracker, and Academic Progress.

### 3. Academic Progress Tracker
- Allows users to view and track their weekly academic progress and completed tasks. This feature supports reflection on academic milestones and achievements.

### 4. Degree Classification Calculator
- Users can input grades and credits to calculate their degree classification for Foundation, Undergraduate, and Postgraduate levels. The app also supports "What-If" scenarios to help students assess potential outcomes for different grades.

### 5. Grade Tracker
- Track grades for different modules, set academic goals, and receive notifications for incomplete or missing data. The app helps users visualize their academic performance and track the achievement of personal goals.

### 6. Degree Tracker
- Allows users to track their overall progress toward completing their degree. This feature includes tools to simulate degree progression based on current and projected grades.

### 7. Gamification
- The app includes a reward system where users can earn badges and achievements for completing tasks, hitting academic milestones, and staying on top of their goals.

### 8. Performance Analytics
- Users can visualize their academic performance through graphs and analytics, helping them to understand their strengths and areas for improvement. Tailored feedback is provided to enhance the learning experience.

### 9. Academic Calendar
- Sync deadlines, exam schedules, and result publications to ensure that users are always prepared for key academic events.

---

## Design and Implementation

### Sign-In Layout 
The `activity_sign_in.xml` layout defines the structure for a simple sign-in screen.

UI Components  
- Email Input Field (`EditText`): Positioned at the top with a margin of 100dp. The hint is "Email," and the input type is set to email.
- Password Input Field (`EditText`): Positioned below the email input with a 20dp margin. The hint is "Password," and the input type is set to password (hidden).
- Sign-In Button (`Button`): Positioned below the password input with a 20dp margin. Text is "Sign In," and the button is centered horizontally.

How to Use the Sign-In Layout 
1. Place the `activity_sign_in.xml` in the `res/layout` directory of your Android project.
2. Link this layout to your Activity with the following code:
   ```java
   setContentView(R.layout.activity_sign_in);
   ```
3. Access the UI components in your Java/Kotlin code:
   ```java
   EditText emailEditText = findViewById(R.id.emailEditText);
   EditText passwordEditText = findViewById(R.id.passwordEditText);
   Button signInButton = findViewById(R.id.signInButton);
   ```

Future Enhancements for the Sign-In Layout
- Implement a Forgot Password link.
- Add a Sign Up button for new users.
- Improve the UI with Material Design components.
- Implement form validation to ensure the correct input format.

---

## Reflection on App Design and Plan for Implementation

The app follows an object-oriented approach and employs core Android development techniques, including activities, fragments, and layouts. It ensures user data privacy and security with an authentication system that integrates email, social media logins, and password recovery. Advanced features such as degree classification calculation, grade tracking, and gamification offer a comprehensive solution to track academic progress.

### Challenges and Solutions
- Challenges: Ensuring smooth user authentication.
  - Solution: Implemented secure login mechanisms with social media and email options.
  
- Challenge: Database connectivity for saving user data.
  - Solution: Integrated Firebase for storing user data, grades, and academic progress securely.

- Challenge: Limited time to implement additional features.
  - Solution: I applied for mitigation to extend the deadline but unfortunately did not get accepted. If granted more time, I would have added more features, including advanced analytics, additional notifications, and further database optimization.

### Monetisation Plan
- In-App Purchases: Offer premium features such as advanced analytics and personalized academic coaching.
- Ads: Integrate non-intrusive ads to generate revenue while keeping basic features free for students.
- Subscription Model: Provide a subscription for unlimited access to degree simulations and notifications.

---

## Database Connection and Features

The app connects to a database (Firebase) to store user data, track grades, and maintain academic progress. Features requiring database access include the Sign-In Activity, Degree Classification, Grade Tracker, and Academic Progress Tracker.

## Evidence of Testing

Testing has been conducted using Android Studio's Layout Validation tool to validate the UI on different screen sizes. Additionally, JUnit tests have been performed for basic functionalities such as user login and grade tracking.

## Future Enhancements

- Advanced Analytics: Integrate predictive analysis to help students forecast future grades and degree classifications.
- University Integration: Sync with university databases to automatically fetch academic data.
- Accessibility Features: Implement customizable themes for better accessibility.

---

## Learning Resources

For development guidance, I referred to the following YouTube channels for Android Studio tutorials:

1. The Net Ninja: Provides great tutorials on Android development.
2. Android Developers: The official channel with in-depth tutorials on building Android apps.
3. CodeWithHarry: Another popular channel for Android development basics and advanced topics.

---

## Use of ChatGPT

During the backend development process, I sought assistance from **ChatGPT** to understand how to efficiently implement Firebase for user authentication and data storage. This tool helped me solve challenges in backend logic and integrate the necessary features for storing grades and academic progress securely.


