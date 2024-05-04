
# YOUTUBE SUMMARIZER

A YouTube summarizer is a tool that leverages the power of AI to generate summaries of YouTube videos. It uses APIs like the YouTube Data API to get the transcript of the video. This tool is not limited to English content and can handle non-English videos by automatically grabbing the auto-generated English transcript before summarizing it.

This tool is for anyone who wants to quickly understand the key points of a YouTube video without having to watch the entire video. It's particularly useful for those who consume a lot of video content for research, learning, or entertainment purposes. It can save time and help in retaining information more effectively.


## Features

- Supports multiple AI models for summarization, including Pegasus, BART, mT5, and IndicBART.
- Can handle videos in multiple languages by automatically translating the transcript to English before summarizing it.
- Provides a user-friendly interface to enter the YouTube link and get the summary.
- Can also generate summaries for multiple videos in batch mode.
- Provides additional functionality to get video details like title, views, likes, dislikes, and duration using pytube.
- Includes data preprocessing, model training, and evaluation modules for custom model development.
- Includes visualisation of data into graphs , charts , heatmaps.


## Requirements

- Python 3.6 or higher
- transformers 4.11.3 or higher
- youtube-transcript-api 6.0.0 or higher
- pytube 9.6.4 or higher
- nltk 3.6.5 or higher
- sentencepiece 0.1.95 or higher
- numpy 1.21.2 or higher
- matplotlib 3.4.2 or higher
- keras 2.6.0 or higher


## INSTALLATION

To deploy this project run

```bash
  git clone https://github.com/rooohan-514/youtube-video-summarization.git
```

Install the packages

```bash
pip install -r requirements.txt
```




## Usage

1. Run the script:
```bash
python youtube_summarizer.py
```
2. Enter the YouTube link when prompted.

3. Select the AI model for summarization.

4. Get the summary of the video.

5. Get relevant videos based on the url.



## Batch Mode

1. Prepare a CSV file with the YouTube links.

2. Run the script in batch mode:

```bash
python youtube_summarizer.py --batch_file path/to/csv_file.csv
```


## Data Preprocessing

1. Pre process the data 

``` bash
python preprocess.py
```

2. Train model 

``` bash 
python train.py
```

3. Evaluate the model 

``` bash 
python evaluate.py
```

4. Visualise the data into graphs , heatmaps , etc


## Project work flow

1. Once the file starts, open it in your web browser.

2. Enter the url of the YouTube video you want to summarize in the provided text input.

3. Click the run/execute to begin the summarization process.
  - The application will get the Transcription from Youtube
  - It will then use GPT-3.5 and bart to generate a summary.
  - The generated summary will be displayed on the output box in the language of the transcript.
  - If you want to translate the summary in your preferred language input the language and execute the code the summary will be translated in your preferred language.

4. The code will than extract the data from the youtube url that is provided by you and extract data from it such as likes , dislikes , duration , views.

5. Then it will provide some url links that will be referrenced to the url selected. For further help.

6. The accuracy of the output will be given to you that will help you know that how much the models are accurate in providing the summary from the video.

7. It will display the heatmaps , graphs according to the data provided.

## SNAP SHOT OF SOME OUTPUTS ( VISUALISATIONS )
![Screenshot 2024-05-04 183607](https://github.com/roohan-514/YOUTUBE-SUMMARIZER/assets/113782123/c4c0da05-2adb-4ef1-9882-4c245a4106b7)
![Screenshot 2024-05-04 183453](https://github.com/roohan-514/YOUTUBE-SUMMARIZER/assets/113782123/cebbca50-90df-463a-b47d-f4a22ff223a2)
![Screenshot 2024-05-04 183425](https://github.com/roohan-514/YOUTUBE-SUMMARIZER/assets/113782123/79f931f7-c094-4a4c-aed9-b0f543ff439c)
![Screenshot 2024-05-04 183650](https://github.com/roohan-514/YOUTUBE-SUMMARIZER/assets/113782123/221f65e3-50a3-4e24-99b7-13103d116826)
![Screenshot 2024-05-04 183731](https://github.com/roohan-514/YOUTUBE-SUMMARIZER/assets/113782123/8ed48750-85c4-4d74-90d6-ec1c74c6caa4)
![Screenshot 2024-05-04 183829](https://github.com/roohan-514/YOUTUBE-SUMMARIZER/assets/113782123/8d2db527-9664-4b9b-9586-3e06d7c2d722)
![Screenshot 2024-05-04 181802](https://github.com/roohan-514/YOUTUBE-SUMMARIZER/assets/113782123/35931522-21de-4a56-99d5-683bfe33a6c6)
![Screenshot 2024-05-04 183033](https://github.com/roohan-514/YOUTUBE-SUMMARIZER/assets/113782123/55ded32a-dac1-41ed-8a77-9dc091bcaf2d)
![Screenshot 2024-05-04 183103](https://github.com/roohan-514/YOUTUBE-SUMMARIZER/assets/113782123/c241eb92-566c-4da9-a24c-f858b23bf9e5)
![Screenshot 2024-05-04 183121](https://github.com/roohan-514/YOUTUBE-SUMMARIZER/assets/113782123/ea0ae0d2-b63b-4c08-a903-81b0c6207dfa)
![Screenshot 2024-05-04 183210](https://github.com/roohan-514/YOUTUBE-SUMMARIZER/assets/113782123/05f4f7b2-7248-446c-aa20-fe2a5e9bab33)
![Screenshot 2024-05-04 183228](https://github.com/roohan-514/YOUTUBE-SUMMARIZER/assets/113782123/6d71ef86-95b3-4753-8924-414e90a3eee3)


## Contibuting

Contributions are welcome! Please submit a pull request with your proposed changes.
## Acknowledgements

- YouTube Transcript API: https://github.com/python-youtube-transcript-api/youtube-transcript-api
- transformers: https://github.com/huggingface/transformers
- pytube: https://github.com/pytube/pytube
- nltk: https://github.com/nltk/nltk
- sentencepiece: https://github.com/google/sentencepiece
- numpy: https://github.com/numpy/numpy
- matplotlib: https://github.com/matplotlib/matplotlib
- keras: https://github.com/keras-team/keras
