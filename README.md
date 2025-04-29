# Quiz App

A mobile quiz application built using React Native and Expo.

## Features

- Displays quiz questions sequentially.
- Provides multiple-choice answer options.
- Includes a timer for tracking time (likely per question or overall).
- Manages quiz state (e.g., current question, score) using a context provider.
- Uses custom components for a consistent UI (Cards, Buttons, etc.).

## Project Structure

```
.
├── assets/             # Static assets (images, fonts, animations)
├── src/                # Source code
│   ├── app/            # Main application screens (e.g., QuizScreen)
│   ├── components/     # Reusable UI components
│   ├── hooks/          # Custom React hooks (e.g., useTimer)
│   ├── providers/      # Context providers (e.g., QuizProvider)
│   ├── questions.ts    # Quiz questions data
│   └── types.ts        # TypeScript type definitions
├── .gitignore
├── app.json            # Expo configuration
├── App.tsx             # Root application component
├── babel.config.js     # Babel configuration
├── package.json        # Project dependencies and scripts
├── tsconfig.json       # TypeScript configuration
└── ...                 # Other configuration files
```

## Key Components

- **`QuizScreen.tsx`**: The main screen where the quiz gameplay happens.
- **`QuestionCard.tsx`**: Displays the current question text.
- **`AnswerOption.tsx`**: Represents a single clickable answer choice.
- **`CustomButton.tsx`**: A reusable button component.
- **`Card.tsx`**: A generic card component used for layout.
- **`QuizProvider.tsx`**: Manages the global state for the quiz (e.g., score, current question index).
- **`useTimer.ts`**: A custom hook to handle timer logic.

## Getting Started

### Prerequisites

- Node.js (LTS version recommended)
- Expo CLI: `npm install -g expo-cli`
- Watchman (for macOS users): `brew install watchman`
- Git

### Installation

1.  Clone the repository:
    ```bash
    git clone <your-repository-url>
    cd <your-project-directory>
    ```
2.  Install dependencies:
    ```bash
    npm install
    # or
    yarn install
    ```

### Running the App

1.  Start the Metro Bundler and development server:
    ```bash
    npx expo start
    ```
2.  Scan the QR code with the Expo Go app (available on iOS and Android) on your physical device, or run on an emulator/simulator:
    - Press `a` to run on an Android emulator/device.
    - Press `i` to run on an iOS simulator/device.
    - Press `w` to run in the web browser (if configured).

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1.  Fork the Project
2.  Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3.  Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4.  Push to the Branch (`git push origin feature/AmazingFeature`)
5.  Open a Pull Request

## License

Distributed under the MIT License. See `LICENSE` file for more information (if you add one).
