# StudAudio

**Allowing users to school on-the-go with audio.**

StudAudio strives to alleviate stress for older adult students by providing them the flexibility to engage in readings and assignments using our app, even during commutes or while attending to family responsibilities. With this app, adult learners can conveniently accomplish tasks during their commutes — such as listening to readings in the form of podcasts, submitting assignments through audio, and taking and sharing notes with others.

## Key Pages

1. **Sign In** — Users can log in with their username/password, with options to sign up or reset a forgotten password.
2. **Home Screen** — Contains the list of all classes a user is currently enrolled in.
3. **Class Screen** — Includes access to assignments, notes, and reading tasks:
   - *Simple Task*: Submit assignments (listen to or read the question, then submit an answer through speech)
   - *Moderate Task*: Listen to or read course materials
   - *Complex Task*: Create and share a note (create a note, edit its content and name, and share it via messages, Gmail, Slack, etc.)
4. **Connect Screen** — Classmates taking the same courses are recommended, and users can swipe right to send a connection request.
5. **FAQ Screen** — List of frequently asked questions and answers.

## Getting Started

### Prerequisites

- [Node.js and npm](https://nodejs.org/)
- Expo CLI — install globally with:
  ```bash
  npm install -g expo-cli
  ```
- Xcode (for the iOS simulator) — install from the Mac App Store, then:
  ```bash
  xcode-select --install
  ```
  Open Xcode once to accept the license agreement.

### Installation

```bash
git clone https://github.com/yasserajamal/StudAudio.git
cd StudAudio
npm install
```

### Running the App in Simulator

```bash
expo start
```

This starts the Expo development server and opens the Expo developer tools in your browser. From there, click **"Run on iOS simulator"** to build and launch the app.

## Troubleshooting

**Invariant Violation — Native Module Doesn't Exist**
Ensure all dependencies are properly installed. Run `npm install` again in the project root.

**Build Issues**
Try cleaning the project in Xcode (`Product` → `Clean Build Folder`) and rebuild.

**Simulator Doesn't Launch**
Make sure Xcode is correctly installed with all necessary components. If the simulator doesn't start automatically, open it manually via `Xcode` → `Open Developer Tool` → `Simulator`.

**Audio Not Working**
Try refreshing the app, or test on a simulator running iOS 15.x or earlier.

**Ejecting from Expo**
If needed, eject to a bare workflow for more control over native code with `expo eject`, and follow the prompts.

**Detailed Build Errors**
Open the `.xcworkspace` file in Xcode and run the app there for more detailed error logs.

> Always ensure your local environment matches the app's required versions for Node.js, npm, Expo CLI, and Xcode.

## Project Notes

### Wizard of Oz Items

1. **Connection Profiles** — Suggested based on proximity and shared course enrollment.
2. **Course List** — Ideally users could add their own enrolled courses; the app currently simulates this experience.
3. **Assignments** — Generally provided based on course enrollment.

### Hard-Coded Aspects

1. Names of the courses
2. Recommended connection profiles
3. User profile
4. List of readings
5. List of assignments

## Style Guide

- **Headings**: Georgia
- **Screen content**: Arial
- **Font sizes**: 50 for titles, 15–20 for other text

## Resources

1. [The Ultimate Guide to the Hamburger Menu and Its Alternatives](https://uxplanet.org/the-ultimate-guide-to-the-hamburger-menu-and-its-alternatives-e2da8dc7f1db)
2. [Custom Bottom Tab Navigator in React Native](https://www.youtube.com/watch?v=gPaBicMaib4)
3. [Authentication using Firebase](https://www.youtube.com/watch?v=ONAVmsGW6-M)
4. [Options for Building React Native Collapsible Accordions](https://blog.logrocket.com/building-react-native-collapsible-accordions/)
5. [React Navigation Guide](https://reactnavigation.org/docs)
6. [How to Build React Native Swipe Cards Inspired by Tinder](https://instamobile.io/react-native-controls/react-native-swipe-cards-tinder/)
7. [react-native-deck-swiper](https://www.npmjs.com/package/react-native-deck-swiper)
8. [Expo Audio](https://docs.expo.dev/versions/latest/sdk/audio/)
9. [React Native Voice](https://www.npmjs.com/package/@react-native-voice/voice?activeTab=readme)
10. [Expo Speech](https://docs.expo.dev/versions/latest/sdk/speech/)
