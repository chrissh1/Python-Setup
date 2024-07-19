# Python-Setup

## Installation
### Get Python
```brew install python3``` to install the latest version of python
### Use Pyenv to Manage Python Versions
Install using homebrew:
```
brew update
brew install pyenv
```
Add the path and variables to zshrc:
```
echo 'export PYENV_ROOT="$HOME/.pyenv"' >> ~/.zshrc
echo '[[ -d $PYENV_ROOT/bin ]] && export PATH="$PYENV_ROOT/bin:$PATH"' >> ~/.zshrc
echo 'eval "$(pyenv init -)"' >> ~/.zshrc
```
Update the terminal:
```
source ~/.zshrc
```
## Usage
### Set and install python versions
Check version using ```python3 -V```
Check pyenv available versions using: ```pyenv install --list```
Install the version you want using: ```pyenv install -v 3._._```
To change the versions in use: ```pyenv global 3._._```
### Check Versions
```ls ~/.pyenv/versions/``` to check available versions. Or use ```pyenv versions```
```rm -rf ~/.pyenv/versions/3._._``` to remove a versions
## VENV
To create a virtual environment, go to the project's directory and run:
```
python3 -m venv .venv
```
To run: ```source .venv/bin/activate```
To deactivate: ```deactivate```

## Use in VSCODE
Set the Python Interpretor at the top of VSCode to the venv
