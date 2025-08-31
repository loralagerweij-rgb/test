# Setting up a python environment

## Create python environment for the default python version on the system
```
 python -m venv ./venv
 ```

 ## Activate the virtual environment
 ```
 source ./venv/bin/activate
 ```

 ## Install packages
 ```
 pip install pandas
 ```

## Save installed package in requirements file
 ```
 pip freeze > requirements.txt
 ```

## Install all required packages
```
pip install -r requirements.txt
```

## Create git repository
```
git init
```

## Avoid checking in the virtual environment

Create a file '.gitignore' and list files we don't want in git.

```
echo -n "venv/" >> .gitignore
```
