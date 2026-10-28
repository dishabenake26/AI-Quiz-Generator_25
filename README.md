# AI-Quiz-Generator_25
# 🧠 AI Quiz Generator 

**Turn your study material into an interactive learning challenge!**

AI Quiz Generator is a gaming-inspired desktop application built with Python and `pywebview`. It combines an attractive neon-themed interface with quiz creation, timed challenges, instant feedback, and performance tracking to make learning more engaging.

Users can practise with built-in offline questions, generate quizzes on different topics using AI, or create questions from their own study documents.

## ✨ Key Features

### 🎮 Interactive Quiz Experience

- Modern dark dashboard with a neon-inspired design.
- Customisable quiz challenges.
- Countdown timer for answering questions.
- Instant feedback after submitting answers.
- Final score, results, and answer review.
- Quiz history and learning progress tracking.

### 🤖 AI-Powered Quiz Generation

- Generate questions on user-selected topics using OpenAI's `gpt-4o-mini` model.
- Create personalised practice quizzes based on learning needs.
- Use AI-generated questions when a valid API key is configured.

### 📚 Study Material-Based Quizzes

- Upload study materials in **PDF, DOCX, and TXT** formats.
- Generate questions using the extracted document content.
- Apply strict source-only validation so accepted questions must contain supporting evidence from the uploaded material.
- Fail safely when AI is unavailable instead of silently replacing document-based questions with general-knowledge questions.

### 💻 Offline Learning

- Built-in sample question banks for Python, Physics, and Biology.
- Practise supported subjects without configuring an API key.
- Store quiz history locally in `data/history.json`.

## 🛠️ Technologies Used

| Technology                             | Purpose                                  |
| -------------------------------------- | ---------------------------------------- |
| Python                                 | Application logic and quiz functionality |
| pywebview                              | Desktop application window               |
| HTML, CSS and JavaScript               | User interface and interactions          |
| OpenAI API                             | AI-based question generation             |
| PDF, DOCX and TXT processing libraries | Reading uploaded study materials         |
| JSON                                   | Local quiz history storage               |

## ⚙️ Installation and Setup

### Prerequisites

- Windows 10 or Windows 11
- Python 3.11 or newer
- Internet connection for AI features and optional online fonts
- An OpenAI API key for AI-powered quiz generation

### Step 1: Open the Project

Extract the project folder, then open PowerShell or the VS Code terminal inside that folder.

### Step 2: Install Dependencies

Run the following command:

```powershell
py -m pip install -r requirements.txt
```

### Step 3: Configure the OpenAI API Key

AI-powered features require an API key. Set it in the current PowerShell session:

```powershell
$env:OPENAI_API_KEY="your_api_key_here"
```

Replace the example value with your actual key. **Never publish your API key in your source code or upload it to GitHub.**

### Step 4: Launch the Application

Run:

```powershell
py main.py
```

The application should open in its desktop window. Keep the terminal open while running it.

## 🚀 How to Use the Application

1. **Launch the dashboard:** Open the application to access its learning interface.
2. **Choose a quiz mode:** Select a supported offline subject, enter a topic for AI generation, or upload study material.
3. **Customise your challenge:** Configure the available quiz settings.
4. **Answer the questions:** Complete the challenge while managing the timer.
5. **Review your performance:** Check your score, feedback, correct answers, and previous quiz history.
6. **Track your progress:** Use the stored history to review your learning activity.

## 🔐 Important Notes

- Without an API key, the application provides its bundled offline question banks for Python, Physics, and Biology.
- AI-generated quizzes and strict study-material question generation require a working API configuration and internet access.
- In study-material mode, questions are checked against evidence extracted from the uploaded content. This validation helps enforce source-only generation but does not guarantee that every AI-generated question is perfectly accurate.
- Large documents may not be covered completely because the current implementation samples up to four overlapping sections. For more comprehensive results, split large documents into smaller chapters.
- The application stores quiz history locally in `data/history.json`.
- The first launch may require internet access to load Google Fonts. Fallback fonts are available if the online fonts cannot be loaded.

## 🎯 Project Objectives

- Make learning more interactive through a game-inspired interface.
- Reduce the effort required to create practice quizzes manually.
- Support both topic-based learning and document-based revision.
- Provide immediate feedback and performance summaries.
- Demonstrate the integration of Python, web technologies, AI APIs, and local data storage in a desktop application.

## 🔮 Future Enhancements

- Add more offline subjects and larger question banks.
- Introduce difficulty levels and additional question formats.
- Provide detailed analytics and subject-wise performance charts.
- Support chapter-wise quizzes and more comprehensive document coverage.
- Add export options for quiz questions and results.
- Package the application as a Windows executable for easier distribution.

## 👩‍💻 Project Information

**Project Name:** AI Quiz Generator&#x20;

**Project Type:** AI-powered desktop learning application

**Primary Language:** Python

**Interface:** HTML, CSS, JavaScript and pywebview

**AI Integration:** OpenAI API

---

*Learn smarter. Challenge yourself. Track your progress.*
