# Road_Damage_Detection_Using_YOLOV3

This repository contains solution for the topic which I have selected as part of self case study on Deep learning using one of the state of art architecture YOLOv3 to detect road damages of different types.

Link : https://arxiv.org/pdf/2008.13101.pdf

# 1. Problem Description:

India is one of the busiest nations in the world in terms of traffic and as
per the Indian ministry of road transport and highways provided
figures of 2015,2016 and 2017 that over 9300 people were killed and
nearly 25000 people were injured in road accidents due to potholes
and damage roads which is grave concerns in a country like india over
these deaths because these deaths are more than due to terror
attacks(reference
https://www.indiatoday.in/india/story/over-9300-deaths-25000-injured
-in-3-years-due-to-potholes-1294147-2018-07-24).

And road infrastructure plays crucial role in saving lives and economic
development of a country, so to reduce the road accidents due to
potholes and damaged roads it's an important task to manage and
inspect the roads on a timely basis because roads deteriorate over
time considering various factors related to location,age, temperature
etc.
Visual inspection of roads by engineers is very time consuming given
the extensive length of roads or highways. So to come up with an
automated AI based solution which can detect the type of damage can
help and improve the way of monitoring of road conditions.

So the main agenda of this problem is to analyze how can we utilize
the Japanese dataset to detect road damages in other countries.

# 2. Solution Description:

To solve this problem, I had implemented 2 Models each with by using only Japan dataset, only Indian dataset and by combining both the dataset.
  * Model 1: Implemented Model 1 on all the above mentioned datasets using precomputed anchor boxes on COCO dataset.
  * Model 2: Implemented Model 2 on all the above mentioned datasets by computing custom anchor boxes using K-means clustering algorithm as per the given datasets.
 And after selecting best model deployed the app using streamlit on GCP and also on Heroku.
 
# 3. Dataset:
Dataset can be found from here https://github.com/sekilab/RoadDamageDetector which consists of 3 zip files one for train images consisting of already annotated xml files and images  and two files for testing on images.

# 4. Hardware:

Due to GPU limitations on my system, I implemented and trained all models for this case study on Google colab.

# 5. Libraries:

Below libraries used for solving this problem:

* seaborn
* xml
* opencv
* matplotlib
* numpy
* imgaug - library for augmenting images and its corresponding bounding boxes 
* tensorflow
* tensorflowlite
* streamlit
* sklearn
* And many more


