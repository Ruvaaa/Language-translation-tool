import googletrans
from googletrans import Translator

# Create translator instance
translator = Translator()

# Language mapping dictionary
language_mapping = {name.lower(): code for code, name in googletrans.LANGUAGES.items()}

print("Available languages:")
for name in googletrans.LANGUAGES.values():
    print("-", name.title())

def translate_text(text, target_language):
    translated = translator.translate(text, dest=target_language)
    return translated.text

while True:
    # User Input
    text1 = input("\nEnter a sentence to translate (or type 'exit' to quit): ")
    if text1.lower() == "exit":
        break

    target_language_name = input("Enter a target language (e.g., 'French', 'Spanish'): ").lower()

    target_language_code = language_mapping.get(target_language_name)

    if not target_language_code:
        print("Invalid language name. Please try again.")
        continue  # Ask for input again instead of proceeding

    translated_text = translate_text(text1, target_language_code)
    print("\nOriginal text: " + text1)
    print("Translated text: " + translated_text)

    # Detect language
    detected_lang = translator.detect(text1)
    detected_language_name = googletrans.LANGUAGES.get(detected_lang.lang, "Unknown Language")
    confidence = detected_lang.confidence if detected_lang.confidence is not None else "N/A"
    print(f"Detected language: {detected_language_name} (Confidence: {confidence})")
