# INFO-555_project_2
## Author

Kiwoon Hong
University of Arizona
kiwoon2799@arizona.edu

## Project Title

Data Annotation - Hate Speech Annotation by Sampling Tweets

## Description

Effective hate speech detection is critical to maintaining respectful interactions and protecting communities on social media. Hate speech can have far-reaching consequences, such as discrimination and social division.

This project focuses on annotating hate speech in tweets. Hate speech can range from obvious to subtle. This complexity often leads to problems with both LLM's annotation and in-person annotation.

## Instructions

### Files
* `INFO555_Project2_Kiwoon_Hong.ipynb`: A file that has the code for the project. This includes codes that sampling the data, but also includes loading the sampled and annotated data.
* `INFO_555_Project_2_Writeup`: A 2-page paper containing the description, experiment, analysis, and results of the project. It also includes sampled data and annotated data.
* `~\INFO-555_project_2\data`: A folder for data from the project.
* `~\INFO-555_project_2\tex`: A folder for LaTex files of `INFO_555_Project_2_Writeup`.
### Executing

* You **must** run the code in Google Colab.
* You **must** download this project folder into specific google drive directory like this - `/content/drive/MyDrive/INFO-555_project_2`, otherwise you'll need to change the part of the code that mounts the directory.
* Set the runtime type to GPU.
* You can skip the `Skip this part if you are exploring` part in `INFO555_Project2_Kiwoon_Hong.ipynb`. This part is for making directory(it's been already created now) and downloading sampled data.

### Running code blocks

* If you run them in order from the top, it would work out(You can skip `Skip this part if you are exploring`).
* `Import Libraries`, `Load Dataset`: Import the required libraries and load the dataset from the huggingface
* `EDA`: Shows the structure of your data, but must be run for the next step.
* `Undersampling`: Undersample biased data, and extract some of it.
* `Download the Sampled data` Mount the directory and download the data.
* `Load the annotated data` Load the data that includes tagged labels by annotators.
* `Annotation Using an LLM (Prediction)`: Making a comparison/reference LLM model.
* `Summary Statistics`: Showing and visualizing the distribution of the tagging.
* `IAA` Verifiying data quality by using IAA.
* `Error Analysis`: Showing unmatches between two annotators.
* `Data Quality Demonstration - Logistic Regression`: Building a simple prediction model to demonstrate a utility of the data.

## Data Source
https://huggingface.co/datasets/tweets-hate-speech-detection/tweets_hate_speech_detection