# Audio denoising through morphological processing of the spectrogram of audio signals 


[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://github.com/joeljose/audio_denoising/blob/main/spec_morph_filter.ipynb)

In this project we try out image based morphological filtering to audio spectrograms for removing noise from audio signals. Regions of the spectrogram having high energy are estimated to be of more importance and likely to contain the original audio signal. The process of erosion can remove noise while dilation can then restore any erroneously removed signal regions. The combination of the two techniques results in a non-linear, time-frequency filter. We then recreate the denoised audio from the processed spectrogram.

## Applications

This project was part of a bigger project called "Visual Mic", where we extract audio from motion due to vibrations caused by sound waves on materials. Here is the link to the project: https://github.com/joeljose/Visual-Mic </br> This denoising algorithm was effective in extracting out the signal from the noisy audio.



## Follow Me
<a href="https://twitter.com/joelk1jose" target="_blank"><img class="ai-subscribed-social-icon" src="https://github.com/joeljose/assets/blob/master/images/tw.png" width="30"></a>
<a href="https://github.com/joeljose" target="_blank"><img class="ai-subscribed-social-icon" src="https://github.com/joeljose/assets/blob/master/images/gthb.png" width="30"></a>
<a href="https://www.linkedin.com/in/joel-jose-527b80102/" target="_blank"><img class="ai-subscribed-social-icon" src="https://github.com/joeljose/assets/blob/master/images/lnkdn.png" width="30"></a>

<h3 align="center">Show your support by starring the repository 🙂</h3>
