<!-- TODO:

Repository
- Run notebooks with clean output
- README instruction:
    - How to run this project?
    -  -->

# Coding Challenge - Computer Vision for Remote Sensing

This repository contains the notebooks and models regarding the CV4RS coding challenge.


## How to run this project

If you want to reproduce the results or run the models yourself, follow these steps.

1. Clone the repository.
```
git clone https://github.com/jakhac/rs-classification
```

2. Include the dataset into the project folder. There already is a `./ds` folder where the train and test folder should be placed. The folder structure should look like this:

```
rs-classification
│   README.md
│   notebooks.ipynb
│   requirements.txt
└───ds
    └───test
    └───train
└───models
    └───baseline_v1
    └───baseline_v2
    └───transfer
└───venv (if installed)
```

3. Install the required packages. A requirements.txt containing all used imports file is provided.
```
pip install -r requirements.txt
```

4. Now you can execute the notebooks. By default, the best model for each notebook is loaded such that results are reproduceable (in this case you can skip the execution training..). However, you can also train a model again. In this case, you have to uncomment one line as explained in the notebooks to evaluate your newly trained model, instead of loading the stored model.



