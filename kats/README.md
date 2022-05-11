# Using Kats to work with time-series data

[Engineering at Meta](https://engineering.fb.com/) team, [published](https://engineering.fb.com/2021/06/21/open-source/kats/) Kats (https://facebookresearch.github.io/Kats/), a one stop shop for time series analysis in Python.

Our experiment ultimately consists of making use of it to *deal with* walking related data coming from acceleromenter(s) and gyroscope(s).

## Installing a working environment locally with Docker

As for the environment, a combination of assets will be used, consisting of:

1. Docker (in host node)
2. Miniconda (docker image)
3. Kats (time-series library)

#### Prepare your environment

Make sure Docker (or Docker Desktop) is running in your environment.

In the terminal, run:

```bash
docker run -i -t -p 8888:8888 continuumio/miniconda3 /bin/bash -c "\
    conda install jupyter -y --quiet && \
    mkdir -p /opt/notebooks && \
    jupyter notebook \
    --notebook-dir=/opt/notebooks --ip='*' --port=8888 \
    --no-browser --allow-root"
```

> There's also the option to use VS Code to run/edit the Notebooks. (Documentation to come in the future).

Once `NotebookApp` gets launched, copy the `http://127.0.0.1[...]` URL that gets printed on screen, head to your browser (in your Docker host machine), and navigate to it.

Open the main notebook (located at `./main.ipynb`, assuming we're looking in the `kats` folder, after cloning this repo. Then, run it. This will install all required dependencies to run Kats inside the running container.

```
# GCC compiler requirement
!apt update && apt install build-essential -y
# Prophet library
!conda install -y -c conda-forge Prophet
# Kats library
!pip install kats
# Installing CmdStan
!install_cmdstan
```
