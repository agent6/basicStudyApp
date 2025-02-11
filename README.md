# Basic Study App

Welcome to the Basic Study App! This application is designed to help users prepare for exams by simulating test environments, practicing with ad-hoc questions, and tracking performance over time.

## Getting Started

To get started with the Basic Study App, follow these steps:

1. **Download the Application Files**:
   - Clone or download the repository from GitHub: [https://github.com/agent6/basicStudyApp](https://github.com/agent6/basicStudyApp)

2. **Create Your Question Bank**:
   - The application uses a `questions.json` file to load questions. You can create your own question bank by writing your questions in JSON format. See the [JSON Schema](#json-schema-for-questions) section below for guidance.

3. **Run the Application**:
   - Open the `index.html` file in your preferred web browser to start using the app.

## Features

The Basic Study App offers three main features:

1. **Simulate Exam**:
   - This mode allows you to take a full-length exam simulation. The app will randomly select questions from your question bank, and you'll have a set amount of time to complete the exam.

2. **Adhoc Questions**:
   - Practice individual questions in a non-exam setting. This mode is ideal for quick study sessions and allows you to focus on specific topics.

3. **Performance Tracker**:
   - Track your performance over time. The app records your attempts and scores for each topic, helping you identify areas that need improvement. *Note: This information will reset if you reload the page.*

## JSON Schema for Questions

To create your own question bank, structure your `questions.json` file according to the following schema:

```json
[
  {
    "questionText": "What is the capital of France?",
    "miniLesson": "Paris is the capital and most populous city of France.",
    "topicSection": "Geography",
    "topicSubsection": "Europe",
    "topicTertiary": "Capital Cities",
    "options": [
      {
        "optionText": "Paris",
        "isCorrect": true
      },
      {
        "optionText": "London",
        "isCorrect": false
      },
      {
        "optionText": "Berlin",
        "isCorrect": false
      },
      {
        "optionText": "Madrid",
        "isCorrect": false
      }
    ]
  }
]
```
Field Descriptions:

questionText (string): The text of the question.
miniLesson (string): A brief explanation or lesson related to the question.
topicSection (string): The main category of the question.
topicSubsection (string): A subcategory under the main category.
topicTertiary (string): A further division under the subcategory.
options (array): A list of possible answers, each containing:
optionText (string): The text of the option.
isCorrect (boolean): Indicates whether this option is the correct answer.
By following this schema, you can customize the app with your own questions tailored to your study needs.

Testing the Application
You can test the application with a sample question bank by visiting: https://agent6.github.io/basicStudyApp/

This sample includes 16 CCNP ENCOR questions to demonstrate how the app functions.

Happy studying!
