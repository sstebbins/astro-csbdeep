# Astro CSBDeep – a toolbox for CARE with some tweaks

**NOTE: This is a fork of [CSBDeep](https://github.com/CSBDeep/CSBDeep). Thank you to the developers.**

This is a modified version of the CSBDeep Python package, which provides a toolbox for content-aware restoration of fluorescence microscopy images (CARE), based on deep learning via Keras and TensorFlow.

Additionally some helpful changes have been added to easily process Astrophotography images.

Please see the documentation at http://csbdeep.bioimagecomputing.com/doc/.

This fork has been modified to work with Mac OS. 

## Environment Setup

You will need a few things to get started:
1. Python 3 installed
2. If you have a mac, you should install tensorflow and tensorflow-metal EXACTLY as instructed [here](https://developer.apple.com/metal/tensorflow-plugin/). **Note the version numbers of tensorflow, tensorflow-macos, tensorflow-metal, and macOS required in the table below "Releases"!** 
3. Activate the conda or venv virtual environment created in (2).
3. Install the pip3 requirement found in the `requirements.txt` file by running `pip3 install -r requirements.txt`
4. (Optional) Install Visual Studio Code
5. Can run the GUI client by the following:
```
python astrodenoisepygui.py &
```
The above is **ALL YOU NEED** to run astrodenoisepy.  To test / play with jupyter notebooks, continue reading.

## Example Notebook For Astro

The example notebook for astrophotography `AstroNoise2Noise.ipynb` can be opened in jupyter and used to step through the process.

Further details are documented in the notebook.

In your venv start up jupiter:

```
(.venv) C:\CSBDeep> jupyter notebook
```

## Working in Visual Studio Code

Once you have you have a python venv and dependencies are installed fire up VS Code.

Note: VS Code prefers python a venv named `.venv` by default. See above for installing python requirements.

Install the following VS Code extensions:

* python (ms-python.python)
* pylance (ms-python.vscode-pylance)
* jupyter (ms-toolsai.jupyter)
* jupyter-keymap (ms-toolsai.jupyter-keymap)

Settings in the `.vscode` folder configure the default python interpreter path for the venv folder `.venv` and your default startup terminal.

Note if you dont see the the venv startup automatically in terminal just activate as above, its temperament :) 

Open up the notebook `AstroNoise2Noise.ipynb` and configure the same python interpreter path `.venv` in the top right hand of the VS Code interface.

Happy coding and clear skies!

## Contributors

Want to say a big thank you to the CSBDeep team who provided their framework along with great examples to get started.

To date, further much appreciated thanks go to contributions from:

* Michael Kitange - ongoing validation and contributions to code
* JimmyTheChicken#2719 - STF Tone Mapping Algorithm

More to come!
