# Air Pollution Challenge

Goal of this challenges is to predict PM2.5 particulate matter concentration in the air every day for each city. The data covers the last three months, spanning hundreds of cities across the globe.

---

## Data

The project is providing transparent air quality information for more than 100 countries, covering more than 12,000 stations in 1000 major cities, via those two websites: aqicn.org and waqi.info

## Starting to work

- Chat created
- Data.zip added
- Workflow created
- Kanban Board created
- Repos

## PM2.5 Measures

Key indicator of air quality

## Baseline model

Assupmtion: wind magnitude and air pollution are related

## Evaluation metric

Root Mean Squared Error (train & test)

## Predictive models

- XGBoost
- Random Rorest

## Requirements and Environment

Requirements:
- pyenv with Python: 3.11.3

Environment: 

For installing the virtual environment you can either use the Makefile and run `make setup` or install it manually with the following commands: 

```Bash
pyenv local 3.11.3
python -m venv .venv
source .venv/bin/activate
pip install --upgrade pip
pip install -r requirements.txt
```

## Usage

In order to train the model and store test data in the data folder and the model in models run:

```bash
#activate env
source .venv/bin/activate

python example_files/train.py  
```

In order to test that predict works on a test set you created run:

```bash
python example_files/predict.py models/linear_regression_model.sav data/X_test.csv data/y_test.csv
```
## Limitations

Development libraries are part of the production environment, normally these would be separate as the production code should be as slim as possible.


