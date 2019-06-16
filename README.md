# AIFORSEA
Submission for Grab aiforsea - Safety

TLDR
- Feature Engineering based on count
- Stacking Model
- 0.8 AUC on train set & 0.74 AUC on validation set
- Customizable probability cut off based on preferred risk appetite
- more detail on notebook

## dependency
- pystacknet https://github.com/h2oai/pystacknet
- sklearn, numpy, pandas, standard python 3 library (up to date version)
- xgboost, shap (optional, used in exploration)


## Usage
1. Put TEST data and TRAIN data into folder hierarchy below:

├── PREDICT.ipynb
├── test
│   ├── features
│   │   ├── x*.csv
│   └── labels
│       └── x.csv
├── train
│   ├── data_dictionary.xlsx
│   ├── features
│   │   ├── x*.csv
│   └── labels
│       └── .csv
├── train_data_adv.pkl
└── train_data.pkl

2. Please run PREDICT.ipnyb and put the data test Path.

### Running Time Estimation
- Feature Engineering ~20 minutes
- Training ~3 minutes
Tested on 2 core 16 GB RAM VPS

### Description
Final Model:
- PREDICT.ipnyb 

EDA and Thought process:
-  baseline.html
- advanced.html

References:
- [Insurance Telematics: Opportunities and Challenges with the Smartphone Solution](https://ieeexplore.ieee.org/document/6936433/authors#authors)

- [Grab Weekly Safety Report](https://help.grab.com/driver/en-my/360001944868-Weekly-Safety-Report)

