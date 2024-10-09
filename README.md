# PyLabRobot Tutorials BME590

### Required software installs

[Install Python=3.11](https://www.python.org/downloads/release/python-3110/) </br>
[Install Git](https://git-scm.com/downloads)</br>


### Setting up the virtual environment and dependencies
First, set up a virtual environment to prevent conflicts with any other projects. From the terminal:
```bash
pip install virtualenv
virtualenv plr_env --python python3.11
source plr_env/bin/activate
```



### Installing PyLabRobot
From the terminal:</br>
```bash
git clone https://github.com/PyLabRobot/pylabrobot.git
cd pylabrobot
pip install -e '.[visualizer]'
pip install libusb_package
pip install websockets
cd ..
```

If you've previously installed PyLabRobot don't repeat the above, just run`cd PyLabRobot` and `git pull`.


Now, install jupyterlab and all the other dependencies. Make sure to pip install opentrons with `--no-deps`.
```bash
pip install jupyterlab
pip install pylibftdi
pip install aionotify==0.3.1
pip install pydantic==1.10.9
pip install ipykernel==6.29.3
pip install ipython==8.25.0
pip install pyserial
pip install numpy
pip install opentrons --no-deps
pip install opentrons_shared_data --no-deps
```

### Download the tutorial notebook (do this once)
```bash
git clone https://github.com/stefangolas/PyLabRobot_Tutorials_BME590.git
```


## Recommended development environment
It is recommended to use VSCode with the following extensions:
* Python
* Jupyter
* Browser Lite

[Install VSCode here](https://code.visualstudio.com/download) 

To install extensions on VSCode, click the building block icon on the left side.

To start a notebook in VSCode, 
* Open the notebook file from VSCode (File-> Open "PyLabRobot_Tutorials_BME590/...")
* In the VSCode terminal, enter your virtual environment and run jupyter lab

##  Do this every time before you start working
`source plr_env/bin/activate`
`cd pylabrobot`
`git pull`
`cd ..`
`cd PyLabRobot_Tutorials_BME590`
`git pull`
