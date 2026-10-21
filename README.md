# 📚 E-Learning Mobile Application

An interactive Android learning application built with **Java, Android Studio, and Firebase**, designed to help students explore programming concepts, study code examples, attempt quizzes, and track their performance through a leaderboard.

## ✨ Features

### 🔐 Authentication & Profile Management
- User registration and login with Firebase Authentication
- Profile management with custom profile pictures
- User data storage using Firebase Realtime Database
- Session persistence and user-state management

### 📖 Interactive Learning
- Chapter-based learning modules
- Grid-based subject and topic navigation
- Programming content covering Java, Android development, PHP, and JavaScript
- Firebase-powered dynamic content, where configured

### 💻 Programming Examples
- Code viewer with syntax highlighting using CodeView
- Examples covering algorithms and data structures
- Graph algorithms, including DFS, BFS, Dijkstra's, Kruskal's, and Prim's
- Examples involving arrays, stacks, linked lists, and problem-solving techniques

### 🎯 Quiz & Assessment
- Quiz questions loaded from Firebase
- Multiple-choice questions with answer feedback
- Score calculation and performance tracking
- Interactive quiz screens and question transitions

### 🏆 Leaderboard & Gamification
- User score tracking
- Leaderboard with user names and profile pictures
- Ranking and score comparison
- A competitive learning experience

### 🎨 User Interface
- Material Design components
- Navigation drawer and bottom navigation
- RecyclerView-based lists
- Splash screen and organized learning screens
- Interfaces designed for different Android screen sizes

## 🛠️ Technology Stack

| Category | Technologies |
|---|---|
| Language | Java |
| IDE | Android Studio |
| Backend Services | Firebase Authentication, Realtime Database, Firebase Storage |
| UI Components | Material Design, Navigation Components, RecyclerView |
| Image Loading | Glide, CircleImageView |
| Code Display | CodeView Android library |
| Build System | Gradle with Kotlin DSL |

## 📱 Screenshots

The following screenshots illustrate the application's main learning and assessment workflows.

### Home & Learning Modules

![Subjects Overview](assests/subjects.png)

*Dashboard displaying available programming subjects.*

![Subject Course Template](assests/subject_course_template.png)

*Course structure and chapter-based learning modules.*

![Subjects Topics](assests/subjects_topics.png)

*Topic selection within a subject.*

### Authentication

![User Registration](assests/registeer_fir_new_user.png)

*Registration screen for new learners.*

![Successful Registration](assests/successful_register.png)

*Registration confirmation interface.*

![Login for Quiz](assests/login_for_quiz.png)

*Login interface for accessing learning and quiz features.*

### Quiz & Assessment

![Start Quiz Page](assests/start_quiz_page.png)

*Quiz entry screen.*

![Attempt Quiz Subject](assests/attempt_quiz_subject.png)

*Subject-specific quiz selection.*

![User Attempt Quiz Questions](assests/user_attempt_its_quizs_question.png)

*Multiple-choice quiz interface.*

![Question with Code Templates](assests/question_with_solution_of_code_templates.png)

*Programming questions featuring code examples and solutions.*

### Leaderboard & Scores

![Leaderboard Scores](assests/leaderboard_scores.png)

*Leaderboard displaying user scores and rankings.*

![Leaderboard Registration](assests/ui_to_show_yo_open_leaderbporad_register_itsef_for_quiz.png)

*Interface related to leaderboard access and quiz registration.*

> **Screenshot note:** The image paths above preserve the names in the original README. Confirm that the `assests/` directory exists in the repository and that each filename matches exactly. If the folder is actually named `assets/`, update the paths accordingly.

## ⚙️ Prerequisites

- Android Studio
- A compatible JDK and Gradle version as specified by the project
- Android SDK
- An Android emulator or physical Android device
- A Firebase project with the required services enabled

The original project documentation specifies Android API 28 as the minimum SDK and API 34 as the target SDK. Confirm these values against the current Gradle configuration.

## 🚀 Installation & Setup

### 1. Clone the Repository

```bash
git clone https://github.com/ZunaishaN00R/E-Learning-App-in-Java-on-Android-Studio.git
cd E-Learning-App-in-Java-on-Android-Studio
```

### 2. Open the Project

1. Launch Android Studio.
2. Select **Open** and choose the cloned project directory.
3. Allow Gradle to synchronize the project.
4. Resolve any missing SDK or dependency requirements.

### 3. Configure Firebase

1. Create or select a project in the [Firebase Console](https://console.firebase.google.com/).
2. Register the Android application using its actual package name.
3. Download `google-services.json`.
4. Place the file in the application's `app/` directory.
5. Enable Email/Password authentication.
6. Configure Realtime Database and Firebase Storage as required by the application.
7. Verify the Firebase security rules before testing.

**Important:** Use your own Firebase project configuration. Never commit private credentials or sensitive service-account keys to the repository.

### 4. Build and Run

Select an Android emulator or connect a physical device with USB debugging enabled. Then build and run the application from Android Studio.

Alternatively, from the project root, use the Gradle wrapper on Windows:

```powershell
.\gradlew.bat assembleDebug
```

The debug APK is normally generated under:

```text
app/build/outputs/apk/debug/app-debug.apk
```

## 🗂️ Project Structure

```text
app/
└── src/
    └── main/
        └── java/
            └── com/zunaisha/e_learning_app/
                ├── authentication/
                ├── chapter/
                ├── chaptertopics/
                ├── leaderboard/
                ├── ui/
                │   ├── code/
                │   ├── home/
                │   └── quiz/
                ├── MainActivity.java
                └── SplashScreen.java
```

*This is the structure documented for the project; verify package and directory names against the current source code.*

## 🗄️ Firebase Data Organization

The original documentation describes a Realtime Database structure similar to the following:

```text
Firebase Realtime Database
├── Score/
│   └── {userId}/
│       ├── name
│       ├── image
│       └── score
└── Questions/
    └── {questionId}/
        ├── question
        ├── option1
        ├── option2
        ├── option3
        ├── option4
        └── answer
```

The actual database paths and field names should match the application's Firebase read/write operations. Apply appropriate security rules to protect user information, quiz answers, and scores.

## 🔍 Learning Outcomes

This project demonstrates practical Android development concepts, including:

- Java-based Android application development
- Firebase authentication and database integration
- Profile image handling and cloud storage
- Dynamic content loading
- Quiz logic and score management
- RecyclerView-based interfaces
- Code presentation and algorithm learning
- UI navigation and application state management

## 🤝 Contributing

Contributions and suggestions are welcome.

1. Fork the repository.
2. Create a feature branch:

   ```bash
   git checkout -b feature/your-feature
   ```

3. Commit your changes:

   ```bash
   git commit -m "Add your feature"
   ```

4. Push the branch:

   ```bash
   git push origin feature/your-feature
   ```

5. Open a pull request describing your changes.

## 📄 License

This project is documented as being licensed under the MIT License. See the [`LICENSE`](LICENSE) file to verify the license terms before reusing or distributing the code.

## 👩‍💻 Authors

**Zunaisha N00R**
- GitHub: [@ZunaishaN00R](https://github.com/ZunaishaN00R)

**Usmana Zulfiqar**
- GitHub: [@usmana0820](https://github.com/usmana0820)
- Email: usmanazulfiqar20@gmail.com

## 🙏 Acknowledgments

- Firebase for authentication and cloud services
- Google and the Android community for development tools and resources
- Material Design for UI components and design guidance
- CodeView library for code syntax highlighting

---

⭐ If you find this project useful, consider giving the repository a star.

