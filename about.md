---
layout: page
title: About our workshop
permalink: /about/
---

Introduction

Devices that document daily life experiences could provide a unique view on the user’s spontaneous speech use. For the past years, speaker recognition research, has mainly focused on telephone and close microphone applications with high speech quality levels. However, far-field recordings have recently emerged as an area of interest. This is due to new applications like annotating the videos in platforms as Facebook and Youtube; home assistant devices which need to distinguish between family members; and wearables that document our everyday life. These applications provide a massive amount of data which requires automatic means of analysis. Furthermore, such devices are often used in very challenging environments with multiple speakers, and where the audio is affected by noise and reverberation.
Most devices use a single microphone and, therefore, multichannel signal processing techniques (e.g., beamforming) cannot be applied to alleviate the impact of the real-life conditions. As reference, speaker detection error rates of reverberant speech are 2 times worse than close talk speech in voices dataset; internet videos with noise and multi-speaker error multiplied by 6 in recent NIST SRE18 w.r.t. clean videos;  and systematic evaluation of commercial diarization on wearables in real-life domain shows diarization error rates of about 60%. The aim of this proposal is to research, develop, and benchmark speaker diarization and speaker recognition systems on far-field speech acquired using single microphones in realistic scenarios that include background noises such as a television audio, music, or other people talking (as shown in Figure 1).


Figure 1. Speaker Detection

To get plausible conclusions, we will explore two complementary scenarios. The first one focuses on acoustically challenging environments with known conditions. The information of the room, noise types, and the position of the microphone will be provided so that each problem can be isolated and studied. The other scenario pertains to day-long recordings from child-worn devices. This is a particular innovation of the project because samples from such recordings portray a broad array of room conditions (including outdoors), noise types, speaker similarity, and other adverse conditions (such as long silences alternating with speech bursts by multiple, potentially overlapping talkers) and furthermore, these conditions are not known. This will allow us to assess to what extent highly informed algorithmic solutions generalize across a range of real-life situations. Furthermore, these two well-defined scenarios will allow more accurate measurements of the performance and generalization level of speaker detection and diarization algorithms.

Research Threads
Research areas for the proposed workshop include:


Figure 2. Research Threads

SAD/Speech Classification: we require robust speech detection. This involves ascertaining that speech is produced by real people in the room or from other sources like HVAC, babble, traffic, TV/radio speech, and music; and that child speech and other immature vocalizations are preserved (rather than treated as noise).

Figure 3. SAD output

Speech enhancement: we need to compensate for the effect of noise and reverberation in far-field audio. For this work, we intend to follow two research tracks for which we already have some preliminary results. The first one is supervised training of neural speech enhancement--given clean-noisy paired data. The focus will be to extend this method to train the enhancement block in combination with the speaker embedding network. The second track is unsupervised training of enhancement using CycleGAN. Special care will be taken to keep the children speech which would otherwise be considered a nuisance for some applications.


Figure 4. Spectrum from noisy to enhanced speech

Speaker Diarization/Tracking: Dealing with the problem of detecting the target speakers within a conversation of multiple other speakers (children-adult scenario, often with overlap.


Figure 5. Diarization (1 is the label for speaker1, 2 is the label for speaker2, blank space is silence)

Domain Adaptation: Adaptation of speaker recognition systems using adversarial training to mitigate expected (but unknown) differences between system training data and the evaluation conditions (e.g. indoor vs. outdoor, controlled vs. adverse). Calibration in far-field conditions will also be of interest since different distances and pathways between the source and the microphone affect the distribution of the scores. Calibration approaches will need to compensate for dynamic changes in the environment, such as movement of the source.

Figure 5. Domain adaptation

Expected Outcomes
As a result of the JSALT workshop, the speech community, industry, and academia, will benefit from: a better understanding of single-microphone far-field speech in real-life scenarios with realistic background noises for speaker detection and diarization task; novel machine learning and signal processing algorithms; and a complete benchmarking of single-microphone realistic databases. Moreover, the research outcomes as papers and shareable code will be a priority for the group.  
We believe that the proposed workshop will provide a concentrated effort to address many of the outstanding research problems in the analysis of speaker recognition techniques using distant speech with single microphones in realistic scenarios and motivate future research in the community.







<!-- This is the base Jekyll theme. You can find out more info about customizing your Jekyll theme, as well as basic Jekyll usage documentation at [jekyllrb.com](https://jekyllrb.com/)

#You can find the source code for Minima at GitHub:
#[jekyll][jekyll-organization] /
#[minima](https://github.com/jekyll/minima)

#You can find the source code for Jekyll at GitHub:
#[jekyll][jekyll-organization] /
#[jekyll](https://github.com/jekyll/jekyll)


#[jekyll-organization]: https://github.com/jekyll -->
