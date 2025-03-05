Language Translation Tool

This is a simple command-line language translation tool built with Python using the googletrans library. It allows users to input a sentence, specify a target language, and receive a translated version of the text. The tool also detects the language of the input text and provides a confidence score for the detection.

Features

Translates text from one language to another

Supports multiple languages

Detects the language of the input text with a confidence score

Provides a user-friendly interface with a list of available languages

Prerequisites

Make sure you have Python installed (preferably Python 3.x). You also need to install the googletrans library.

Installation

Clone this repository or download the script.

Install the required dependencies:

pip install googletrans==4.0.0-rc1

Usage

Run the script:

python translator.py

Follow the on-screen instructions:

Enter the text you want to translate.

Specify the target language by its name (e.g., French, Spanish, German).

The program will return the translated text and detect the language of the input.

Type exit to quit the program.

Example

Available languages:
- Afrikaans
- Albanian
- Arabic
...

Enter a sentence to translate (or type 'exit' to quit): Hello, how are you?
Enter a target language (e.g., 'French', 'Spanish'): French

Original text: Hello, how are you?
Translated text: Bonjour, comment allez-vous?
Detected language: English (Confidence: 0.99)

Notes

The script relies on googletrans, which uses Google Translate's API. If the API service is temporarily unavailable, you may experience issues.

Ensure your internet connection is active while using this tool.

Contributing

Feel free to fork this repository and submit pull requests to improve functionality or fix issues.

License

This project is open-source and available under the MIT License.
