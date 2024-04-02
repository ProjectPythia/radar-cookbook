<img src="thumbnail.png" alt="radar thumbnail" width="300"/>

# Radar Cookbook

[![nightly-build](https://github.com/ProjectPythia/radar-cookbook/actions/workflows/nightly-build.yaml/badge.svg)](https://github.com/ProjectPythia/radar-cookbook/actions/workflows/nightly-build.yaml)
[![Binder](https://binder.projectpythia.org/badge_logo.svg)](https://binder.projectpythia.org/v2/gh/ProjectPythia/radar-cookbook/main?labpath=notebooks)
[![DOI](https://zenodo.org/badge/479066261.svg)](https://zenodo.org/badge/latestdoi/479066261)

This Project Pythia Cookbook covers the basics of working with weather radar data in Python.

## Motivation
This cookbook provides the essential materials to learning how to work with weather radar data using Python.

Most of the curriculum is focused around the Python ARM Toolkit, which is defined as:

"a Python module containing a collection of weather radar algorithms and utilities. Py-ART is used by the Atmospheric Radiation Measurement (ARM) user facility for working with data from a number of its precipitation and cloud radars, but has been designed so that it can be used by others in the radar and atmospheric communities to examine, processes, and analyze data from many types of weather radars."

Once you go through this material, you will have the skills to read in radar data, apply data corrections, and visualize your data, building off of the core foundational Python material covered in the [Foundations Book](https://foundations.projectpythia.org/landing-page.html)

## Authors

[Max Grover](https://github.com/mgrover1), [Zachary Sherman](https://github.com/zssherman), [Milind Sharma](https://github.com/gewitterblitz)

### Contributors

<a href="https://github.com/ProjectPythia/radar-cookbook/graphs/contributors">
  <img src="https://contrib.rocks/image?repo=ProjectPythia/radar-cookbook" />
</a>

## Structure
This cookbook is broken up into two main sections - "Foundations" and "Example Workflows."

### Foundations
The foundational content includes the:
- Py-ART Basics - an overview of Py-ART package, how to read in data, and basic plotting functionality
- Py-ART Corrections - how to correct your data, especially when dealing with raw radar data
- Py-ART Gridding - how to utilize the gridding tools in Py-ART

If you are new to Py-ART, starting with the basics is a good place to start, and is required to know before moving onto Py-ART Corrections and Py-ART Gridding.

### Example Workflows
Here, we **apply** the lessons learned in the foundational material to various analysis workflows, including everything from reading in the data to plotting a beautiful visualization at the end. We include the additional dataset-specific details, focusing on building upon the foundational materials rather than duplicating previous content.

## Running the Notebooks
You can either run the notebook using [Binder](https://binder.projectpythia.org) or on your local machine.

### Running on Binder

The simplest way to interact with a Jupyter Notebook is through
[Binder](https://binder.projectpythia.org), which enables the execution of a
Jupyter Book in the cloud. The details of how this works are not
important for now. All you need to know is how to launch a Pythia
Foundations book chapter via Binder. Simply navigate your mouse to
the top right corner of the book chapter you are viewing and click
on the rocket ship icon, (see figure below), and be sure to select
“launch Binder”. After a moment you should be presented with a
notebook that you can interact with. I.e. you’ll be able to execute
and even change the example programs. You’ll see that the code cells
have no output at first, until you execute them by pressing
`Shift` `Enter`. Complete details on how to interact with
a live Jupyter notebook are described in [Getting Started with
Jupyter](https://foundations.projectpythia.org/foundations/getting-started-jupyter.html).

### Running on Your Own Machine
If you are interested in running this material locally on your computer, you will need to follow this workflow:

1. Clone the ["radar-cookbook"](https://github.com/ProjectPythia/radar-cookbook) repository
    ```bash
    git clone https://github.com/ProjectPythia/radar-cookbook.git
    ```

2. Move into the `radar-cookbook` directory
    ```bash
    cd radar-cookbook
    ```

3. Create and activate your conda environment from the `environment.yml` file
    ```bash
    conda env create -f environment.yml
    conda activate radar-cookbook-dev
    ```

4.  Move into the `notebooks` directory and start up Jupyterlab
    ```bash
    cd notebooks/
    jupyter lab
    ```

At this point, you can interact with the notebooks! Make sure to check out the ["Getting Started with Jupyter"](https://foundations.projectpythia.org/foundations/getting-started-jupyter.html) content from the [Pythia Foundations](https://foundations.projectpythia.org/landing-page.html) material if you are new to Jupyter or need a refresher.
