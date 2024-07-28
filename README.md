# Grabbie Hackathon

## Feature Description

Grabbie is an application that leverages Generative AI to enhance user experience by promoting local businesses, providing personalized recommendations, easing transportation, and evolving through user feedback. The main features include a list of places by category, personalized recommendations via an LLM-powered prompt engine, and a 'Grab Pioneers' feature that allows users to add new places with verification, rewarding them for verified contributions.

## Project Structure

The project is divided into two main parts:
- Backend
- Frontend

## Backend

The backend is developed using:
1. **Python 3.11**: The Python version used to develop the backend server.
2. **FastAPI**: A framework used to create fast and efficient APIs.
3. **gpt4-o**: The Generative AI model used for recommendations and other smart features.
4. **NGROK**: Used as a gateway to expose the port to the internet, facilitating development and testing.
5. **Clean Code Architecture**: An architectural approach used to keep the code clean, organized, and maintainable.

### Running the Backend

1. Clone this repository:
    ```sh
    https://github.com/ichsansaid/grabbie-hackathon.git
    cd grabbie-hackathon/backend
    ```
2. Create and activate a virtual environment:
    ```sh
    python -m venv venv
    source venv/bin/activate   # for Unix-based OS
    .\venv\Scripts\activate    # for Windows OS
    ```
3. Install dependencies:
    ```sh
    pip install -r requirements.txt
    ```
4. Run the server:
    ```sh
    fastapi run main.py
    ```

## Frontend

The frontend is developed using:
1. **Dart**: The programming language used to develop the frontend application.
2. **Flutter**: The UI framework used to create an interactive and responsive frontend application.

### Running the Frontend

1. Clone this repository:
    ```sh
    https://github.com/ichsansaid/grabbie-hackathon.git
    cd grabbie-hackathon/frontend
    ```
2. Install dependencies:
    ```sh
    flutter pub get
    ```
3. Run the application:
    ```sh
    flutter run
    ```

## Directory Structure

```plaintext
.
├── backend
│   ├── domain
│   │   ├── contracts
│   │   ├── dao
│   │   ├── dto
│   │   └── usecases
│   ├── infra
│   │   ├── fastapi
│   │   ├── openai
│   │   └── usecases
│   └── requirements.txt
└── frontend
    ├── lib
    ├── pubspec.yaml
    └── test
