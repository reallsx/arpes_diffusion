# Instruction for setting up environment on rapid cluster

One can access https://hub.rapid.crc.rice.edu if permitted. This document is about how to set up virtual environment for running the code in this repository on the machine.

# Initialize Conda

Open an terminal and run 

`conda init`

Then run the following in the home directory

`source .bashrc`

This should activate conda and put the current shell in the base environment

# Make an environment

Upload `environment.yaml` to the machine and create an conda virtual environment with the file:

`conda env create -n pytorch -f environment.yaml`

after this, activate the environment by

`conda activate pytorch`

and install a ipython kernel so that it can be used in the notebooks

`python -m ipykernel install --user --name=pytorch`

After this step, a kernel named 'pytorch' should should up in the kernel selection list.
