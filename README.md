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
```
├── PREDICT.ipynb  
├── test  
│   ├── features  
│   │   ├── *.csv  
│   └── labels  
│       └── *.csv  
├── train  
│   ├── features    
│   │   ├── *.csv  
│   └── labels  
│       └── *.csv  
├── train_data_adv.pkl  
└── train_data.pkl  
```

2. Please open PREDICT.ipnyb and run all.

### Running Time Estimation
- Feature Engineering ~20 minutes (Unoptimized Pandas bottleneck)
- Training ~3 minutes
  
Tested on 2 Core CPU 16 GB RAM VPS

### Description
Final Model:
- PREDICT.ipnyb 

Thought process and EDA:
- baseline.html
- advanced.html

References:
- [Insurance Telematics: Opportunities and Challenges with the Smartphone Solution](https://ieeexplore.ieee.org/document/6936433/authors#authors)

- [Grab Weekly Safety Report](https://help.grab.com/driver/en-my/360001944868-Weekly-Safety-Report)

