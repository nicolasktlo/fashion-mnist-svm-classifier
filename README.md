# Fashion-MNIST SVM classifier

This repo contains a Jupyter notebook where I train a Support Vector Machine (SVM) on the Fashion-MNIST dataset and then test it on a small custom image dataset.

The aim is to see how well a model trained on clean benchmark images (Fashion-MNIST) transfers to more realistic clothing images.

## What's inside

- `fashion-mnist-svm-classifier.ipynb` – the main notebook with the code, plots and discussion
- `requirements.txt` – the Python packages needed to run the notebook
- `data/` – files related to the datasets used in this project
- `data/newimages.zip` – a zipped version of my custom image dataset

## How to run it

1. Clone this repo.
2. Create a virtual environment if you want to.
3. Install the dependencies:

   ```bash
   pip install -r requirements.txt
   ```

4. Start Jupyter:

   ```bash
   jupyter notebook
   ```

5. Open `fashion-mnist-svm-classifier.ipynb` and run the cells from top to bottom.

## Data

- **Fashion-MNIST** is not uploaded in full to this repository.
- **Custom images** are included as `data/newimages.zip`.
- I uploaded the custom dataset as a zip file because the original image folder was too large for GitHub.

## What the notebook shows

The notebook:

- trains an RBF-kernel SVM on Fashion-MNIST
- reports accuracy and confusion matrices on the test set
- applies the model to my custom image data
- reflects on why real images are harder than benchmark images, for example because of backgrounds, lighting and cropping

This is mainly a coursework / learning project, but I’ve tried to keep it tidy enough to also work as a small portfolio project.
