# DeepSC


This code is a modified version of the code available at this link: 
https://github.com/13274086/DeepSC/tree/master
which is related to the paper "Deep Learning Enabled Semantic Communication Systems" by Huiqiang Xie et al. (arXiv link).

In this modified code, we reproduce some of the results mentioned in the paper. We calculate Mutual Information (MI) and loss during the training process, as well as BLEU scores for 1, 2, 3, and 4-grams to measure performance versus Signal-to-Noise Ratio (SNR).

We conducted this study for different scenarios, varying learning rates (1e-4, 1e-3, and 2e-3), channel types (AWGN and Rayleigh), and the number of layers used in the encoder/decoder sides of the DeepSC model (3 and 4).

In the directory ./data/europarl, must save the last checkpoints (related to the last released epoch number) for each scenario, where checkpoints1 refers to the first scenario an so on. These parameters are detailed in the file training scenarios parameters.pdf.

Additionally, there is a directory named bert that must contain the downloaded BERT model used to estimate sentence similarity. Preprocessing of the data is performed using preprocess_text.py.

Our results in terms of training and performance measurement are presented in the directory extract-data, along with the appropriate Python codes to display the results.

The file performance2.py is a modified version for the sentence similarity metric versus SNR.


this project code has been modified by Raafat Ali.


For additional information on running the code, please refer to the original source code at this link:
https://github.com/13274086/DeepSC/tree/master

