
# Signal to Noise Ratio (SNR)

This repository is Copyright ©Patrik Lechner 2021 under Creative Commons, Attribution-ShareAlike 4.0 International. [![License: CC BY-SA 4.0](https://licensebuttons.net/l/by-sa/4.0/80x15.png)](https://creativecommons.org/licenses/by-sa/4.0/)

It contains only [one notebook](SNR.ipynb) which can be tried [out interactively in callab](https://colab.research.google.com/github/hrtlacek/SNR/blob/master/SNR.ipynb).

This notebook documents how to calculate the Signal to Noise Ratio (SNR) for audio applications in python. This measure is used in many engineering disciplines. In audio applications, the desired signals mostly contain AC components that should not be confused with noise, making simple approaches focusing on DC signals not very useful. 4 Methods are shown here:
- Method 1 assumes we can measure/record a noise only signal, emmitted by the system in question without an input signal.
- Method 2 assumes we can measure an input signal and an output signal of a system. It is assumed that their difference is noise, which is not always the case, especially when we want to measure the SNR of a system that actually does something.
- Method 3 uses the FFT to analyse for a fundamental frequency. It assumes that the input is a sinusoidal signal, the system adds noise and can contain weak non-linearities.
- Methos 4 is here mostly for reference and is mostly suited for DC signals (not audio signals)

## Cite
[![DOI](https://zenodo.org/badge/362257136.svg)](https://zenodo.org/badge/latestdoi/362257136)
