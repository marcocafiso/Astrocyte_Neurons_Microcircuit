# Astrocyte_Neurons_Microcircuit

This repository contains a Brian2 notebook implementing a two-module spiking-neuron and astrocyte model, described in this [bioRxiv preprint](https://www.biorxiv.org/content/10.64898/2026.06.15.732376v1).

The model includes excitatory and inhibitory synapses, astrocyte-neuron interactions mediated by extracellular potassium, and potassium coupling between the two modules. The notebook runs the simulation and plots neuronal, astrocytic, and extracellular potassium dynamics.

## Contents

- `Astro_NN_Two_Modules.ipynb`: model definition, simulation, and plots.
- `requirements.txt`: Python dependencies.

## Installation

Install Python and a C++ compiler (for example, `g++` on Linux). From the project directory, create and activate a virtual environment, then install the dependencies:

```bash
python3 -m venv .venv
source .venv/bin/activate
python -m pip install --upgrade pip
python -m pip install -r requirements.txt
```

## Run

Start Jupyter from the project directory:

```bash
jupyter notebook Astro_NN_Two_Modules.ipynb
```

In Jupyter, run the notebook cells in order. The simulation uses Brian2's C++ standalone device, which compiles the simulation when it runs.
