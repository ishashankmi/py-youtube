from pytube import YouTube
import subprocess

def download_and_convert_to_mp3(youtube_url):
    try:
        video = YouTube(youtube_url)
        stream = video.streams.filter(only_audio=True).first()

        print("Downloading Video:", video.title)
        video_path = stream.download()

        print("Download complete, converting to MP3...")

        mp3_filename = video.title + '.mp3'
        cmd = f'ffmpeg -i "{video_path}" -b:a 320k "{mp3_filename}"'
        subprocess.call(cmd, shell=True)

        print("Conversion to MP3 complete:", mp3_filename)

    except Exception as e:
        print("An error occurred:", str(e))

if __name__ == "__main__":
    url = input("Enter the YouTube video URL: ")
    download_and_convert_to_mp3(url)
