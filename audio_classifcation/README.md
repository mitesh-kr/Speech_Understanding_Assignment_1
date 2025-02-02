# Urban sound classification

The goal of the project is to build a neural network capable of classification on the [Urban Sound 8k dataset](https://drive.google.com/drive/folders/1OjQNi9TJHK99DZyhiZPl8NlFbIQqaLFg?usp=drive_link).<br>

## Project structure
The project folder is structured as follows:
- **data/** contains processed and raw data. To reproduce results using the dataset, 
put the folds folders inside **data/raw/audio**, then put the metadata file inside **data/raw/metadata**
- **models/** contains trained models, namely the scaler and pca used in the project
- **notebooks/** contains the Jupyter notebooks used execute the code
- **src/** contains **data**, **model** and **utils** sub-folders, with code regarding the different parts 
of the project
- **report/** contains the project report written in Latex

## Requirements
Libraries used in the project are the following: *pandas*, *numpy*, *matplotlib*, *tensorflow*, *torch*, *torchvision*, *seaborn*, *keras*, *scikit_learn*, *timm*, *ipython*

You can install them using the following command
```[shell]
pip install -r src/requirements.txt
```

## Methodology
The methodology followed in the project can be seen in the various jupyter notebooks.

### Data Preprocess
In this [first notebook](audio_classifcation/pre_process.ipynb) visual demonstration of spectrogram from each class has been displayed , which is obtained my 3 different window tengniques. <be>.


### Feature extraction and dataset creation
In the [second notebook](https://github.com/tomfran/urban-sound-classification/blob/main/notebooks/02_dataset_extended_cnn.ipynb), more features are extracted and PCA feature selection is exploited to reduce the dataset dimensionality.
Also, audio as an image is extracted from the dataset for later training a CNN.

### Cross validation on the training sets
To understand what training set is best suited for the project, 
cross validation is performed on the initial, scaled, extended and pca dataset obtained at the previous step.
The results are presented in the [third notebook](https://github.com/tomfran/urban-sound-classification/blob/main/notebooks/03_cross_validation_mlp.ipynb).

### Hyperparameter tuning 
After selecting the best dataset from the cross validation results, 
a Random Search is performed to optimize the network hyperparameters, 
details about results as well as test set evaluation can be found on the [fourth notebook](https://github.com/tomfran/urban-sound-classification/blob/main/notebooks/04_hyperparameter_tuning_mlp.ipynb).

### CNN training and tuning
The [last notebook](https://github.com/tomfran/urban-sound-classification/blob/main/notebooks/05_cnn.ipynb) presents the results using a convolutional neural 
network on the image dataset obtained in the second notebook.
This notebook was executed on Google Colab for performance reasons.
