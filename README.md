# Neurons
Run it in your browser on Kaggle instead:
https://www.kaggle.com/code/olekristianouff/neuron-tutorial

YouTube tutorial:
https://youtu.be/H8_fhavLdoA

This is the notebook from my YouTube tutorial on how to make a neuron from scratch. Play around and edit it. You can also try forking it, fixing it, and making a pull request if you want to learn how to do that!

## What Is Included

- [`neurons.ipynb`](neurons.ipynb), the tutorial notebook
- [`requirements.txt`](requirements.txt), a pip-based install list
- [`environment.yml`](environment.yml), a Conda environment file
- [`pyproject.toml`](pyproject.toml), project metadata for modern Python tooling

## Install

Click the green code button on the upper right part of the files window, and download as zip. Extract anywhere. Make sure you have Python installed.

Open a cmd window in the folder with the extracted files and write these lines one by one in the window.

### Option 1: `requirements.txt`
this is the easiest one.
```bash
python -m venv .venv
.venv\Scripts\activate
pip install -r requirements.txt
```

### Option 2: `environment.yml`

```bash
conda env create -f environment.yml
conda activate neurons
```

### Option 3: `pyproject.toml`

If you use `uv`, install from the project metadata with:

```bash
uv sync
```

## Open The Notebook

```bash
jupyter notebook neurons.ipynb
```

## Sharing On Kaggle Or Google Colab

You do not need to add anything extra for the repo itself, because the dependency files already cover the Python packages used here.

For Kaggle or Colab, the usual extra step is to add a setup cell at the top of the notebook so the platform installs dependencies before running the rest of the code.

### Colab

```bash
!pip install -r requirements.txt
```

### Kaggle

```bash
!pip install -r requirements.txt
```

# Support me
https://ko-fi.com/snowpire

https://www.patreon.com/cw/Snowpire
## Notes

- The notebook uses `mplcursors` and the Matplotlib widget backend in a few places, so interactive behavior can vary a bit across platforms.
- If a hosted notebook does not render widgets cleanly, switch to the inline backend or keep a fallback cell ready.
