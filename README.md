# NanopolishComp 0.2.1 package documentation

---

**Python package for upstream preprocessing and downstream analysis of nanopolish**

---

* Author: Adrien Leger - aleg {at} ebi.ac.uk
* URL: https://github.com/a-slide/NanopolishComp
* Licence: MIT
* Python version: >=3.3

# Installation

Ideally, before installation, create a clean python3 virtual environment to deploy the package, using virtualenvwrapper for example (see http://www.simononsoftware.com/virtualenv-tutorial-part-2/).

## Required python packages:

[Nanopolish 0.10+](https://github.com/jts/nanopolish) is required to generate the files used by  several commands from this package

All python dependencies are automatically installed with pip

## Installation with pip

Ideally, before installation, create a clean python3 virtual environment to deploy the package, using virtualenvwrapper for example (see http://www.simononsoftware.com/virtualenv-tutorial-part-2/).

* To install the package

    ```pip3 install git+https://github.com/a-slide/NanopolishComp.git```

* To update the package:

    ```pip3 install git+https://github.com/a-slide/NanopolishComp.git --upgrade```

## Command list

* **Eventalign_collapse**
This program collapses the raw file generated by *nanopolish eventalign* by kmers rather than by event.

The following fields are discarded: *strand, event_index, model_kmer, model_mean, model_stdv, standardized_level, samples*

If using the *--signal-index* option the *start_idx* and *end_idx* are updated to correspond to the entire kmer signal.

If using the *--samples* mean, median, std and variance are computed for each kmer based on the raw datapoint

## Usage

The package has a command line interface and a Python API.

The usage is detailed in the [usage jupyter notebook](https://nbviewer.jupyter.org/github/a-slide/NanopolishComp/blob/master/tests/NanopolishComp_usage.ipynb?flush_cache=true)


# Note to power-users and developers

Please be aware that NanopolishComp is an experimental package that is still under development. It was tested under Linux Ubuntu 16.04 and in an HPC environment running under Red Hat Enterprise 7.1.

You are welcome to contribute by requesting additional functionalities, reporting bugs or by forking and submitting patches or updates pull requests

Thank you

### Contributors

### Acknowledgments
