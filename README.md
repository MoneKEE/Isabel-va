# Isabel - Virtual Assistant

Isabel is a virtual assistant designed to interpret, listen, and respond to voice commands. It leverages several Python modules to perform speech recognition, text-to-speech, and linguistic tagging.

## Features

- **Interpret**: Analyzes and tags phrases to understand their meaning.
- **Listen**: Records and converts voice data to text.
- **Speak**: Converts text responses into speech.

## Requirements

Ensure you have the following Python modules installed:

- speech
- sound
- dialogs
- linguistictagger
- sqlite3
- csv
- sys

You can install these modules using pip:
```bash
pip install pyobjc-core pyobjc-framework-Speech
```

## Usage

### Running the Script

1. **Install Dependencies**:
   Ensure all required Python modules are installed.

2. **Run the Script**:
   Execute the script using Python:
   ```bash
   python Isabel.py
   ```

### Functionality

- **Interpret**:
  Tags each term in a phrase with its corresponding part of speech and uses this information to simplify response selection.

- **Listen**:
  Records voice data and converts it to text using the `speech` and `sound` modules.

- **Speak**:
  Converts text responses into speech and voices them using the `speech` module.

### Main Functions

- `interpret(text)`: Handles the logic for interpreting various types of questions and statements.
- `listen()`: Records and transcribes audio input.
- `speak(text)`: Converts text to speech.
- `tagtext(text)`: Tags text with linguistic information.
- `cleantext(text)`: Cleans and normalizes text input.
- `main()`: The main function that initiates the virtual assistant and handles the database operations.

## Database

Isabel uses `sqlite3` to store and manage phrases and their linguistic tags. The database file `isabel.db` is created and managed within the script.

## Example

To start using Isabel, run the script and follow the prompts. Speak or type commands and Isabel will interpret, respond, and manage the conversation.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

For more information, refer to the [source code](https://github.com/MoneKEE/Python-Code-Samples/blob/master/Isabel.py).
