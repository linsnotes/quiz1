# Quiz App

A lightweight, client-side quiz application that loads questions from Google Sheets.

## Overview

Quiz App is a simple HTML/JavaScript application that allows teachers or quiz creators to create quizzes using Google Sheets and share them with students or participants. The app runs entirely in the browser with no server-side components, making it easy to host on GitHub Pages or any static hosting service.

![Quiz App Screenshot](screenshot.png)

## Features

- 📝 Supports multiple-choice and text-input questions
- 📚 Optional reading material for each question
- 💡 Hints for difficult questions
- ⏱️ Timer to track quiz duration
- 📊 Detailed results with score statistics
- 🔄 Review mode to see correct answers and explanations
- 📸 Screenshot functionality to save results
- 🏃‍♂️ Fast loading and responsive design

## How It Works

1. Quiz questions are stored in a Google Sheet
2. Users enter their name and the Quiz ID (Google Sheet ID)
3. The app loads questions directly from the Google Sheet
4. Users complete the quiz and receive immediate feedback
5. Results can be reviewed and saved as screenshots

## Setup Instructions

### Creating a Question Sheet

1. Create a new Google Sheet with the following columns:
   - `No` - Question number
   - `Question` - The question text
   - `Answer` - The correct answer
   - `Type` - Question type (MCQ or Text)
   - `MCQ Options` - Options for multiple-choice questions (separated by # symbol)
   - `Reading Material` - Optional background information
   - `Hint` - Optional hint for the question
   - `Explanation` - Explanation of the answer

2. Fill in your questions
3. Make sure the Google Sheet is publicly accessible (File > Share > Anyone with the link > Viewer)
4. Copy the Sheet ID from the URL (the long string between /d/ and /edit in the URL)

### Hosting the App

The app is a single HTML file that can be:
1. Hosted on GitHub Pages
2. Deployed to any static file hosting service
3. Run locally by opening the HTML file in a browser

## Usage

### For Quiz Creators

1. Create your question sheet in Google Sheets
2. Share the link to the Quiz App along with the Sheet ID
3. Students will enter the Sheet ID to access the quiz

### For Quiz Takers

1. Open the Quiz App link
2. Enter your name (used only for displaying on the result screen)
3. Enter the Quiz ID provided by your teacher
4. Complete the quiz and review your results

## Privacy

This application:
- Is purely client-side HTML/CSS/JavaScript
- Does not collect any personal data
- Does not store user answers or quiz results on any server
- The name entered is only used locally to display on the results screen
- No cookies are used except those required by GoatCounter for anonymous visit tracking

## Technical Details

The app uses:
- Vanilla JavaScript (no frameworks)
- SheetJS for parsing Excel files
- html2canvas for taking screenshots
- GoatCounter for anonymous visitor counting
- Responsive design that works on desktop and mobile devices

## License

MIT License

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.
