# MSc Thesis: "Deep Learning for Cycling Infrastructure Mapping from Images and Videos"

This repo contains the code and the report paper I produced as a final thesis for MSc Spatio-temporal Analytics and Big Data Mining at UCL (thesis submitted in September 2021; repo with final work created in June 2021 after receiving the final grade).

Grade: Distinction (72%)


## Summary

Up-to-date maps of cycling infrastructure are important for both cyclists and urban transport planners. However, generating such maps using traditional mapping methods can be a costly and ineffective. This research project makes use of the unique London Cycling Infrastructure Database (CID) imagery to investigate whether deep learning can be used effectively to train a computer vision model to classify images of cycling assets. A framework is created that proposes a partially automated process of updating databases such the CID using this model. A multilabel classifier, built from several binary image classifiers with deep convolutional layers, was trained and tested on unseen image and video datasets respectively to evaluate the feasibility of this framework.

Keywords: computer vision, cycling infrastructure database, deep learning, urban mapping.


## [1. Image Preprocessing](1_image_preprocessing.ipynb)

This notebook was used to select, preprocess and convert into arrays the images from the original CID dataset. Videos of cycling infrastructure used for model evaluation are also converted to images and preprocessed.


## [2. Build and Train Binary Classifiers](2_binary_classifier_training.ipynb)

This notebook goes through building the model architecture and training the binary classifiers for each of the 7 image classes.


## [3. Ensemble Model and Evaluation](3_ensemble_model_and_evaluation.ipynb)

This final notebook contains the code used to evaluate the binary classifier models seperately, and also as an ensemble, on unseen images from the CID and custom videos.


## [4. Report Paper](4_thesis_report_paper.pdf)