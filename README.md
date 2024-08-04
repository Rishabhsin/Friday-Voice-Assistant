# Friday Voice Assistant

Friday is a voice-activated assistant designed to perform specific tasks based on voice commands. It can open websites and play music from a predefined list.

## Features

- Voice recognition using `speech_recognition`.
- Text-to-speech conversion using `gtts` (Google Text-to-Speech) and `pyttsx3`.
- Opens websites in the default web browser.
- Plays music from a predefined list of YouTube links.

## Installation

1. Clone the repository:
    ```sh
    git clone https://github.com/RISHABHSINGH3006/Friday-Voice-Assistant.git
    cd Friday-Voice-Assistant
    ```

2. Install the required Python packages:
    ```sh
    pip install speechrecognition pyttsx3 gtts pygame pocketsphinx
    ```

## Usage

1. Run the main script:
    ```sh
    python main.py
    ```

2. Use the wake word "Friday" followed by a command. Example commands include:
    - "Open Google" to open https://google.com
    - "Open Facebook" to open https://facebook.com
    - "Play stealth" to play a specific song from the predefined list

## Files

### main.py

This is the main script that runs the Friday assistant. It includes the following key functions:

- `speak(text)`: Converts text to speech using `gTTS` and plays it using `pygame`.
- `processCommand(c)`: Processes voice commands to open specific websites or play music from the `musicLibrary`.

### musicLibrary.py

This script contains a dictionary of music links:

```python
music = {
    "stealth": "https://www.youtube.com/watch?v=jHpQERs3ktc&list=PLEX0_dFX2_BakyTEXosZrSxrMRC21lRVH&index=3",
    "march": "https://www.youtube.com/watch?v=CRHsb0usNV4&list=PLEX0_dFX2_BakyTEXosZrSxrMRC21lRVH&index=2",
    "skyfall": "https://www.youtube.com/watch?v=d7eZsOADCos&list=PLEX0_dFX2_BbkQ4tR5x8CKHsn8xfyVoK6&index=2",
    "wolf": "https://www.youtube.com/watch?v=2lLwaDK7mEs"
}
```

## Requirements

- Python 3.x
- `speechrecognition`
- `pyttsx3`
- `gtts`
- `pygame`
- `pocketsphinx`
