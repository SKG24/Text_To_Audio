# Sentence-to-Audio Conversion Script

This repository provides a Python script to convert a list of sentences into individual MP4 audio files optimized for low data usage. The script uses the **gTTS** library for text-to-speech conversion and **pydub** for audio processing.

---

## Features
- Converts multiple sentences into individual MP4 audio files.
- Optimized for low data usage by reducing the bitrate to 32 kbps.
- Automatically handles temporary files.

---

## Libraries Used

### 1. [gTTS](https://pypi.org/project/gTTS/)
- **Purpose**: Converts text into speech audio files.
- **Installation**: 
  ```bash
  pip install gtts
  ```

### 2. [pydub](https://pypi.org/project/pydub/)
- **Purpose**: Handles audio processing, including exporting audio in different formats and bitrates.
- **Installation**: 
  ```bash
  pip install pydub
  ```
- **Note**: `pydub` requires **ffmpeg** for audio processing.
  - **Linux**: `sudo apt install ffmpeg`
  - **MacOS**: `brew install ffmpeg`
  - **Windows**: Download from [ffmpeg.org](https://ffmpeg.org) and add it to your PATH.

---

## How to Use

### 1. Clone the Repository
```bash
git clone https://github.com/your-username/sentence-to-audio.git
cd sentence-to-audio
```

### 2. Prepare Your Input
Edit the Python script to include the sentences you want to convert. Replace the example `sentences` list with your own sentences:
```python
sentences = [
    "Your first sentence.",
    "Your second sentence.",
    "More sentences here."
]
```

### 3. Run the Script
Run the Python script to generate the audio files:
```bash
python sentences_to_audio.py
```

### 4. Output
The audio files will be saved in the specified `output_audio` directory as MP4 files.

---

## Example
Given the input:
```python
sentences = [
    "This is the first sentence.",
    "Here is another example sentence.",
    "This script converts text to audio efficiently."
]
```
The output will include the files:
- `sentence_1.mp4`
- `sentence_2.mp4`
- `sentence_3.mp4`

---
