# Cataract-phase-recognition
Surgical Workflow Analysis - Cataract Phase Recognition

Link to Presentation: https://docs.google.com/presentation/d/1UFIC4-HahptUiadY_2NTNrZ52LSX2ULtdI2lOstg-d4/edit#slide=id.g180656819a4_0_52

Overview:

Surgical work
ow analysis is currently an active area of computer vision research, the process of
which is to analyze video of endoscopic surgeries to automatically detect its different phases. In
this research, the end-to-end recurrent convolutional networks are developed for cataract surgical
workfow analysis based on a temporal memory relation network, referred to as CataRCNet. The
research goal is to leverage supervised deep learning algorithms to classify cataracts video frames
according to their surgical phases. In this project, nine methods are designed to recognize the steps
of cataract surgery including three different network architectures with three different backbones,
and they all can complete the recognition task. The Non-local operator and temporal variant layer
are designed to provide long-range and multi-scale temporal supportive information for accurate
classi cation without disturbing the end-to-end learning process. The highest f1-score of 25 test
videos is 0.7796 achieved by the end-to-end ResNet50 plus LSTM model.

Key Challenges

- Quality of video/image data and the difficulty in procuring high quality data 
- Noise in Data 
- Transition between different phases during the surgery 
- Capturing spatio-temporal features effectively. These are those features in the images/videos which vary with time and space. 
- Surgeon’s experience plays a role in how much time a surgeon spends on a particular phase. Experience surgeons spend more time than a inexperienced one so having data covering the operations conducted by different level of experienced surgeons ends up making a difference in terms of how well our model is able to generalize. 
- Capture Long term temporal dependencies - Capturing long-term temporal dependencies in videos means understanding and modeling the relationships and patterns that exist over an extended period of time within a video sequence. In other words, it involves recognizing how events and actions evolve, persist, or change over a substantial duration in a video. Coming up with a model/architecture which does exactly that is challenging.
  

Key Contributions

- CataRCNet - This architecture was previously used for colonoscopy videos and this is the first time we used it for Cataract Surgeries
- SV-DenseRCNet - first use of DenseNet169 as the backbone 
- We were able to process long Cataract surgery video clips. The previous methodologies at the time failed to do so
- Capturing spatio-temporal features in a efficient way


About the Dataset and Preprocessing

Videos - average - 10 mins, min - 6, max - 40, 9 hours of surgery 
Train - 25 vids
Validation - 5 vids
Test - 20 Vids
19 phases/steps 					
common steps - 0, 3, 4, 5, 6, 7, 8, 10, 13, 14, 15, and 18 
special steps - 1, 2, 9, 11, 12, 16, 17
Downsample, Resolution Augmentation, Cropping, Jitter, Flip, Rotation 

