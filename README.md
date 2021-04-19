***Setup with Anaconda:***

1. create virtual environment and activate
conda create -n st python pandas tqdm
conda activate st

2. install pytorch (specified version that is cpu only, as my machine does not have cuda graphic card)
conda install pytorch cpuonly -c pytorch
(else, for cuda: conda install pytorch>=1.6 cudatoolkit=11.0 -c pytorch)

3. install simpletransformer
pip install simpletransformers

4. install wandb (weights and biases) for experiment tracking and visualizin training in a web browser.
pip install wandb



Negative polarity is class 1, and positive class 2










`remarks: pipenv is not working for this`
1. create local environment in python 3
pipenv --python 3
2. install packages `pandas` and `tqdm`
pipenv install pandas tqdm
3. install package `pytorch`
pipenv install torch torch==1.6.0+cpu
--->> failing to install pytorch. what the hell. so I abandoned this package manager for now and go with anaconda