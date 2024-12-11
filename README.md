Here’s a **README.md** for your Flashcard App:

---

# Flashcard App

A simple and interactive Flashcard App built with **PyQt5** for managing, reviewing, and generating flashcards. The app allows you to manually add flashcards, review them, delete individual or all flashcards, and even generate flashcards automatically using the **Gemini API**.

---

## Features

- **Add Flashcards**: Create custom flashcards with a question and answer.
- **Review Flashcards**: Randomly review flashcards, with options to:
  - Show the answer.
  - Delete the current flashcard.
- **Generate Flashcards**: Automatically generate flashcards using the Gemini API by providing a topic and the number of flashcards.
- **Delete All Flashcards**: Clear all saved flashcards with a single click (confirmation required).
- **Data Persistence**: Flashcards are saved locally in a JSON file (`flashcards.json`) for later use.

---

## Requirements

### Python Version
- Python 3.7 or later

### Dependencies
Install the required libraries using `pip`:
```bash
pip install PyQt5 google-generativeai
```

---

## Installation

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/your-username/flashcard-app.git
   cd flashcard-app
   ```

2. **Install Dependencies**:
   ```bash
   pip install -r requirements.txt
   ```

3. **Set up the Gemini API**:
   - Replace the placeholder `API_KEY` in the code with your **Gemini API Key**.

4. **Run the App**:
   ```bash
   python flashcard_app.py
   ```

---

## Usage

### Main Menu
- **Add Flashcard**: Opens a dialog to enter a question and its corresponding answer.
- **Review Flashcards**: Starts a random review session of all flashcards.
- **Generate Flashcards**: Enter a topic and number of flashcards to generate flashcards automatically using the Gemini API.
- **Delete All Flashcards**: Deletes all saved flashcards after confirmation.
- **Exit**: Closes the application.

### Flashcard Review
- Displays a flashcard question with options to:
  - **Show Answer**: Reveals the answer to the current question.
  - **Delete Flashcard**: Deletes the current flashcard.
  - **Skip**: Moves to the next flashcard without revealing the answer.

---

## File Structure

```
flashcard_app.py       # Main application code
flashcards.json        # File for storing flashcards (auto-generated)
README.md              # Documentation for the app
requirements.txt       # List of dependencies
```

---

## How to Use the Gemini API

1. **Obtain an API Key**:
   - Visit the [Google Gemini API Console](https://developers.google.com) and generate an API key.

2. **Configure the API in Code**:
   - Replace the `API_KEY` variable in the `flashcard_app.py` file with your API key:
     ```python
     API_KEY = "your-api-key-here"
     ```

3. **Generate Flashcards**:
   - Use the "Generate Flashcards" feature to create flashcards on your desired topic.

---

## Screenshots (Optional)
You can add screenshots here to visually explain the app functionality.

---

## Troubleshooting

1. **Missing Dependencies**:
   - Ensure all required libraries are installed:

2. **Gemini API Issues**:
   - Check your API key and ensure it has the necessary permissions.

3. **App Crashes**:
   - Make sure the `flashcards.json` file is present and not corrupted. If missing, the app will create a new one.

---

## Contributing

1. Fork the repository.
2. Create a new feature branch:
3. Commit your changes and push to your forked repository.
4. Create a pull request.

---

## License

This project is licensed under the MIT License. See the `LICENSE` file for details.

---

## Author

Developed by **Aledare John **.  
Feel free to reach out for questions or suggestions!  

---

Let me know if you'd like help tweaking or customizing this further!
