# Biocartis Technical Exercise

Data science project to classify qPCR Amplification curves.

`Data` folder contains:
- Trainingset.csv: dataset contains 1000 training examples, each row = 1 record.
  
  Columns: 
  - Id
  - 7 features derived from the PCR curve (together these features characterize a curve)
  - Truth value for the curve: “CurveCall” if True, this curve represents a mutation, if False, it does not

- Validationset.csv: 100 samples on which you can validate the model.

## Setup
Run `poetry install`

## Development

- Format:
  - Black to standardise formatting: `poetry run black .` 
  - isort to standardise import order: `poetry run isort .`
- Lint: 
  - Use flake8 to adhere to PEP 8: `poetry run flake8`

## Data science project
Run `poetry run jupyter lab`
