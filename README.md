# Computer Vision course - final project: Gaze Detection

## Introduction

This project is aimed at mapping images of faces to pixel positions on screens using advanced computer vision techniques, balancing both detection accuracy and efficiency.

## Dataset

The dataset contains 20.800 pictures of faces, gazing at a position on a screen: 

https://www.kaggle.com/datasets/pricoptudor/pogdataset

The data is split into train/validation/test beforehand, based on 3 meta csv files. They map the face pictures to metadata, which includes information about the resolution of each person's screen, both in pixels and in milimeters, and the target gaze position, in pixels and normalized:

https://www.kaggle.com/datasets/pricoptudor/gazedetection-aux

Additionally, due to the nature of the task, the pictures of this dataset were enhanced, using the DeepFace framework, each instance being cut to contain only the face of the gazer, without additional noisy background information:

https://www.kaggle.com/datasets/pricoptudor/gazedetection

Unfortunately, the dataset cannot be made publicly accessible, as the participants mutually agreed to keep the dataset course-private.

## Results

Three main models achieved outstanding results, each improving either accuracy, or efficiency, or both.

For the face-cropped dataset, the results are as follows:

- 87.586 params (Mini model): 4.144 cm
- 379.234 params (Maxi model): 3.413 cm
- 2.389.986 params (Simple model): 3.465 cm
