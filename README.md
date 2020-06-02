# gitmanager
Console tool for manage projects on github/gitlab

## Installation

    'pip install gitmanager'


## Usage

Go to your project folder and execute the new gm command.
First time ask for link of your repo, for example: https://github.com/katmai1/gitmanager


## Developer section

For install the develop version go to source folder and execute:
    'pip install -e'

### Create new version

Update version number on file [setup.py](setup.py)

git commit all changes

git tag 0.1 -m "tag description"

git push --tags origin master

Build package:

    python setup.py sdist bdist_wheel

Upload 
    
    twine upload -r pypi --skip-existing dist/*
