---
layout: archive
title: "Projects"
permalink: /projects/
author_profile: true
---

My PhD research is broadly in the area of deep learning for the physical layer.
Specifically I have used deep learning for two distinct ares of:
* Deep learning for signal classification, RF fingerprinting. 
* Deep learning in the wireless receiver chain.

# Deep Learning for signal classification and RF fingerprinting:
**Deep learning-aided signal detection and spectrum localization in the CBRS band**

<img align="right" width="30%" src="/images/waldo.drawio.png">
Opening the Citizen Broadband Radio Service (CBRS) band in the US to secondary users offers unprecedented opportunities to LTE and 5G networks, as long as incumbent radar signals are protected from interference. Towards this aim, the US Federal Communications Commission (FCC) requires Environmental Sensing Capabilities (ESCs) to be installed along the coastal regions. Furthermore, FCC mandates that the secondary users transmit with low power levels, such that the aggregated interference and noise power in the vicinity of ESC sensors remains below -109 dBm/MHz. At this interference level, the ESC must detect 99\% of radar pulses with peak power of at least -89 dBm/MHz. In this paper, we design an enhanced ESC sensor, called ESC+, that leverages the deep learning framework called `you only look once' (YOLO) for signal detection using spectrograms. We propose a two-stage spectrogram-based coarse and fine signal analysis method for: (i) detecting, and characterizing radar pulses in environments where the aggregated noise and interference level goes beyond FCC restrictions, and (ii) detecting and characterizing other signal types (e.g., 5G and LTE) in the CBRS band, with a goal of determining unauthorized users. We generate a realistic spectrogram dataset in MATLAB consisting of three signal types of radar, 5G, and LTE where the aggregated interference and noise power occurring concurrently with the radar pulse is varied upto -104 dBm/MHz. We show 100\% radar pulse detection in interference and noise levels of up to 3 dB higher than what is required today.

[paper](https://nasimsoltani.github.io/files/waldo.pdf), [poster](https://nasimsoltani.github.io/files/waldo-poster.pdf) presented at [AI-Edge](https://aiedge.osu.edu/) annual meeting Septermber 2022, [slides](https://docs.google.com/presentation/d/1qv1SYKsGWMZfAAeIvOyLrjOPhzTsuUEhbcy94QAbFmE/edit?usp=sharing) presented at IEEE GLOBECOM December 2022, [Dataset](), [code]().
