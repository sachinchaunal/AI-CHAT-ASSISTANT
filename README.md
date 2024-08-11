# AI Chat Assistant

This project is an AI Chat Assistant that uses speech recognition to take user input and respond with voice output. The assistant is designed to recognize specific commands and respond accordingly using natural language processing.

## Features

- **Speech Recognition**: The assistant listens to user input via a microphone and processes the spoken words.
- **Voice Output**: The assistant responds verbally using text-to-speech capabilities.
- **Command Recognition**: The assistant recognizes specific commands, such as greetings or asking for the time, and provides appropriate responses.

## Requirements

To run this project, you'll need to have the following Python libraries installed:

- `pyttsx3`: For text-to-speech conversion.
- `speech_recognition`: For speech input and recognition.
- `sklearn`: For machine learning processes.
- `nltk`: For natural language processing and text handling.

You can install all the required packages using `pip`:

```bash
pip install pyttsx3 speechrecognition scikit-learn nltk
```

## Cloning the Repository

To get started with this project, first clone the repository from GitHub:

```bash
git clone https://github.com/sachinchaunal/AI-CHAT-ASSISTANT.git
cd AI-CHAT-ASSISTANT
```

## Configuration

Before running the project, ensure that your microphone is properly configured and connected.

### NLTK Data

The project requires specific NLTK data. You may need to download the necessary data files. Uncomment and run the following code once:

```python
import nltk
nltk.download("punkt")
```

### Text-to-Speech Voice Configuration

The project uses a specific voice for text-to-speech (TTS). You may need to modify the `voice` ID in the `speak()` function to match the voices available on your system. The current configuration is set to use the Microsoft David Desktop voice.

## Running the Project

To start the AI Chat Assistant, run the main Python script:

```bash
python AI-CHAT-ASSISTANT.py
```

The assistant will listen for your voice commands and respond accordingly. You can test it by saying phrases like "hello" or "what's the time?"

## Notes

- Make sure your environment supports the required TTS and speech recognition features.
- The project is set up to ignore warnings for a smoother user experience.
- The current configuration uses a pause threshold of 1 second for speech recognition. Adjust this in the `speechrecognition()` function if necessary.

## License

This project is licensed under the MIT License.

---
