# Generate TV Script
Generate a TV script using Recurrent Neural Network (RNN).  This project is part of the Udacity Deep Learning Nanodegree.

# Introduction
In this project, we'll generate your own [Seinfeld](https://en.wikipedia.org/wiki/Seinfeld) TV scripts using RNNs.  We'll be using part of the [Seinfeld dataset](https://www.kaggle.com/thec03u5/seinfeld-chronicles#scripts.csv) of scripts from 9 seasons.  The trained RNN will then generate a new ,"fake" TV script, based on patterns it recognizes in this training data.


# Instructions

1. Set up the Jupyter ipython notebook environment
2. Load and explore the data
3. Create dictionary of lookup tabe and tokenize punctuations, create dataloaders
4. Implement an RNN using PyTorch's [Module class](http://pytorch.org/docs/master/nn.html#torch.nn.Module) (you may choose to use a GRU or an LSTM)
5. Train the RNN
6. Generate TV script using the trained model

## 1. Set up the Jupyter ipython notebook environment
## 1.1 Installation

* Download [Anaconda](https://www.anaconda.com/distribution/#download-section)

* Install [Anaconda](https://docs.anaconda.com/anaconda/install/)  

## 1.2 Create and Activate the Environment

Please go though this [doc](https://conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html) before you creating an environment.
After that create a environment using following command:

```
conda create --name deep-learning
```

Then activate the environment using following command:

```
activate deep-learning
```

#### Git and version control
These instructions also assume you have `git` installed for working with Github from a terminal window, but if you do not, you can download that first with the command:
```
conda install git
```

**Now, you can create a local version of the project**

1. Clone the repository, and navigate to the downloaded folder. 
```
git clone https://github.com/sureshsubr/generate-tv-script.git
cd generate-tv-script
```

2. Install PyTorch and torchvision; this should install the latest version of PyTorch.
	
	- __Linux__ or __Mac__: 
	```
	conda install pytorch torchvision -c pytorch 
	```
	- __Windows__: 
	```
	conda install pytorch -c pytorch
	pip install torchvision
	```

3. Install a few required pip packages, which are specified in the requirements text file.
```
pip install -r requirements.txt
```
Or
```
conda install --yes --file requirements.txt
```

4. That's it! Open a terminal window and navigate to the project folder. Open the notebook and follow the instructions.
```
jupyter notebook
```

Once jupyter notebook instance is open follow the remaining instructions steps #2 - #6 in the ipython notebook called `dlnd_tv_script_generation.ipynb`.

To exit the environment when you have completed your work session, simply close the terminal window.

__NOTE:__ In the notebook, you will need to train RNNs in PyTorch.  If your RNN is taking too long to train, feel free to pursue the options under the section __Accelerating the Training Process__ below.



#### (Optionally) Accelerating the Training Process 

If your code is taking too long to run, you will need to either reduce the complexity of your chosen RNN architecture or switch to running your code on a GPU.  If you'd like to use a GPU, you can spin up an instance of your own, for example, you can use Amazon Web Services to launch an EC2 GPU instance but note that this costs money!!
