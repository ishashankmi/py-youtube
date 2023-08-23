# YouTube Video to MP3 Converter

This Python script allows you to download audio from a YouTube video and convert it to an MP3 file with a specified bitrate. It uses the `pytube` library for downloading the video and the `ffmpeg` command-line tool for converting the audio to MP3.

## Prerequisites

- Python 3.x
- [pytube](https://pytube.io/en/latest/) library: You can install it using `pip install pytube`
- [ffmpeg](https://www.ffmpeg.org/) command-line tool: You need to have ffmpeg installed on your system.

## Usage

1. Clone the repository or copy the script to your local machine.

2. Install the required Python libraries using the following command:

    ```bash
    pip install pytube
    ```

3. Install `ffmpeg` if it's not already installed. You can download it from the official website: https://www.ffmpeg.org/download.html

4. Run the script using Python:

    ```bash
    python youtube_to_mp3.py
    ```

5. Follow the prompts to provide the YouTube video URL and desired output file name.

## Script Overview

The script performs the following steps:

1. Takes the YouTube video URL and output file name as input.
2. Downloads the audio stream of the video using the `pytube` library.
3. Converts the downloaded `.webm` audio file to an MP3 file using the `ffmpeg` command-line tool.
4. Saves the MP3 file with the desired bitrate and the default title of the YouTube video.

## Notes

- Respect YouTube's terms of service and ensure you have the right to download and use the content.
- Make sure to provide the appropriate input (video URL and output name) as prompted.

## License

This project is licensed under the [MIT License](LICENSE).
