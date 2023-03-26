Sure, here's the README.md file:

```
# MP4 to MP3 Converter

A Python application that converts MP4 files to MP3 using the FFmpeg library.

## Installation

To install the dependencies, run:

```bash
pip install -r requirements.txt
```

## Usage

To run the application, simply run the `main.py` file:

```bash
python main.py
```

The input file name and output file name are hardcoded in the `main.py` file. You can modify them to suit your needs.

## Docker

To run the application using Docker, first build the Docker image:

```bash
docker build -t mp4-to-mp3-converter .
```

Then, run the Docker container:

```bash
docker run -p 8000:8000 mp4-to-mp3-converter
```

The application will be available at `http://localhost:8000`.

## Files

- `ffmpeg.py`: Contains the `convert_to_mp3` function that uses FFmpeg to convert MP4 files to MP3.
- `main.py`: The main file that uses the `convert_to_mp3` function to convert the input file to MP3.
- `requirements.txt`: Contains the Python dependencies required by the application.
- `Dockerfile`: The Dockerfile used to build the Docker image.