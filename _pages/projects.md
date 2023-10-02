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

- Publication: **Nasim Soltani**\*, V. Chaudhary\*, D. Roy, K. Chowdhury, “Finding Waldo in the CBRS Band: Signal Detection and Localization in the 3.5 GHz Spectrum,” IEEE GLOBECOM 2022. [pdf](https://nasimsoltani.github.io/files/waldo.pdf), 
- [Poster](https://nasimsoltani.github.io/files/waldo-poster.pdf) presented at [AI-Edge](https://aiedge.osu.edu/) annual meeting, Septermber 2022, Columbus, Ohio. 
- [Slides](https://docs.google.com/presentation/d/1qv1SYKsGWMZfAAeIvOyLrjOPhzTsuUEhbcy94QAbFmE/edit?usp=sharing) presented at IEEE GLOBECOM December 2022, Rio, Brazil.
- [Dataset](), [Code]().

Other papers that I have co-authored in this topic:
* G. Reus-Muns, P. Upadhyaya, U. Demir, N. Stephenson, **Nasim Soltani**, V. K. Shah, K. R. Chowdhury, “SenseORAN: O-RAN based Radar Detection in the CBRS Band,” IEEE Journal on Selected Areas in Communications (JSAC), July 2023. [link]()
* C. Tassie, A. Gaber, V. Chaudhary, **Nasim Soltani**, M. Belgiovine, M. Loehning, V. Kotzsch, C. Schroeder, and K. Chowdhury, “Detection of Co-existing RF Signals in CBRS using ML: Dataset and API-based Collection Testbed,” IEEE Communications Magazine Accepted May 2023. [link]()

_____________________________________________________________________________

# Neural networks in wireless receiver chain:
**To achieve higher bit error rate**


**For secure communication**

**To reduce communication overhead and increase throughput**

<img align="right" width="40%" src="/images/pronto.drawio.png">
In IEEE 802.11 WiFi-based waveforms, the receiver performs coarse time and frequency synchronization using the first field of the preamble known as the legacy short training field (L-STF). The L-STF occupies upto 40% of the preamble length and takes upto 32 $\mu$s of airtime. With the goal of reducing communication overhead, we propose a modified waveform, where the preamble length is reduced by eliminating the L-STF. To decode this modified waveform, we propose a neural network (NN)-based scheme called PRONTO that performs coarse time and frequency estimations using other preamble fields, specifically the legacy long training field (L-LTF). Our contributions are threefold: (i) We present PRONTO featuring customized convolutional neural networks (CNNs) for packet detection and coarse carrier frequency offset (CFO) estimation, along with data augmentation steps for robust training. (ii) We propose a generalized decision flow that makes PRONTO compatible with legacy waveforms that include the standard L-STF. (iii) We validate the outcomes on an over-the-air WiFi dataset from a testbed of software defined radios (SDRs). Our evaluations show that PRONTO can perform packet detection with 100\% accuracy, and coarse CFO estimation with errors as small as 3%. We demonstrate that PRONTO provides upto 40\% preamble length reduction with no bit error rate (BER) degradation. We further show that PRONTO is able to achieve the same performance in new environments without the need to re-train the CNNs.
Finally, we experimentally show the speedup achieved by PRONTO through GPU parallelization over the corresponding CPU-only implementations.

- Publication: **Nasim Soltani**, D. Roy, K. Chowdhury, "PRONTO: Preamble Overhead Reduction with Neural Networks for Coarse Synchronization," IEEE Transactions on Wireless Communications, March 2023. [pdf](https://nasimsoltani.github.io/files/pronto.pdf)
- [Poster](https://nasimsoltani.github.io/files/pronto-poster.pdf) presented at [WIoT instituite](https://wiot.northeastern.edu/) industry day, May 2023, Boston, MA.
- [Dataset](https://genesys-lab.org/oracle), [Code](https://github.com/nasimsoltani/PRONTO)

