# Sequence To Sequence GRU for automatic Spelling Correction.
This repository contains code for an auto spell checker built using **Pytorch** as framework.

We've built encoder-decoder networks using GRU as the building block. 
Luong Attention mechanism is used to speeden up the training process and improve accuracy.

Characters (not words) were provided as input to the architecture while training and testing.   
The model was trained on free cloud GPU available on google colab. 

We used a billion word dataset that Google released for Language Modeling research, and injected artificial noise. 
The noise is the simulated spelling mistakes and the model tries to learn how to correct the input by comparing the output to the original text — an Autoencoder. The dataset can be found [here](https://research.google/pubs/pub41880/)

The trained weights file is available [here](https://drive.google.com/file/d/1-LFmzixL3dMH99nDziw3aVkBIa6BVCUz/view?usp=sharing)

### Major Modifications
- Used GRU instead of RNN as building block.
- Introduced Attention Mechanism

### Acknowledgment
This work is an extension to [this repo](https://github.com/MajorTal/DeepSpell) by Tal Weiss. 
