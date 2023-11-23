# Music-genre-Classification
Sound/Audio signals can be represented in the form of various parameters such as frequency, bandwidth, roll-off and so on. Using various python libraries, we can perform feature extraction for these audio signals. These features can then be processed and further used to perform classification. In this project, we will use GTZAN dataset https://www.kaggle.com/andradaolteanu/gtzan-dataset-music-genreclassification which consists of 10 genre with 100 songs each, all having a length of 30 seconds.

Task:
Take two songs from each of the genre and visualize them and also find their spectrogram.

a) Create a dataset by extracting feature for each of the songs in GTZAN dataset. For our task, we will specifically use the following features: Mel-Frequency Cepstral Coefficients, Spectral Centroid, Zero Crossing Rate, Chroma Frequencies and Spectral Roll-off.
b) Given total 1000 examples, perform K-Means-Clustering on the dataset to cross verify that the optimal number of clusters are 10 (one for each genre).
c) Divide the dataset into two parts: 90% train and 10% test i.e. for each genre use 90% of the dataset as train and the remaining as test dataset.
d) Perform classification using any of the four classification algorithms and compare the accuracy obtained. Study the architecture of the model used and describe the reason for the model with best accuracy
About the Dataset
genres original - A collection of 10 genres with 100 audio files each, all having a length of 30 seconds (the famous GTZAN dataset, the MNIST of sounds)
images original - A visual representation for each audio file. One way to classify data is through neural networks. Because NNs (like CNN, what we will be using today) usually take in some sort of image representation, the audio files were converted to Mel Spectrograms to make this possible.
2 CSV files
Containing features of the audio files. One file has for each song (30 seconds long) a mean and variance computed over multiple features that can be extracted from an audio file.

The other file has the same structure, but the songs were split before into 3 seconds audio files (this way increasing 10 times the amount of data we fuel into our classification models). With data, more is always better.
