<h1>CNN Waste Segregation<h1>



<b>Introduction<b>

**Business Problem**

Improper waste disposal contributes to environmental degradation, increased landfill waste and inefficient recycling processes. Manual sorting is labour-intensive, error-prone and costly. An AI-powered waste classification system addresses these challenges by streamlining waste segregation, reducing operational costs and improving recycling rates.

**Objective**

The objective of this project is to implement an effective waste material segregation system using convolutional neural networks (CNNs) that categorises waste into distinct groups. This process enhances recycling efficiency, minimises environmental pollution, and promotes sustainable waste management practices.

**Key business benefits:**

Accurately classify waste materials into categories like cardboard, glass, paper, and plastic. Improve waste segregation efficiency to support recycling and reduce landfill waste. Understand the properties of different waste materials to optimise sorting methods for sustainability.

**Use Cases:**

Smart Recycling Bins
Automated Waste Sorting Facilities
Waste Monitoring and Reporting


**Insights:**
All images(7625) provided are colorful of dimensions 256x256x3 which were resized to 64x64 (lower resolution) for the purpose of this assignment.
The seven categories of images are: Cardboard, Food_Waste, Glass, Metal, Other,Paper, Plastic.
The total number of images of 'plastic' category is almost double than that of others.
Decreasing batch_size results in better accuracy
Increasing learning rate(config3 , config 4) results in more fluctuations and lesser validation accuracy in same number of epochs.

**Conclusions:**

For all 5 custom models, train_accuracy improves with epochs however the test_accuracy fluctuates drastically after a certain point which indicates over-fitting. This is most likely due to a relatively simpler model or smaller training data set. We need more traing data and augmented data to help improve model accuracy.
The transfer learning model(ResNet) shows the consistent improvement in test accuracy inline with train accuracy as epochs increase. I expect this to perform better if it is to be trained with more number of epochs
Unexpectedly, the model accuracy has dropped using augmented data. This needs to be investigated further in terms of kind of augmentations done etc(Out of scope of this assignment)

**Technologies Used**

seaborn 0.11.1
jupyter 1.0.0
numpy 1.20.1
anaconda 2021.05
python 3.8.8
matplotlib 3.3.4
tensorflow 2.19.1
Dataset
All images of waste material is available under the following link https://drive.google.com/file/d/1j2dDF3CGA8DsucDfNySNu1lklLa8Tsgr/view?usp=sharing

**Contact**

Created by priyanka9199 - feel free to contact me!
