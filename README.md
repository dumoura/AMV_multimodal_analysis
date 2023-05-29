# AMV Multimodal Sentiment Analysis Project

This Python script uses the `youtube-dl` command-line tool to download YouTube videos, audio, and lyrics from Anime Music Videos (AMVs) to conduct further multimodal sentiment analysis.

## Requirements

- Python 3.6 or above.
- [youtube-dl](https://github.com/ytdl-org/youtube-dl)

## How to Use

1. Install `youtube-dl` using pip:

   ```bash
   pip install youtube-dl
   ```

2. Run the script providing the link to the video as an argument:

   ```bash
   python amvdownloader.py [YouTube URL]
   ```

   Replace `[YouTube URL]` with the URL of the video that you want to download.

## Code

Here is the main command used by this script:

```python
os.system(f"youtube-dl -a {link} -x --audio-format mp3 -i --id")
```

This command does the following:

- `-a {link}`: Downloads the video at the URL specified by `{link}`.
- `-x`: Extracts audio from the video (converts the video to audio).
- `--audio-format mp3`: Specifies that the audio format should be MP3.
- `-i`: Continues on download errors.
- `--id`: Uses the video ID as the filename.

## Warning

Remember, it's your responsibility to respect YouTube's Terms of Service. Make sure that you have the appropriate permissions to download and use the content.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
