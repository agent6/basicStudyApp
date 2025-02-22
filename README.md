# Basic Study App

A simple, standalone study application that helps you test your knowledge using a custom question bank. This project is perfect for exam simulation, adhoc practice, and performance tracking, all loaded from a local JSON file.

## Features

- **Simulate Exam:** Run a full exam simulation with a randomized selection of questions.
- **Adhoc Questions:** Practice individual questions on the fly.
- **Performance Tracker:** See your performance across different topics (please note, this data resets on page reload).

## Live Demo

Test out the app live at:  
[https://agent6.github.io/basicStudyApp/](https://agent6.github.io/basicStudyApp/)

If you want see where I took this basic code and made it a full webapp where there are multiple exams to choose from and where you can build out your own private questions as you study take a look at:

[https://myexam-prep.com](https://myexam-prep.com)

## Getting Started

To use this project, simply download or clone the repository. The project consists of two primary files:

- **index.html:** The main application file.
- **questions.json:** A sample question bank containing CCNP ENCOR sample questions.

### How to Download

Clone the repository using Git:

```bash
git clone https://github.com/agent6/basicStudyApp.git
```

Or download the ZIP archive directly from GitHub and extract it.

### Running the App

1. Ensure that both `index.html` and `questions.json` are in the same directory.
2. Open the `index.html` file in your web browser.
3. The app will load the questions from `questions.json` automatically.
4. Navigate through the three main screens:
   - **Simulate Exam**
   - **Adhoc Questions**
   - **Performance Tracker**

## Creating Your Own Question Bank

You can customize the app by modifying the `questions.json` file to create your own question bank. The file should contain an array of question objects that follow the schema outlined below.

### JSON Schema for Questions

Each question object should have the following structure:

```json
[
  {
    "questionText": "What is the purpose of OSPF in a network?",
    "miniLesson": "OSPF (Open Shortest Path First) is a routing protocol used to determine the best path for data.",
    "topicSection": "Routing",
    "topicSubsection": "OSPF",
    "topicTertiary": "Basics",
    "options": [
      {
        "optionText": "To exchange routing information between routers",
        "isCorrect": true
      },
      {
        "optionText": "To manage network security",
        "isCorrect": false
      }
    ]
  }
]
```

**Field Descriptions:**

- **questionText:** The text of the question.
- **miniLesson:** A brief explanation or lesson that is displayed if the answer is incorrect.
- **topicSection:** The main category (e.g., Routing, Switching).
- **topicSubsection:** A more specific sub-category.
- **topicTertiary:** A further subdivision for detailed topics.
- **options:** An array of answer options. Each option object includes (min 2 max 6 options):
  - **optionText:** The text for the answer option.
  - **isCorrect:** A boolean indicating if the option is correct.

## Sample Questions

The included `questions.json` file contains sample CCNP ENCOR questions to demonstrate how the app works. Use these as a reference when building your own question bank.

---

Happy studying!

