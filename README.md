# Song-Popularity-Prediction

Using a dataset from Kaggle (derived from Billboard and EchoNest), which contained different songs by different 
artists since 1991 with different sound parameters like time signature, loudness, key, pitch, tempo, and 
timbre. The objective was to build a model to predict whether a song will reach a spot in the Top 10 of 
the Billboard Hot 100 Chart.

![image](https://user-images.githubusercontent.com/86877457/131524822-03f182f0-6b6e-44cc-ad2a-e9b560fec82f.png)


Description
===========

Source: https://www.kaggle.com/didwaniagourav/bill-board-top-100-songs

Data: This data derived from three sources: Wikipedia, Billboard.com, and EchoNest.


**Problem statement**
=====================

How can we use analytics to predict the popularity of a song? I challenge myself to predict whether a song will reach a spot in the Top 10 of the Billboard Hot 100 Chart.

Taking an analytics approach, I aim to use information about a song's properties to predict its popularity. 

**Real-world/Business objectives and constraints**
==================================================
- Artist will only release the song if song has that popularity quotient
- Interpretability is important.
- False claims can be very costly.
- Probability of a data-point belonging to each class is needed.


**Data Overview**
==================
The dataset songs.csv consists of all songs which made it to the Top 10 of the Billboard Hot 100 Chart from 1990-2010 plus a sample of additional songs that didn't make the Top 10. The variables included in the dataset either describe the artist or the song, or they are associated with the following song attributes: time signature, loudness, key, pitch, tempo, and timbre.

With each passing year, the no of hits varried.

![Sheet 1](https://user-images.githubusercontent.com/86877457/131533144-dcdb8716-524f-4d73-bdca-b584474ba05b.png)
Also, total number of hit is almost 1/7th of the total songs released in the period.

![Sheet 1](https://user-images.githubusercontent.com/86877457/131530980-b22322f6-2f81-4279-ae50-9cec46a0fcff.png)


**Example Data Point**
=======================

2010,This Is the House That Doubt Built,A Day to Remember,SOBGGAB12C5664F054,AROBSHL1187B9AFB01,3,0.853,-4.262,91.525,0.953,11,0.453,0.966655566,0.024,0.002,57.342,-6.496,171.093,-81.664,95.117,-285.049,259.426,-40.385,73.63,-104.683,183.089,-88.771,73.549,-71.127,82.475,-52.025,39.116,-35.368,71.642,-126.44,18.658,-44.77,25.989,0

Mapping the real-world problem to an ML problem
==================
There are two ways the song could be classified into => Binary Classification problem

Performance Metric
=================

- Accuracy
- False Positive Rate
- Confusion matrix
- Brier Score Loss

Constraints:
==================
- Interpretability  
- Latency Constraint

Train, CV and Test Datasets
=========================
Split the dataset randomly into three parts train, cross validation and test with 80%,10% and 10% of data respectively

Results Obtained
=========================
 Accuracy: 99%
 FPR: 0.01%
 Train Brier Score Loss: 0.0001
 Test Brier Score Loss: 0.013

