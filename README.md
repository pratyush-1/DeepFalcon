# ML4SCI DeepFalcon Tasks
The tasks can be accessed from [here](https://docs.google.com/document/d/1bwRaHc0IYIcFOokMcW-mYJv2i24iP1mm08ALTSyQ4EI/edit) 

Applying for: - **Specific Task 1 - "Graph Representation Learning for Fast Detector Simulation"**  and **Specific Task 2 - "Diffusion Models for Fast Detector Simulation"**

## DATASET - Data of Quark/Gluon jet events available [here](https://drive.google.com/file/d/1WO2K-SfU2dntGU4Bb3IYBp9Rh7rtTYEr/view?usp=sharing). The dataset consists of 3 channels (ECAL, HCAL and Tracks) each containing 125x125 images.

### SAMPLE IMAGE CHANNELS-
![input image](https://github.com/pratyush-1/DeepFalcon/blob/main/assets/img.png)

### Common Task 1. Common Task 1. Auto-encoder of the quark/gluon events

* Please train a variational auto-encoder to learn the representation based on three image channels (ECAL, HCAL and Tracks) for the dataset. 

* Please show a side-by-side comparison of original and reconstructed events. 

### Variational Autoencoder reconstructions vs original image
![input image](https://github.com/pratyush-1/DeepFalcon/blob/main/assets/img.png)
![VAE reconstruction](https://github.com/pratyush-1/DeepFalcon/blob/main/assets/vae.png)

### DISCUSSION - 

* As the data doesn't contain normal RGB channels and instead has different channels like ECAL,HCAL,Tracks ,data preprocessing needs to be chosen carefully

* Model architecture might not be too complex to extract the patterns in the underlying data

* Since Images are highly structured data, the pixels are arranged in a meaningful way. If the way pixels are arranged changes then we lose the meaning , hence here convolutions may not work as we aren't dealing with our normal RGB channels image data.

* Instead working with other type of data like graphs (aka Graph Neural Networks) would give better results by extracting features in the graphical representation of the given images.
