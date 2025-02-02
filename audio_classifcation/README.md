# Urban sound classification

The goal of the project is to build a neural network capable of classification on the [Urban Sound 8k dataset](https://drive.google.com/drive/folders/1OjQNi9TJHK99DZyhiZPl8NlFbIQqaLFg?usp=drive_link).<br>

## Project structure
The project folder is structured as follows:

## Requirements
Libraries used in the project are the following: *pandas*, *numpy*, *matplotlib*, *tensorflow*, *torch*, *torchvision*, *seaborn*, *keras*, *scikit_learn*, *timm*, *ipython*

You can install them using the following command
```[shell]
pip install -r src/requirements.txt
```

## Methodology
The methodology followed in the project can be seen in the various jupyter notebooks.

### Data Preprocess
In this [first notebook](https://github.com/mitesh-kr/Speech_Understanding_Assignment_1/blob/main/audio_classifcation/pre_process.ipynb) visual demonstration of the spectrogram from each class has been displayed, which is obtained by 3 different window techniques. <be>.


### Feature extraction and dataset creation
In the [second notebook](https://github.com/mitesh-kr/Speech_Understanding_Assignment_1/blob/main/audio_classifcation/feature_extraction.ipynb), using 3 different techniques spectrogram tensors are obtained.



### Hann Window Based Classification
Hann window-based spectrogram tensors are used as input to the vit_tiny_patch16_224 model for classification.
The results are presented in the [third notebook](https://github.com/mitesh-kr/Speech_Understanding_Assignment_1/blob/main/audio_classifcation/hann_window_based_classification.ipynb).

### Hamming Window Based Classification
Hann window-based spectrogram tensors are used as input to the vit_tiny_patch16_224 model for classification.
The results are presented in the [Fouth notebook](https://github.com/mitesh-kr/Speech_Understanding_Assignment_1/blob/main/audio_classifcation/hamming_window_based_classification.ipynb).

### Rectangular Window Based Classification
Hann window-based spectrogram tensors are used as input to the vit_tiny_patch16_224 model for classification.
The results are presented in the [Fifth notebook](https://github.com/mitesh-kr/Speech_Understanding_Assignment_1/blob/main/audio_classifcation/Rectangular_window_based_classification.ipynb).
