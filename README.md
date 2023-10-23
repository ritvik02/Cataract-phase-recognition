# Cataract-phase-recognition
Surgical Workflow Analysis - Cataract Phase Recognition

Link to Presentation: https://docs.google.com/presentation/d/1UFIC4-HahptUiadY_2NTNrZ52LSX2ULtdI2lOstg-d4/edit#slide=id.g180656819a4_0_52

Overview:

Surgical work
ow analysis is currently an active area of computer vision research, the process of
which is to analyze video of endoscopic surgeries to automatically detect its di erent phases. In
this research, the end-to-end recurrent convolutional networks are developed for cataract surgical
work
ow analysis based on a temporal memory relation network, referred to as CataRCNet. The
research goal is to leverage supervised deep learning algorithms to classify cataracts video frames
according to their surgical phases. In this project, nine methods are designed to recognize the steps
of cataract surgery including three di erent network architectures with three di erent backbones,
and they all can complete the recognition task. The Non-local operator and temporal variant layer
are designed to provide long-range and multi-scale temporal supportive information for accurate
classi cation without disturbing the end-to-end learning process. The highest f1-score of 25 test
videos is 0.7796 achieved by the end-to-end ResNet50 plus LSTM model.
