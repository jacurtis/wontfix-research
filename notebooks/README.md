# How to use these Notebooks?

This directory contains a collection of Jupyter Notebooks that demonstrate how to use or reproduce the `wontfix` 
research.

The Notebooks each isolate a step in the research process, from data collection to model evaluation. They are designed
to be run in order, as each Notebook depends on the output of the previous one.

The outputs are generally stored into the `data/` directory, and the Notebooks are designed to read and write from this
directory.

## Notebook Overview and Order

1. `01-setup.ipynb`
    - This Notebook sets up the environment and installs the necessary packages.
    - It does not output any files.
    - It should be run only once if this is the first time running the Notebooks.
    - All future notebooks depend on this one and assume it was ran successfully at least once in the current environment.
2. `02-repo-scan.ipynb`
    - This Notebook scans the repositories and collects the metadata.
    - It outputs the metadata into a CSV file.
3. `03-create-training-dataset.ipynb`
    - This Notebook creates the training dataset from the metadata.
    - It outputs the training dataset into a CSV file.
4. `04-train-model.ipynb`
    - This Notebook trains the model using the training dataset.
    - It outputs the trained model into a file.