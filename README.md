# VR-EEG-Social-Anxiety
[![Twitter URL](https://img.shields.io/twitter/url?label=%40ANDlab3&style=social&url=https%3A%2F%2Ftwitter.com%2Flizhn7)](https://twitter.com/ANDlab3)

> From [Affective, Neuroscience, and Decision-making Lab](https://andlab-um.com)


## Highlights
* We combined virtual reality & simultaneous EEG-ECG recording to probe the neurophysiological responses of negative emotions, which can be considered as individualistic neural features which can predict individuals’ affective patterns during social interaction

* We found that individual differences in generating emotions during social interactions can be detected through neurophysiological responses. Individuals who shared similar neural patterns during VR-induced anxiety shared a similar effect of cue on their affective experience during social interaction.

* The results also suggested that controlling for other factors, social reward holds a unique contribution to the anxiety component of individuals' mixed affective experience.

* Virtual reality proved to be a valuable tool in creating realistic social and emotional experiences within controlled laboratory settings. This enhances the naturalism of neuroimaging and socio-affective research, which provides deeper insights into human behavior and affection.



## Description
* This repo mainly contains scripts for processing multimodal neurophysiological data from this project. 
* Data modality: EEG (Brain Porduct 64 ch, montage see *BP_Montage*), ECG (BIOPAC 3 leads)
* Paradigm: naturalistic viewing of negative emotinal videos under virtual reality (Unity + Steam VR), computer-based behavioral task, scales
* VR googles: VIVE Pro EYE (HTC)
* Main analysis method: ANOVA, Linear Regresssion, Intersubject similarity analysis (ISC) & Intersubject representational similarity analysis (IS-RSA)

## Structure

```bash
├── Unity_call_python
│   ├── PortEEG.py         # set the trigger to EEG & ECG
│   ├── AddPortEEG.py      # load the PortEEG function 
│   ├── UnityCallPython.cs # script for importing python script in unity
│   └── inpoutx64.dll      # dll for parallel ports
├── data                   # preprocessed behavioral and EEG data
├── 1_behav_all_figs.qmd   # visualization of the behavioral results
├── 2_ISC_EEG_new.ipynb    # intersubejct simialrity analysis of the EEG data
├── 3_ISC_behav.ipynb      # intersubejct simialrity analysis of the preprocessed behav data
├── 4_ISRSA.ipynb          # intersubject representational similarity analysis
├── LICENSE
└── README.md
```
## Requirements

Python

```bash
python 3.8
mne
neurokit2
pandas
numpy
scipy
statsmodels
matplotlib
seaborn

```

R

```bash
Quarto
ggplot2
tidyverse
dplyr
ggpubr
knitr
circlize
leaps
```
## References
Hu, K., Wang, R., Zhao, S., Yin, E., & Wu, H. (2024). The association between social rewards and anxiety: Links from neurophysiological analysis in virtual reality and social interaction game. *NeuroImage*, 299, 120846. https://doi.org/10.1016/j.neuroimage.2024.120846

```@article{hu2024association,
  title={The association between social rewards and anxiety: Links from neurophysiological analysis in virtual reality and social interaction game},
  author={Hu, Keyu and Wang, Ruien and Zhao, Shaokai and Yin, Erwei and Wu, Haiyan},
  journal={NeuroImage},
  volume={299},
  pages={120846},
  year={2024},
  publisher={Elsevier}
}
```
