# Podcast Transcription with AssemblyAI

This Python script facilitates the transcription of podcast episodes using the AssemblyAI transcription service. The process involves downloading podcast episodes based on specific criteria, uploading them to AssemblyAI, and retrieving the transcriptions.

## Usage

1. Install the required Python libraries:

    ```bash
    pip install requests beautifulsoup4 lxml
    ```

2. Set up your AssemblyAI API key as an environment variable:

    ```bash
    export ASSEMBLY_AI_KEY='your_assemblyai_api_key'
    ```

3. Customize the script:

    - Provide the URL of the podcast RSS feed in the `rss_feed_url` variable.
    - Tweak the transcription parameters (e.g., audio start and end times) as needed.

4. Run the script:

    ```bash
    python podcast_transcription.py
    ```

## Script Overview

### Podcast Download

- The script downloads up to 5 podcast episodes based on a keyword search in the episode description.
- Downloaded episodes are saved as MP3 files in the "./downloads/" directory.

### AssemblyAI Transcription

- The script uses the AssemblyAI API to transcribe the downloaded podcast episodes.
- Each podcast episode is uploaded to AssemblyAI, and its transcription status is periodically checked.
- Transcriptions are saved as text files in the "./transcripts/" directory upon completion.

## Important Notes

- Make sure to comply with the terms of service of both the podcast provider and AssemblyAI.
- Adjust the keyword and other parameters based on your preferences.
- Ensure that you have the necessary permissions and rights to transcribe and use the content.

## Dependencies

- [Requests](https://docs.python-requests.org/en/latest/)
- [Beautiful Soup](https://www.crummy.com/software/BeautifulSoup/)
- [lxml](https://lxml.de/)

## Environment Variables

- `ASSEMBLY_AI_KEY`: Your AssemblyAI API key.

## License

This Podcast Transcription script is provided under the [MIT License](LICENSE). Feel free to use and modify it for your specific needs.
