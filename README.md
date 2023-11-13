# ChatGPT Voice Interaction Script

This script enables voice interaction with OpenAI's ChatGPT. It records audio from the user, transcribes it using OpenAI's Whisper model, sends the transcription to ChatGPT for processing, and then uses a text-to-speech model to vocalize the response.

## Features

- Voice recording for user input.
- Transcription of voice input using OpenAI's Whisper model.
- Interaction with ChatGPT for conversation.
- Vocalization of ChatGPT's response using text-to-speech.
- Custom playback of audio using FFmpeg.

## Prerequisites

- Python 3.8+
- OpenAI API Key (set as an environment variable `OPENAI_API_KEY` or in a `.env` file)
- FFmpeg installed and available in the system PATH.
- Python libraries: `sounddevice`, `soundfile`, `numpy`, `pathlib`, `openai`, `os`, `requests`, `re`, `colorama`, `pydub`.

## Installation

1. Clone the repository or download the script to your local machine.
2. Install the required Python libraries by running `pip install -r requirements.txt` (you will need to create this requirements file based on the imports).
3. Make sure FFmpeg is installed and properly set in your system's PATH.
4. Place your OpenAI API key in a `.env` file in the same directory as the script or export it as an environment variable `OPENAI_API_KEY`.

## Usage

Run the script using the following command:

```shell
python snippets.py
```

The script will start recording audio for the specified duration when prompted. Speak into your microphone after the "Recording..." prompt. The script will process your input and respond aloud.

## Configuration

To adjust recording settings, text-to-speech voices, or other features, modify the corresponding variables and function parameters within the script.

## Troubleshooting

If you encounter permission issues or errors related to audio file paths, ensure that the paths are correct and that your user account has the necessary permissions to read from and write to the specified directories.

## Contributing

Contributions to this project are welcome. 

## License

This project is under the MIT License.

## Acknowledgements

Thanks to the OpenAI team for providing the GPT and Whisper models used in this script.