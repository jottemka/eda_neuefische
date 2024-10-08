# EDA Project: King County House Sales 2014-2015

<img src="optional/bellevue_fall_lnb6qm.webp" width="600">

This repo contains the results of the EDA project in the neuefische Data Science, Machine Learning & AI Bootcamp. It consists of 2 notebooks:

1. The EDA notebook itself containing a classical EDA and a client-focused EDA:

    - https://github.com/jottemka/eda_neuefische/blob/82a769aa8193682e45b5cc63c326e136f3ea55d0/eda_king_county.ipynb

2. A presentation notebook that was used to generate the corresponding Jupyter slides for the stakeholder meeting:

    - https://github.com/jottemka/eda_neuefische/blob/ef8f00f8dba6c665a72b53648f7c0915470c23d3/presentation.ipynb


## Data Insights

There are 3 interesting data insights that might be contrary to common views:

1. More rooms does mean higher price, but the relationship is not as strong as one might expect.

2. Older houses are not generally cheaper. The correlation is almost zero.

3. Surprisingly, just like agricultural products, house prices exhibit seasonality effects.

## Client Recommendations

Instead of specific buying recommendations, we decided to propose the following methodology to our (fictional) client:

1. Start with most affordable house with at least 3 bedrooms and 2 bathrooms

2. Ask yourself: would you be willing to pay for a neighborhood lower fluctuation?

The least expensive option resulting from this procedure is a house with ID 15796 in Rainier Beach with 5 bedrooms for 133,000 USD.


## Environment Setup
This repo contains a requirements.txt file with a list of all the packages and dependencies you will need.

Before you can start with plotly in Jupyter Lab you have to install node.js (if you haven't done it before). Check **Node version**  by run the following commands:

```sh
node -v
```

If you haven't installed it yet, begin at `step_1`. Otherwise, proceed to `step_2`.


### **`macOS`** type the following commands : 


`Step_1:` Update Homebrew and install Node by following commands:

```sh
brew update
brew install node
```

`Step_2:` Install the virtual environment and the required packages by following commands:

```BASH
pyenv local 3.11.3
python -m venv .venv
source .venv/bin/activate
pip install --upgrade pip
pip install -r requirements.txt
```
### **`WindowsOS`** type the following commands :


`Step_1:` Update Chocolatey and install Node by following commands:
```sh
choco upgrade chocolatey
choco install nodejs
```

- `Step_2:` Install the virtual environment and the required packages by following commands.

For `PowerShell` CLI :

```PowerShell
pyenv local 3.11.3
python -m venv .venv
.venv\Scripts\Activate.ps1
pip install --upgrade pip
pip install -r requirements.txt
```

For `Git-Bash` CLI :

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

