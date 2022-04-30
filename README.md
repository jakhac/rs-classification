# Computer Vision for Remote Sensing

## Coding Challenge

As part of a 4-day coding challenge, the goal was to explore an imbalanced dataset containing remote sensing data and build several models to predict labels, for instance agriculture, beach or forest.

This repository contains the notebooks and [final paper](paper_summary.pdf) which summarizes the approach, models and findings. The baseline notebooks contain CNN models trained from scratch achieving 20% respectively 47% accuracy. The transfer learning notebook retrains the final layer of EfficientNet model and labels 83% of images correctly.

## How to execute the code

If you want to reproduce the results or run the models yourself, follow these steps.

__1. Clone the repository__

To this end, execute the following command
```
git clone https://github.com/jakhac/rs-classification
```
and `cd` into the folder.

__2. Include the dataset into the project folder__

There already is a `./ds` folder where the train and test folder should be placed. The folder structure should look like this:

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
└───venv (if used)
```

__3. Install the required packages__ 

A requirements.txt containing all used imports file is provided.
```
pip install -r requirements.txt
```

__4. Run the notebooks.__

Now you can execute the notebooks. By default, the best model for each notebook is loaded such that results are reproduceable (in this case you can skip the execution training..). However, if you can also train the model again. In this case, you have to uncomment one line as explained in the notebooks to evaluate your trained model, instead of loading stored model.



