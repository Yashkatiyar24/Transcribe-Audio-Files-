# 🎵 Audio Transcription with OpenAI Whisper

<div align="center">

![Python](https://img.shields.io/badge/python-v3.7+-blue.svg)
![Whisper](https://img.shields.io/badge/OpenAI-Whisper-green.svg)
![License](https://img.shields.io/badge/license-MIT-blue.svg)

A powerful and easy-to-use audio transcription tool that converts speech to text using OpenAI's Whisper model.

</div>

## 📋 Table of Contents

- [Overview](#-overview)
- [Features](#-features)
- [Installation](#-installation)
- [Usage](#-usage)
- [Supported Formats](#-supported-formats)
- [Project Structure](#-project-structure)
- [Examples](#-examples)
- [Contributing](#-contributing)
- [License](#-license)

## 🎯 Overview

This project provides a simple yet powerful solution for transcribing audio files to text using OpenAI's state-of-the-art Whisper automatic speech recognition (ASR) system. Whether you have podcasts, music, voice recordings, or any other audio content, this tool can convert it to accurate text transcriptions.

## ✨ Features

- 🎙️ **High-Quality Transcription**: Leverages OpenAI Whisper for accurate speech-to-text conversion
- 🎵 **Multiple Format Support**: Works with various audio formats (WAV, MP3, etc.)
- 📝 **Text File Output**: Automatically saves transcriptions to organized text files
- 🔄 **Batch Processing**: Process multiple audio files in sequence
- 🚀 **Easy Setup**: Simple Jupyter notebook interface for quick start
- 🎯 **Flexible Model Selection**: Uses Whisper's base model for optimal speed/accuracy balance

## 🚀 Installation

### Prerequisites

- Python 3.7 or higher
- pip package manager

### Setup

1. **Clone the repository**
   ```bash
   git clone <repository-url>
   cd Transcribe-Audio-Files--main
   ```

2. **Install OpenAI Whisper**
   ```bash
   pip install openai-whisper
   ```

3. **Launch Jupyter Notebook**
   ```bash
   jupyter notebook "Transcribe Audio Files .ipynb"
   ```

## 💻 Usage

### Quick Start

1. Open the `Transcribe Audio Files .ipynb` notebook
2. Run the installation cell to install Whisper
3. Place your audio files in the project directory
4. Execute the transcription cells for your desired audio files
5. Find your transcriptions in the generated `.txt` files

### Code Example

```python
import whisper

# Load the Whisper model
model = whisper.load_model("base")

# Transcribe an audio file
result = model.transcribe("your_audio_file.wav")

# Save transcription to text file
with open("transcription.txt", "w") as f:
    f.write(result["text"])
```

## 🎧 Supported Formats

- **Audio Formats**: WAV, MP3, M4A, FLAC, and more
- **Languages**: Supports 99 languages (automatic detection)
- **Quality**: Handles various audio qualities and background noise levels

## 📁 Project Structure

```
Transcribe-Audio-Files--main/
├── 📓 Transcribe Audio Files .ipynb    # Main Jupyter notebook
├── 🎵 harvard.wav                      # Sample audio file
├── 🎵 Attention-(Mr-Jat.in).mp3       # Sample music file
├── 🎵 Ghane Gande - PagalNew.mp3      # Sample music file
├── 📄 transcription.txt                # Harvard audio transcription
├── 📄 transcription_song.txt           # Attention song transcription
├── 📄 transcriptions_har_.txt          # Ghane Gande transcription
└── 📖 README.md                        # This file
```

## 🔄 Examples

### Example 1: Speech Transcription
**Input**: `harvard.wav` (Clear speech sample)
**Output**: Professional quality text transcription suitable for documentation

### Example 2: Music Transcription
**Input**: `Attention-(Mr-Jat.in).mp3` (Music with vocals)
**Output**: Lyrics and vocal content extracted from the song

### Example 3: Batch Processing
Process multiple files in sequence and organize outputs systematically.

## 🛠️ Advanced Configuration

### Model Options
- `tiny`: Fastest, least accurate
- `base`: Good balance (default)
- `small`: Better accuracy
- `medium`: Higher accuracy
- `large`: Best accuracy, slowest

### Custom Parameters
```python
# Transcribe with specific language
result = model.transcribe("audio.wav", language="en")

# Transcribe with temperature for creativity
result = model.transcribe("audio.wav", temperature=0.2)
```

## 🤝 Contributing

We welcome contributions! Here's how you can help:

1. **Fork the repository**
2. **Create a feature branch** (`git checkout -b feature/AmazingFeature`)
3. **Commit your changes** (`git commit -m 'Add some AmazingFeature'`)
4. **Push to the branch** (`git push origin feature/AmazingFeature`)
5. **Open a Pull Request**

### Ideas for Contributions
- Add support for video file transcription
- Implement GUI interface
- Add batch processing with progress bars
- Include timestamp generation
- Add speaker identification

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- [OpenAI Whisper](https://github.com/openai/whisper) - The powerful ASR model that makes this possible
- The open-source community for continuous improvements and feedback

## 📞 Support

If you encounter any issues or have questions:

1. Check the [Issues](../../issues) page
2. Create a new issue if your problem isn't already reported
3. Provide detailed information about your setup and the problem

---

<div align="center">

**⭐ Star this repository if you found it helpful!**

Made with ❤️ using OpenAI Whisper

</div>
