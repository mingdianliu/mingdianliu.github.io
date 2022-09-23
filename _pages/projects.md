---
layout: archive
title: "Projects"
permalink: /projects/
author_profile: true
---

{% include base_path %}

## Text-guided music to dance generation [[demo]](https://drive.google.com/file/d/1uRkPxgTAInu8Pk81MsnR0pr4TQTiUaLm/view?usp=sharing)
<b> 2022 Summer Intern at Alexa AI </b>

Generating 3D dances from music is an emerging research topic that can enable delightful use cases such as dance trainer, 
dance animator for avatars, etc. The generated dance motion should conform to constraints of human body mechanics such as 
not hyperextend elbows, and have realistic movements that a human could perform. Previous works approaches use techniques 
such as Full-Attention Transformer, add physics-based constraints and leverage VQ-VAE for feature extraction and fusion to 
generate diverse dance movements. However, these methods do not generalize well to new music. Further, these dance 
motions cannot be easily edited by customers by saying simple text commands such as “Move your right arm up”. We propose an 
alternative approach where we project dance movements and corresponding text descriptions of motion to a common latent space. 
A dance motion codebook conditioned on music features (genre, audio spectogram, beats per minute) is used to predict these 
latent space variables, thus allowing us to generate realistic dance motions and empower our customers to edit dance movements 
by using simple text/voice commands. Our model produces realistic dance predictions. Extensive experiments show that our 
proposed method can enable both algorithmic and personalized dance motion generation from music.

<p float="left" align="center">
<img src="{{ site.baseurl }}/files/music_to_dance_model_1.png" width="500" />
</p>
<p float="left" align="center">
<img src="{{ site.baseurl }}/files/music_to_dance_model_2.png" width="500" />
</p>
<p float="left" align="center">
<img src="{{ site.baseurl }}/files/final_demo.gif" width="500" /> 
<figcaption align="center">
Visualization of the generated dance conditioned on music input and text guidance.
</figcaption>
</p>

## Smart watch-based hand gesture reognition model for AR glass <b><span style="color:red">[[demo]](https://drive.google.com/file/d/1uRkPxgTAInu8Pk81MsnR0pr4TQTiUaLm/view?usp=sharing)</span></b>
<b> 2021 Summer Intern at OPPO US Research Center </b>

Augumented reality (AR) glasses are the promising commerical products as the enterance to Metaverse. However, the common 
user interface (UI) for AR glass is the vision-based hand gesture recognition which can only capture the gestures in the 
view of camera. This limit the usage of AR glass. Here, we proposed a smart watch-based hand gesture recognition system 
which takes the data from Inertial Measurement Unit (IMU) sensor and Photoplethysmography (PPG) sensor as input and 
predicts user's hand gesture in real time. A modified MobileNet deep learning model was trained on 0.4 million data 
collected from various users. The well-trained model has averaged 96% recall and 94% precision for each type of gesture.
By combining handcrafted signal features into the model, we reduced 35% power consumption over existing methods. You can
check the demo here.

<p float="left" align="center">
<img src="{{ site.baseurl }}/files/hand_gesture_recognition_table.png" width="500" />
</p>



## Indoor Activity Recognition with mmWave Radar Sensor for Aging in Place [[demo]](https://drive.google.com/file/d/1lqY2VUE8lh5t8FvmbUYUHSbuY_utCTl-/view?usp=sharing)[[code]](https://drive.google.com/file/d/1lqY2VUE8lh5t8FvmbUYUHSbuY_utCTl-/view?usp=sharing)
<b> Computer Science master thesis </b>

Nowadays, world population aging, which requires heavy investment of time and
manpower in daily care, is having a heavy impact on society and economic of
human beings. To caregivers, injury or death caused by fall-down and declined
self-dependence due to Alzheimer’s disease are two main issues to struggle on.
Herein, we devise a human activity recognition (HAR) system which is potential
to handle these issues. In contrast to traditional system using RGB camera, the
indoor activity recognition system with mmWave Radar offers an service with low
privacy leakage risk without costing any recognition accuracy. Taking the data of
daily indoor activities as input, four deep learning models are trained and com-
pared to build up an optimized activity classifier. The averaged accuracy of best
model in test data set reaches 91.87%, which shows its full potential for practi-
cal deployment. A simplistic user interface (UI) is also designed to demonstrate
the functionality of well-trained model. To implement distributed deployment, we
connect Raspberry Pi to AWS IoT for real-time data collection and processing
respectively. A probability threshold of fall-down action is set by AWS Lambda
to trigger an alarming and call for first-aid in time. We hope the proposed system 
could provide an accurate recognition service which further enable the remote
monitoring for elderly people and reduce labour for caregivers.


<p float="left" align="center">
<img src="{{ site.baseurl }}/files/indoor_activities_recognition_1.png" width="500" />
</p>
<p float="left" align="center">
<img src="{{ site.baseurl }}/files/indoor_activities_recognition_2.png" width="500" />
</p>

## Intelligient Antenna Design using Generative Adversarial Network [[code]](https://drive.google.com/file/d/1lqY2VUE8lh5t8FvmbUYUHSbuY_utCTl-/view?usp=sharing)


Featured by low conduction loss and high radiation efficiency, dielectric resonator antennas (DRA) have been considered 
as a promising antenna type for the applications of 5G technologies at 60 GHz band. To date, the design of the DRA 
mainly depends on the intuitive reasoning and trial-and-error process, which is time-consuming and resource-demanding. 
To address this challenge, a generative adversarial network (GAN)-based approach is developed to automate the design of 
DRA structures. The GAN model incorporates a simulator and generator for the DRA modeling and DRA structure design, 
respectively. A training dataset of the pattern-annotation pairs of geometric shapes and S11 parameter was generated to 
train the GAN model. During the training process, the distribution of this dataset was captured by the end-to-end GAN 
model. The trained GAN model is capable of predicting DRA performance as well as generating new DRA structures according
to a given S11 spectrum.


<p float="left" align="center">
<img src="{{ site.baseurl }}/files/GAN_for_antenna_design.png" width="500" />
<figcaption align="center">
GAN model architecture developed to design DRA patterns with a given S11 spectrum. (a) GAN model consising of generator,
simulator, and critic networks.   The inputs of the generator network (b) include the training S11 data and Gaussian 
noise. {describe the blocks in the figure} The generator output, represeting the calculated DRA pattern, is used as the 
inputs of the simulator and critic networks. The simulator and circtic networks consist of the ConvNet, BN and ResNet.
</figcaption>
</p>

