# Capstone Project
## Bioacoustics

This project aims to use the vocalisations of animals to create a classification model which can be used for species identification. Using audio as apposed to images for species identification has several advantages. Audio is recorded essential in 360 degrees, recording of audio is possible in dense forest conditions and it is possible to record continuous audio of high quality for an extended period as audio files are smaller than video files. 

By converting short audio clips to spectrograms, it is possible to reduce the task to one of image classification. A spectrogram is simply the image that results by taking the Fourier transform, that is it is simply in image of the frequency distribution of the audio over time. Each species vocalisation has a distinct frequency distribution, in most cases visible to the naked eye. 

This project provides a dataset of long recording taken in suburban Durban. Importantly, the data is unlabelled, and the goal is to create a pipeline to classify the species present using only a small subset of data labelled by a user. In this way the pipeline cold be used to process any unlabelled data set provide that a small subset is labelled by hand. This would greatly reduce the man hours required to identify species in audio. 

## Summary of content

| Description        | Link |
|---|---|
| Folder containing two examples of audio recording taking the suburban areas of Durban. The larger data set containing approximately 14 hours of audio is available upon request. |  [here](https://github.com/AmyRouillard/Capstone_Project/tree/main/Audio_files) |
| Audio_processing: This notebook takes long audio recordings and segments them into short clips of the length of the user’s choice. Audio clips are then converted into spectrograms (images in the Fourier domain) and saved. | [here](https://github.com/AmyRouillard/Capstone_Project/blob/main/Notebooks/Audio_processing.ipynb) |
|View_training_data: This file allows one to view the training data. This file can be used to facilitate the process of labelling a small subset of the images. | [here](https://github.com/AmyRouillard/Capstone_Project/blob/main/Notebooks/View_training_data.ipynb) |
| Self_labeling: A classification model is trained on the small subset of labelled images. This model is this used to classify the unlabelled images, provided that a certain confidence threshold is met. Model training is then continued using the new increased image set. |[here](https://github.com/AmyRouillard/Capstone_Project/blob/main/Notebooks/Self_labeling.ipynb)  |
