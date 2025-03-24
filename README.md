# Vocabulary Builder Flutter App

A simple Flutter application that allows users to add both words and idioms to a vocabulary API. This app communicates with your backend NestJS API endpoints.

## Features

- User authentication (login)
- Add new words to your vocabulary
- Add idioms to your vocabulary
- Tabbed interface to separate words and idioms
- Feedback on successful and failed operations
- Token-based authentication with your API

## Setup Instructions

### Prerequisites

- Flutter SDK (3.0.0 or higher)
- Dart SDK (3.0.0 or higher)
- Working backend API running at http://localhost:3030/api (adjust the URL in the code if needed)

### Installation

1. Clone this repository
2. Navigate to the project directory
3. Install dependencies:

```bash
flutter pub get
```

4. Run the app:

```bash
flutter run
```

### API Configuration

By default, the app is configured to connect to your API at:

- http://localhost:3030/api/auth/login (for authentication)
- http://localhost:3030/api/word (for adding words)
- http://localhost:3030/api/word/idiom (for adding idioms)

If your API is running on a different address or port, you need to modify the URL in the code.

## Usage

1. Launch the app
2. Log in with your credentials
3. Use the tabs to navigate between Words and Idioms
4. Enter a word or idiom and press the corresponding add button
5. You'll receive feedback on whether the operation was successful

## API Endpoints

The app communicates with the following endpoints:

- **POST /auth/login**: Authenticate user and get token
- **POST /word**: Add a new word
- **POST /word/idiom**: Add a new idiom

## Dependencies

- http: For making API requests
- shared_preferences: For storing the authentication token
