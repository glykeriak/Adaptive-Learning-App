# Adaptive-Learning-App

## Overview
This project is an **Android Adaptive Learning Application** developed in **Java**.  
It is designed to help students learn **Python programming** through theory, interactive exercises, and quizzes.  
The app adapts learning content and activities to the student’s progress and stores results in **Firebase**.

Built with:
- **Java (Android SDK)** → application logic  
- **XML layouts** → UI design  
- **Firebase Authentication** → user login & registration  
- **Firebase Realtime Database** → progress tracking, quizzes, and lessons  

---

## System Architecture

### Authentication
- `MainActivity.java` → user login.  
- `SignUpActivity.java` → new user registration.  

### Home & Profile
- `HomeActivity.java` → entry point with lesson categories.  
- `ProfileActivity.java` → user details, progress, learning style.  

### Lessons & Theory
- `LessonPatternActivity.java` → lesson templates.  
- `ALTheoryActivity.java` → theoretical explanations with examples.  

### Adaptive Exercises
- `ALFillTheBlocksActivity.java` + `activity_alfill_the_blocks.xml` → fill-in-the-code blocks.  
- `ALSelectTheImageActivity.java` + `activity_alselect_the_image.xml` → select the correct image/answer.  
- `ALDragAndDropActivity.java` + `activity_aldrag_and_drop.xml` → reorder code blocks via drag & drop.  
- `ALChallengeActivity.java` → challenge-based adaptive tasks.  

### Quizzes
- `QuizActivity.java` + `activity_quiz.xml` → multiple-choice quizzes (expandable lists).  
- `quiz_list_group.xml`, `quiz_list_item.xml` → quiz UI templates.  

### Analytics
- `AdaptiveLearning.java` → progress analytics and adaptation engine.  


---

## Deployment
1. Install **Android Studio (latest version)**.  
2. Clone the repository:  
   ```bash
   git clone https://github.com/username/Unipi-Adaptive-Learning-App.git
3. Open the project in Android Studio.
4. Add your Firebase configuration file (google-services.json) into the app/ folder.
5. Sync Gradle and install dependencies.
6. Run the app on an emulator or a physical Android device (API 24+ recommended).

---

## Results

- Login & Register: Secure user authentication (Firebase).
- Home Screen: Displays lessons and navigation to exercises.
- Profile: Shows user info, progress, and learning style.
- Lessons: Theory pages with Python explanations and examples.
- Adaptive Exercises:
   * Fill-the-blocks coding tasks.
   * Select-the-image multiple-choice tasks.
   * Drag & Drop ordering tasks.
   * Challenge mode for advanced learners.
- Quizzes: Multiple-choice questions with expandable lists.
- Analytics: Tracks time spent, quiz scores, and lesson completion.
