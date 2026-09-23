---
layout: archive
title: "Projects"
permalink: /projects/
author_profile: true
portfolio: true
excerpt: "Open-source simulation, scientific computing, generative motion models, and multimodal sensing projects by Mingdian Liu."
---

<div class="portfolio-intro" markdown="1">

I build machine learning systems and tools for exploring the physical world—from generative motion and sensing to electromagnetic and neural simulation.

[Recent open source](#open-source) · [Research projects](#research) · [Scientific tools](#scientific-tools)

</div>

<section class="portfolio-section" aria-labelledby="open-source">
  <h2 id="open-source">Recent open-source projects</h2>
  {% include recent-projects.html %}
</section>

<section class="portfolio-section" aria-labelledby="research">
  <h2 id="research">Research projects</h2>

  <article class="research-project" id="t2m-x" markdown="1">
### T2M-X: Expressive text-to-motion generation
<p class="research-project__meta">2023 · Snap Research internship</p>

Generating expressive avatars requires coordinated body, hand, and facial motion, while available datasets often annotate only some of these components. T2M-X learns from partially annotated data using separate VQ-VAE experts for each component and a multi-indexing GPT with a motion consistency loss. The model combines these representations to generate coordinated whole-body motion from text.

[Paper](https://drive.google.com/file/d/1AljEcnaItZXaGAjKdGY_V9Eyi2PM6V-e/view?usp=sharing) · [Appendix](https://drive.google.com/file/d/1d5-iMsslwIhRyMCRekdlssYBF5NEqnWl/view?usp=sharing) · [Demo](https://drive.google.com/file/d/12cWo50pgp_Df5zkKRzdX9Yd3-nh7EsmP/view?usp=sharing)

<figure>
  <img src="{{ '/files/t2m_x_expressive.png' | relative_url }}" alt="Comparison of body-only motion generation and expressive motion including hands and face." width="600" height="445" loading="lazy">
  <figcaption>From body motion to expressive whole-body animation.</figcaption>
</figure>
<details>
  <summary>View model architecture</summary>
  <figure>
    <img src="{{ '/files/t2m_x_network.png' | relative_url }}" alt="T2M-X architecture with separate body, hand, and face VQ-VAE experts, a multi-indexing GPT, and a shared consistency space." width="700" height="336" loading="lazy">
    <figcaption>Specialized motion representations coordinated through a multi-indexing GPT.</figcaption>
  </figure>
</details>
  </article>

  <article class="research-project" id="music-to-dance" markdown="1">
### Text-guided music-to-dance generation
<p class="research-project__meta">2022 · Amazon Alexa AI internship</p>

This project generates dance motion conditioned on music while allowing text-based edits such as “move your right arm up.” Motion and text are mapped into a shared latent space, with a motion codebook conditioned on music features—including genre, spectrograms, and tempo—to produce and edit avatar movements.

[Demo](https://drive.google.com/drive/folders/1R9BbFKLR2VZ2f5bEbwbHGalvwlns7sKR?usp=share_link) · [Slides](https://drive.google.com/file/d/1z7Vhz0aXEqYgoT9cG15GUxZlCZpbX7k0/view)

<figure>
  <img src="{{ '/files/final_demo.gif' | relative_url }}" alt="Animated demonstration of dance motion generated from music and text guidance." width="500" height="281" loading="lazy">
  <figcaption>Dance generation conditioned on music and text guidance.</figcaption>
</figure>
<details>
  <summary>View model diagrams</summary>
  <figure><img src="{{ '/files/music_to_dance_model_1.png' | relative_url }}" alt="Diagram of the text-guided music-to-dance generation model." width="600" height="149" loading="lazy"></figure>
  <figure><img src="{{ '/files/music_to_dance_model_2.png' | relative_url }}" alt="Additional architecture diagram for music-conditioned dance generation." width="600" height="126" loading="lazy"></figure>
</details>
  </article>

  <article class="research-project" id="gesture-recognition" markdown="1">
### Smartwatch-based hand gesture recognition for AR glasses
<p class="research-project__meta">2021 · OPPO US Research Center internship</p>

A wrist-worn gesture recognition system using inertial measurement unit (IMU) and photoplethysmography (PPG) signals, enabling interaction beyond a camera's field of view. A modified MobileNet trained on 0.4 million samples achieved average recall of 96% and precision of 94% across gesture types. Incorporating handcrafted signal features reduced power consumption by 35% relative to the compared methods.

[Demo](https://drive.google.com/drive/folders/1UklKZVgKYQrnBLPTODIE5EwHpESQsKLT?usp=share_link) · [Patent](https://patents.google.com/patent/WO2022221781A1/en) · [Yahoo coverage](https://finance.yahoo.com/news/wearable-devices-mudra-neural-gestures-123000768.html) · [Nomtek coverage](https://www.nomtek.com/blog/ar-glasses) · [TNW coverage](https://thenextweb.com/news/oppo-will-launch-ar-glasses-with-gesture-control-in-2021)

<details>
  <summary>View gesture recognition results</summary>
  <figure><img src="{{ '/files/hand_gesture_recognition_table.png' | relative_url }}" alt="Results table for the smartwatch-based hand gesture recognition model." width="600" height="450" loading="lazy"></figure>
</details>
  </article>

  <article class="research-project" id="radar-activity" markdown="1">
### Indoor activity recognition with mmWave radar
<p class="research-project__meta">Computer Science master's thesis · Iowa State University</p>

A human activity recognition system for aging in place using mmWave radar instead of RGB cameras. Four deep learning models were compared, with the best model reaching 91.87% test accuracy. The prototype connects Raspberry Pi devices to AWS IoT for data collection and processing, with an AWS Lambda threshold for fall alerts.

[Project website](https://smarthomelab.github.io/Indoor-Activity-Recognition-with-mmWave-Radar-Sensor-Page/) · [Demo](https://drive.google.com/file/d/1lqY2VUE8lh5t8FvmbUYUHSbuY_utCTl-/view?usp=sharing) · [Presentation](https://youtu.be/om-5EhamHw8) · [Code](https://github.com/SmartHomeLab/Indoor-Activity-Recognition-with-mmWave-Radar-Sensor-Static)

<details>
  <summary>View system diagrams</summary>
  <figure><img src="{{ '/files/indoor_activities_recognition_1.png' | relative_url }}" alt="Overview of the mmWave radar indoor activity recognition system." width="600" height="184" loading="lazy"></figure>
  <figure><img src="{{ '/files/indoor_activities_recognition_2.png' | relative_url }}" alt="Processing and deployment diagram for radar-based indoor activity recognition." width="600" height="171" loading="lazy"></figure>
</details>
  </article>

  <article class="research-project" id="antenna-gan" markdown="1">
### Intelligent antenna design with generative adversarial networks
<p class="research-project__meta">AI for electromagnetics · AntennaGAN</p>

A GAN-based approach to designing dielectric resonator antennas for the 60 GHz band. A simulator learns the relationship between antenna geometry and the S11 response, while a generator proposes geometric patterns conditioned on a target S11 spectrum. The system reduces reliance on manual trial-and-error design.

[Paper](https://onlinelibrary.wiley.com/doi/full/10.1002/mop.34013) · [Code](https://github.com/mingdianliu/AntennaGAN)

<figure>
  <img src="{{ '/files/GAN_for_antenna_design.png' | relative_url }}" alt="AntennaGAN architecture showing the generator, simulator, and critic networks conditioned on an S11 spectrum." width="600" height="225" loading="lazy">
  <figcaption>The generator proposes antenna patterns from a target S11 spectrum and noise; simulator and critic networks guide training.</figcaption>
</figure>
  </article>
</section>

<section class="portfolio-section" aria-labelledby="scientific-tools" markdown="1">
## Scientific tools
{: #scientific-tools }

- **[ASTRA Toolbox for cone-beam CT](https://github.com/mingdianliu/astra-toolbox-for-cone-beam)** — Python scripts for projection loading, rotation-center determination, and cone-beam reconstruction.
- **[HFSS Python API](https://github.com/mingdianliu/HFSS-Python-API)** — Python helpers for generating HFSS modeling scripts.

</section>
