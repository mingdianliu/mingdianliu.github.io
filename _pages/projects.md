---
layout: archive
title: "Projects"
permalink: /projects/
author_profile: true
---

{% include base_path %}

## Text-guided music to dance generation
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
proposed method can enable both algorithmic and personalized dance motion generation from music. You can check the demo with music
[here](https://drive.google.com/file/d/1uRkPxgTAInu8Pk81MsnR0pr4TQTiUaLm/view?usp=sharing).

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

## Smart watch-based hand gesture reognition model for AR glass
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








[//]: # (<iframe src="https://drive.google.com/file/d/1uRkPxgTAInu8Pk81MsnR0pr4TQTiUaLm/preview"></iframe>)

[//]: # (<video autoplay="autoplay" loop="loop" width="768" height="512">)

[//]: # (  <source src="/assets/images/lorenz.mp4" type="video/mp4">)

[//]: # (  <source src="/assets/images/lorenz.webm" type="video/webm">)

[//]: # (</video>)


[//]: # (<p float="left" align="center">)

[//]: # (<img src="{{ site.baseurl }}/images/ADELE.png" width="500" /> )

[//]: # (<figcaption align="center">)

[//]: # (Visualization of the segmentation results of the baseline method SEAM and the baseline combined with the proposed ADaptive Early-Learning corrEction &#40;ADELE&#41;.)

[//]: # (</figcaption>)

[//]: # (</p>)
