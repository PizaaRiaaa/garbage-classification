# Garbage Detection Based on Convolutional Neural Network
Final project for an application of machine learning and deep learning course carried out at José Rizal University. The code has been made available as a reference if anyone would like to reproduce the results of this project.

```Please cite this  project if this repository is useful for your research.```

## Project Overview
![screenshot](preview/screenshot.png)
* The objective of this study is to train the model to be able to predict the input images and classify it into one of the
garbage recycling categories, which includes cardboard, glass, metal, paper, plastic, trash.
* The CNN generated an accuracy score of 92.96% which proved that this model has a potential to be used  a a tool for 
predicting garbage clases.
* Databaset includes cardboard(393), glass(491), metal(400), paper(584), plastic(472), trash(127)

![class-distribution](preview/class-distribution.png)

## Data Preprocessing
Steps that were applied for the data preprocessing for all the images in the dataset. 
Each step is decribed below:
* ```Step 1:``` Resized all the images in the dataset to 32x32 pixel to match the input layer of the model
* ```Step 2:``` Converted all the images to grayscale to simplify the model's algorithm and computational requirements
* ```Step 3:``` Normalized image dataset by dividing each pixel value to 255.The pixel value ranges from 0 to 255 for each the
channels (RGB). Dividing it by 255 is necessary to normalize it to 0 to 1 range.
* ```Step 4:``` Flatten all the images into a vector matrix
* ```Step 5:``` Shuffled the train dataset for equal distribution of the data for splitting
* ```Step 6:``` Split the data into three sets - train, test, and validation. This is undergone to avoid data overfitting and to increase the model accuracy score
