FROM continuumio/miniconda:latest

LABEL version="0.1"
LABEL description="Unofficial Ramp-workflow docker"

# Install Ramp-workflow
RUN conda create -n rampwf --yes pip python=3.6 ipykernel jupyter notebook

RUN /bin/bash -c "source activate rampwf && pip install git+https://github.com/paris-saclay-cds/ramp-workflow.git"

RUN echo "conda activate rampwf" >> ~/.bashrc


