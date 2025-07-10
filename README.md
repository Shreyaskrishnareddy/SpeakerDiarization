# SpeakerDiarization

![Python](https://img.shields.io/badge/python-3.8+-blue.svg) ![License](https://img.shields.io/badge/license-MIT-blue.svg) ![Groq](https://img.shields.io/badge/Groq-1.0.0-blue.svg) ![Whisper](https://img.shields.io/badge/Whisper-1.0.0-blue.svg) ![Transformers](https://img.shields.io/badge/Transformers-4.21.3-blue.svg)

## 🚀 Overview

This project uses Python to automate speaker diarization by downloading audio from YouTube videos, transcribing the audio using Whisper, and generating a set of questions and answers based on the transcript using Groq's LLaMA model. The final output is converted to speech using the Google Text-to-Speech API.

## ✨ Key Features

* **Speaker Diarization**: Automates speaker diarization by downloading audio from YouTube videos, transcribing the audio, and generating questions and answers.
* **Whisper Integration**: Uses Whisper to transcribe audio files.
* **Groq Integration**: Uses Groq's LLaMA model to generate questions and answers from the transcript.
* **Google Text-to-Speech Integration**: Converts the final output to speech using the Google Text-to-Speech API.

## 🛠️ Technology Stack

### Core Technologies
* Python 3.8+
* Groq
* Whisper
* Transformers

### Dependencies
* `groq`
* `torch`
* `whisper`
* `gtts`
* `pydub`
* `pytube`
* `numpy`
* `torchaudio`
* `assemblyai`

## 🚀 Quick Start

### Prerequisites
* Python 3.8+
* `groq` API key

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/username/speakerdiarization.git
   cd speakerdiarization
   ```

2. **Set up environment**
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

4. **Configuration**
   * Create a `config.json` file with your `groq` API key
   ```json
   {
     "groq_api_key": "YOUR_GROQ_API_KEY"
   }
   ```

### Usage

* **Download audio from YouTube video**
   ```python
   download_audio_from_youtube("https://www.youtube.com/watch?v=yX5EJf4R77s", "audio.mp3")
   ```
* **Transcribe audio using Whisper**
   ```python
   transcribe_audio_with_whisper("audio.mp3")
   ```
* **Generate questions and answers using Groq's LLaMA model**
   ```python
   create_qa_from_text(transcript, model="llama3-70b-8192")
   ```
* **Convert questions and answers to speech using Google Text-to-Speech API**
   ```python
   convert_qa_to_speech(qa_text, "output.mp3")
   ```

## 📊 Project Structure

```bash
speakerdiarization/
config.json
requirements.txt
Speaker_Diarization.py
README.md
```

## 🔧 Development

### Running Tests
* **Note:** There are no tests in this project.

### Code Quality
* **Note:** There are no linting or formatting configuration files in this project.

## 🚀 Deployment

* **Note:** This project is not designed for deployment.

## 📖 API Documentation

* **Note:** There is no API documentation for this project.

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

* Groq
* Whisper
* Transformers