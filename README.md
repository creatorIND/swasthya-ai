# Swasthya AI (PulmoEnsemble)

This project aims to create a robust ensemble machine learning model capable of accurately detecting pneumonia from chest X-ray images.  The goal is to provide a tool that could potentially assist medical professionals in making faster and more informed diagnoses, ultimately improving patient care.

`pulmo-ensemble.ipynb` is the only notebook which you need. Other notebooks was just me playing around. Dataset used from Kaggle: [Download link](https://www.kaggle.com/datasets/paultimothymooney/chest-xray-pneumonia)

**PulmoEnsemble** predictions are obtained by averaging the predictions from three different models (for now): `InceptionResNetV2`, `VGG16`, and `Xception`.

Steps to run the notebook locally on your PC:

> Alternatively, you can run it on [Kaggle](https://www.kaggle.com/) by importing the `pulmo-ensemble.ipynb` notebook. They're very considerate, giving 30 hrs/week GPU usage quota. It will be much easier than running it locally on your PC.

 1. First, you need to have Anaconda (or Miniconda) Distribution installed. Check out this link for your specific OS: https://docs.anaconda.com/free/anaconda/install/
 2. Clone this repository. Either download it directly from the browser, or use `git` from  the command line.
 3. Using *Anaconda Prompt*, create a new conda environment, activate it, and install Jupyter Lab using `pip install jupyterlab`. Download this [conda commands cheatsheet](https://docs.conda.io/projects/conda/en/latest/_downloads/843d9e0198f2a193a3484886fa28163c/conda-cheatsheet.pdf) for your reference.
 4. Now, simply enter `jupyter lab` in your terminal to open Jupyter Lab in the browser.
 5. From there, browse to the directory where you downloaded and extracted this repo. Make sure to also download the dataset and include it at the appropriate place. 
 6. Open the `pulmo-ensemble.ipynb` notebook, and run all the cells one by one.
 7. Keep installing the packages till you stop getting any 'package not found' error using `pip` only and not `conda`. I'll update this repo and add `requirements.txt` later :)

To train the models locally using GPU, you may want to check this out from Tensorflow: https://www.tensorflow.org/install/pip
