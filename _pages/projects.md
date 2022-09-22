---
layout: archive
title: "Projects"
permalink: /projects/
author_profile: true
---

{% include base_path %}

## Text-guided music to dance generation
<b> 2022 Summer Inter at Alexa AI </b>

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
<img src="{{ site.baseurl }}/files/final_demo.gif" width="500" /> 
<figcaption align="center">
Visualization of the generated dance conditioned on music input and text guidance).

</figcaption>
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
