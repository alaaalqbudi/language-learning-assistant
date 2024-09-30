# language-learning-assistant
objectv:Develope an interactive language learning tool that convert text to audio 
Helping users hear the correct pronounciation to improve their listining language
code: Library Imports:
gradio: This library is used to create a user interface (UI) for your text-to-speech (TTS) application.
pydub: This library helps you manipulate audio files in Python. It's used for converting MP3 to WAV format in this case.
gtts: This library (Google Text-to-Speech) is the core TTS engine. It interacts with Google's TTS API to convert text to speech in various languages.
subprocess (not explicitly used in the provided code): This library could potentially be used for running external programs like FFmpeg (mentioned in the imports but not utilized in the current code).
text_to_speech Function:
This function takes three arguments:
text: The text string to be converted to speech.
language: The language code (e.g., "en" for English, "ar" for Arabic)
speed: A float value between 0.5 and 2.0 representing the speaking speed (0.5 being slower, 2.0 being faster)
If the text is empty, it returns a message prompting the user to enter some text.
 Text-to-Speech Conversion:
Creates a gTTS object using the provided text, language, and speed.
Saves the generated audio as an MP3 file named "temp_audio.mp3".
4. Audio Format Conversion (Optional)

