# How to maintain different python versions

- Assuming your current ubuntu has python 3.10 installed and you
- want to install python 3.9
```bash
# Install the 'software-properties-common to add external repositories to your package manager's list of available sources.
sudo apt-get install software-properties-common

# Add the deadsnakes repository
sudo add-apt-repository ppa:deadsnakes/ppa

# Update package lists
sudo apt update

# Install Python 3.9
sudo apt install python3.9
```

- Install the venv package and create a venv virtual environment
```bash
# Install the venv package for Python 3.9
sudo apt install python3.9-venv

# Create your project folder and cd into the folder 
mkdir /home/project

# Create a new venv virtual environment (name: myproject) with Python 3.9 in it
python3.9 -m venv myproject

# Activate the new venv
source myproject/bin/activate

# In the virtual environment, verify that your python version is 3.9
python3
