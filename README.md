# housing_prediction_app
[![Build Status](https://jenkins.indigo-datacloud.eu/buildStatus/icon?job=Pipeline-as-code/DEEP-OC-org/{% if cookiecutter.git_base_url == 'https://github.com/deephdc' %}{{ cookiecutter.repo_name }}{% else -%}UC-{{ cookiecutter.git_base_url.split('/')[-1] }}-{{ cookiecutter.repo_name }}{% endif %}/test)](https://jenkins.indigo-datacloud.eu/job/Pipeline-as-code/job/DEEP-OC-org/job/{% if cookiecutter.git_base_url == 'https://github.com/deephdc' %}{{ cookiecutter.repo_name }}{% else -%}UC-{{ cookiecutter.git_base_url.split('/')[-1] }}-{{ cookiecutter.repo_name }}{% endif %}/job/test)



To launch it, first install the package then run [deepaas](https://github.com/indigo-dc/DEEPaaS):
```bash
git clone https://github.com/deephdc/housing_prediction_app
cd housing_prediction_app
pip install -e .
deepaas-run --listen-ip 0.0.0.0
```
The associated Docker container for this module can be found in https://github.com/deephdc/DEEP-OC-housing_prediction_app.

## Project structure
```
├── LICENSE                <- License file
│
├── README.md              <- The top-level README for developers using this project.
│
├── requirements.txt       <- The requirements file for reproducing the analysis environment, e.g.
│                             generated with `pip freeze > requirements.txt`
│
├── setup.py, setup.cfg    <- makes project pip installable (pip install -e .) so
│                             housing_prediction_app can be imported
│
├── housing_prediction_app    <- Source code for use in this project.
│   │
│   ├── __init__.py        <- Makes housing_prediction_app a Python module
│   │
│   └── api.py             <- Main script for the integration with DEEP API
│
└── Jenkinsfile            <- Describes basic Jenkins CI/CD pipeline
```
