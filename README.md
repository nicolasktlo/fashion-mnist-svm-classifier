# Fashion-MNIST SVM classifier

This repo contains a Jupyter notebook where I train a Support Vector Machine (SVM) on the Fashion-MNIST dataset and then test it on a small clothing screenshot dataset.

The goal is to see how well a model trained on clean benchmark images (Fashion-MNIST) transfers to real screenshots from online shops.

## What's inside

- `fashion-mnist-svm-classifier.ipynb` – main notebook with all the code, plots and discussion.
- `requirements.txt` – Python packages needed to run the notebook.
- `data/` – optional folder for my custom clothing screenshots, organised by class label.

## How to run it

1. Clone this repo.
2. Create a virtual environment (optional but recommended).
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

- **Fashion-MNIST** is loaded using the standard API (I don’t upload the full dataset here).
- **Custom clothing screenshots** (if you add them) should go under:

  ```text
  data/clothing_images/
    0-tshirttop/
    1-trouser/
    2-pullover/
    3-dress/
    4-coat/
    5-sandal/
    6-shirt/
    7-sneaker/
    8-bag/
    9-ankleboot/
  ```

Each folder contains `.png` or `.jpg` images for that class.

## What the notebook shows

The notebook:

- Trains an RBF-kernel SVM on Fashion-MNIST.
- Reports accuracy and confusion matrices on the test set.
- Applies the model to my clothing screenshots and compares performance.
- Reflects on why real screenshots are harder (backgrounds, lighting, cropping, etc.).

This is mainly a coursework / learning project, but I’ve tried to keep the structure clean so it can also work as a small portfolio example.
