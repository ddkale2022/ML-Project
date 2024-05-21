# ML Project: Kickstarter projects 

This dataset was collected by [bloomwatcher](https://www.kaggle.com/bloomwatcher). He is  a crowdfunding enthusiast.

Assignment 

1 . To analyse and model success factors of kickstarter campaigns at [dataset](https://www.kaggle.com/datasets/kemical/kickstarter-projects).

2. Give new projects an idea what is needed for a successful funding and potentially even predict campaign success upfront.Different 

3. Predict which Kickstarter Project was successful?


This repo contains 
- [Data exploration and cleaning ](1_kickstarter_eda_dk.ipynb)
- [Logistic regression model- base model ](2_log_reg_kickstarter.ipynb)
- [Random forest classification ](3_RF_model_kickstarter.ipynb)
- [column names](column_names.md)

   



## Set up your Environment

### **`macOS`** type the following commands : 

- For installing the virtual environment you can either use the [Makefile](Makefile) and run `make setup` or install it manually with the following commands:

     ```BASH
    make setup
    ```
    After that active your environment by following commands:
    ```BASH
    source .venv/bin/activate
    ```
Or ....
- Install the virtual environment and the required packages by following commands:

    ```BASH
    pyenv local 3.11.3
    python -m venv .venv
    source .venv/bin/activate
    pip install --upgrade pip
    pip install -r requirements.txt
    ```
    
### **`WindowsOS`** type the following commands :

- Install the virtual environment and the required packages by following commands.

   For `PowerShell` CLI :

    ```PowerShell
    pyenv local 3.11.3
    python -m venv .venv
    .venv\Scripts\Activate.ps1
    pip install --upgrade pip
    pip install -r requirements.txt
    ```

    For `Git-bash` CLI :
  
    ```BASH
    pyenv local 3.11.3
    python -m venv .venv
    source .venv/Scripts/activate
    pip install --upgrade pip
    pip install -r requirements.txt
    ```

    **`Note:`**
    If you encounter an error when trying to run `pip install --upgrade pip`, try using the following command:
    ```Bash
    python.exe -m pip install --upgrade pip
    ```


   
## Usage

In order to train the model and store test data in the data folder and the model in models run:

**`Note`**: Make sure your environment is activated.

```bash
python example_files/train.py  
```

In order to test that predict works on a test set you created run:

```bash
python example_files/predict.py models/linear_regression_model.sav data/X_test.csv data/y_test.csv
```

## Limitations

Development libraries are part of the production environment, normally these would be separate as the production code should be as slim as possible.


