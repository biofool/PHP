# PHP — React Native App

A React Native mobile application scaffolded from the standard React Native template. The project includes a Vagrant configuration for development environment provisioning.

## Overview

This is a React Native app built with the default template (`react-native init`). The `App.js` renders the standard React Native welcome screen with sections for getting started, debugging instructions, and learn-more links. The project is configured for both Android and iOS development.

## Prerequisites

- Node.js (v14+)
- npm or yarn
- React Native CLI (`npx react-native`)
- Android Studio (for Android) or Xcode (for iOS)
- Vagrant and VirtualBox (optional, for the Vagrant-based dev environment)

## Setup

1. Clone the repository:
   ```bash
   git clone https://github.com/biofool/PHP.git
   cd PHP
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. (Optional) Start the Vagrant development VM:
   ```bash
   vagrant up
   ```

## How to Run

### Metro bundler
```bash
npm start
```

### Android
```bash
npm run android
```

### iOS
```bash
npm run ios
```

### Tests
```bash
npm test
```

### Lint
```bash
npm run lint
```

## Project Structure

```
PHP/
├── App.js                 # Main React Native component (default template)
├── index.js               # App entry point, registers App component
├── app.json               # App display name configuration
├── package.json           # Dependencies and scripts
├── babel.config.js        # Babel configuration (metro-react-native preset)
├── metro.config.js        # Metro bundler configuration
├── .flowconfig            # Flow type checker configuration
├── .eslintrc.js           # ESLint configuration
├── .prettierrc.js         # Prettier code formatting config
├── Vagrantfile            # Vagrant VM config (Ubuntu 21.10)
├── __tests__/             # Jest test suite
│   └── App-test.js        # Snapshot test for App component
└── package-lock.json      # Locked dependency versions
```

## Key Features

- React Native 0.66.4 with React 17.0.2
- Default template with dark mode support (`useColorScheme`)
- Jest testing configured with snapshot test
- ESLint and Prettier configured for code quality
- Vagrant development environment (Ubuntu 21.10)
