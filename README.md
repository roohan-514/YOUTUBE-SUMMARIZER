
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