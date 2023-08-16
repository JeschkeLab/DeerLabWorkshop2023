# 1) Installing Python

## Windows

1. The simplest way to install Python is direct from the [Python website](https://www.python.org/downloads/windows/). Please download the windows installer for your processor type (nearly always 64bit) and the latest version 3.11.x

2. Run the installer (that you have just downloaded). Follow the install instructions. **It is important that you tick** `Add python to PATH`
3. Check the installation
    1. Open Command Prompt
    2. Run the command `python`
    3. 



## MacOS

The best way to install python on MacOS is from the offical [Python website](https://www.python.org/downloads/windows/).

## Linux


# 2) Installing packages
The easiest way to install packages is using the python package manager pip. This will install packages along with any depencies that they might have.

The latest version of deerlab can be installed with:

```
pip install deerlab
```

It is also recomended that you install jupyter. This is required for this workshop but not DeerLab.

```
pip install jupyter
```
## Checking the Install

# 3) Installing VScode or Jupyter Lab

Whilst everything above is all that is required to use DeerLab it is highly recomended that an IDE is used to program. Here there is two options:

## Option A: VScode
VScode is the most popular development enviroment in the world, with over 70% of developers using it. It is developed by Microsoft.

1. It can be installed from the [VSCode Website](https://code.visualstudio.com/)
2. Run the installer. Follow the install instructions.
3. Start VScode
4. Open your Extensions Tab. Install:
     1. Python
     2. Jupyter
3. Your python version should appear status bar at the bottom 

## Option B: Jupyter Lab
Jupyter Lab is a self-hosted web based IDE for Jupyter Notebooks.

1. It can be installed using pip
   ```
   pip install jupyter-lab
   ```
2. Start Jupyter Lab from Command Prompt
   ```
   jupyter lab
   ```
3. Navigate to the relevant folder
