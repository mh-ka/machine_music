# Machine Music

* This is a fork of another python project to transform json data into midi that can be used as input for DAW software (like LMMS, Ableton, Fruity Loops, etc.).
* Since the API is closed for new accounts I removed the request part and added a sample json file to be read by the code in weather_to_midi_map.py
* I updated the package versions and used pipenv as package manager.
* The project uses the package rtmidi. Because of compiling errors I could not get the package compiling running on a Windows machine. On a Raspberry Pi it worked quite smooth but LMMS is not available on ARM architecture.
* I tested the weather_to_midi_map.py example and connected it to LMMS. It worked although it seems like the tones are constantly playing (maybe a configuration problem of LMMS).

# Getting Started

* Due to the explanations above it is highly recommended to use Linux or MacOS for this project.
* Clone the repository from github on your local PC (alternatively download it as a zip file and extract it into a folder on your local machine).
* Make sure "pipenv" is installed on your machine.
* (Linux-specific) Make sure the packages "libasound2-dev" and "libjack-dev" are installed
* Go into a command line and navigate to the local project folder.
* Type "pipenv shell" to create a virtual python environment.
* Type "pipenv install" to install the python packages into the virtual environment.
* If the steps were successful, type "python weather_to_midi_map.py" to start the midi channel generation. (Can be cancelled with CTRL+Z at any time).
