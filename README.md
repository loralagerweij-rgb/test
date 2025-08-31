# Setting up a python environment

## Add a section to top of readme on how to start using the project

Do this to install dependencies:
```
sudo apt install python3.9 (or whatever python version)
python3.9 -m venv ~/venv
source ./venv/bin/activate
pip install -r requirements.txt
```

Do this to run:
```
python test.py
```

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

## Commit locally to git
```
git add README.md requirements.txt test.py
git commit -m "Initial commit message"
```


## Add git remote repository and push

```
git remote add origin git@github.com:loralagerweij-rgb/test.git
git branch -M master
git push -u origin master
```

(use 'main' instead of master, depending on how the local git repo is set up.)

# Later commits and pushes
```
git commit -am "Another commit"
git push
```

The `-a` means we add _all_ files! Only do that when that's what you intend!

## Create a virtual env for a specific python version

### Get access to specific python versions to install
```
sudo add-apt-repository ppa:deadsnakes/ppa
sudo apt update
```

### Install a specific python version on the system
```
sudo apt install python3.9
```

###
Use that specific python version to create a new virtualenv with
```
python3.9 -m venv ~/venv
```
