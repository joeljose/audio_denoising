# Audio Denoising through Morphological Spectrogram Filtering

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/joeljose/audio_denoising/blob/main/spec_morph_filter.ipynb)

In this project we apply image-based morphological filtering to audio spectrograms for removing noise from audio signals. Regions of the spectrogram having high energy are estimated to be of more importance and likely to contain the original audio signal. The process of erosion can remove noise while dilation can then restore any erroneously removed signal regions. The combination of the two techniques results in a non-linear, time-frequency filter. We then recreate the denoised audio from the processed spectrogram.

## How It Works

1. Compute the Short-Time Fourier Transform (STFT) of the noisy audio signal.
2. Convert the STFT magnitude to a grayscale image (0-255).
3. Apply binary thresholding to separate signal from noise.
4. Use morphological **erosion** to remove small noise regions.
5. Use morphological **dilation** to restore any signal that was removed.
6. Apply the resulting binary mask to the original complex STFT.
7. Reconstruct the denoised audio with an inverse STFT.

## Getting Started

```bash
pip install -r requirements.txt
jupyter notebook spec_morph_filter.ipynb
```

Or click the **Open in Colab** badge above to run in Google Colab with no local setup.

## Requirements

See [requirements.txt](requirements.txt) for the full list:

- numpy
- scipy
- matplotlib
- librosa

## Applications

This project was part of a bigger project called "Visual Mic", where we extract audio from motion due to vibrations caused by sound waves on materials. Here is the link to the project: https://github.com/joeljose/Visual-Mic

This denoising algorithm was effective in extracting out the signal from the noisy audio.

## Follow Me

<a href="https://twitter.com/joelk1jose" target="_blank"><img src="https://github.com/joeljose/assets/raw/master/images/tw.png" width="30"></a>
<a href="https://github.com/joeljose" target="_blank"><img src="https://github.com/joeljose/assets/raw/master/images/gthb.png" width="30"></a>
<a href="https://www.linkedin.com/in/joel-jose-527b80102/" target="_blank"><img src="https://github.com/joeljose/assets/raw/master/images/lnkdn.png" width="30"></a>

<h3 align="center">Show your support by starring the repository</h3>
