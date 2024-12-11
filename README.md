# Flashcard App with Tkinter

This is a simple Flashcard application built using Python's Tkinter library and the Gemini API to generate flashcards based on a given topic. Users can add custom flashcards, review them, delete individual flashcards or all flashcards, and generate new flashcards automatically with the help of the Gemini API.

## Features

- **Add Flashcards**: Users can create their own flashcards by entering a question and answer.
- **Review Flashcards**: Users can go through their flashcards, one by one, and view the answers.
- **Generate Flashcards with Gemini**: Users can generate flashcards automatically on any topic, specifying the number of flashcards they want.
- **Delete Flashcards**: Flashcards can be deleted individually or all at once.
- **Persistent Storage**: Flashcards are stored in a `flashcards.json` file, ensuring data is saved even when the app is closed.

## Requirements

- Python 3.x
- Tkinter (for GUI)
- google-generativeai library (for generating flashcards via Gemini API)

You can install the required library using pip:

```bash
pip install google-generativeai
```

## Setup

1. Clone the repository:

```bash
git clone https://github.com/yourusername/flashcard-app.git
cd flashcard-app
```

2. Replace the `API_KEY` in the code with your own Gemini API key.

```python
API_KEY = "YOUR_GEMINI_API_KEY"
```

3. Run the application:

```bash
python flashcard_app.py
```

## Screens

- **Main Menu**: The entry point to the app with options to Add Flashcard, Review Flashcards, Generate Flashcards, or Exit.
- **Add Flashcard**: A screen where users can input their question and answer, and save it.
- **Review Flashcards**: Allows users to review saved flashcards, show the answer, and navigate through them.
- **Generate Flashcards**: Users can specify a topic and the number of flashcards they want to generate using Gemini.

## Usage

1. **Add Flashcard**: 
   - Enter a question and answer, and click "Save" to store it.
   
2. **Review Flashcards**: 
   - Click "Show Answer" to view the answer for the current flashcard.
   - Navigate through the flashcards using "Next Flashcard".
   - Delete individual flashcards or all flashcards with the corresponding buttons.

3. **Generate Flashcards**: 
   - Enter a topic and the number of flashcards you'd like to generate.
   - The app will use the Gemini API to generate the flashcards, which are then added to your collection.

4. **Delete Flashcards**: 
   - You can delete flashcards individually or clear all saved flashcards.


## Contributing

Feel free to fork this project, make improvements, or open issues for any bugs or features you want to see.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

### Note:

Make sure to replace the Gemini API key with your personal key to use the AI functionality. If you don’t have an API key, visit the official [Gemini API documentation](https://developers.google.com/generative-ai) to get one.
