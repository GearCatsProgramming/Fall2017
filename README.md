# Fall2017

## Installing OpenCV and Python
We're going to use a package manager -- Miniconda -- to install everything, because it streamlines things and makes it easier to keep track of the versions of stuff. 

0. You're allowed to keep or get rid of the python stuff you downloaded last week - sorry! 

1. Download miniconda here: https://conda.io/miniconda.html. We want the Python 3.6 installer, for your operating system. 

 1a. If you're on a PC, run the .exe file. 
 1b. If you're on a Mac, open Terminal. Run `cd Downloads/`, which will get you into the downloads folder. Then run `bash Miniconda3-latest-MacOSX-x86_64.sh` to get Miniconda installed. 
  
  1c. Generally, you can go by the defaults. If it asks you whether you want to add Miniconda3 to your PATH, this is up to you; if you say yes, your system will default to 3.6 instead of 2.7, but this isn't likely to cause any issues because most things support both versions these days. If you say no, you'll just have a bit more work when launching Python in the future. 
  
2. If you're on Mac, restart the terminal; on PC, open your terminal. Then type `conda info` to make sure everything is working. 

3. Now we're going to be good and follow best practices and create a new python environment so we have a sandbox to play in without getting other stuff messy. Run `conda create -n frc2017env python=3.5`. You can replace the "frc2017env" bit with another environment name if you want to - if so, keep track of the name you use, or at least make it descriptive. Once that command finishes, run `source activate frc2017env`, or whatever environment name you used. 

4. Now your prompt should say you're in your new environment. Check whether it says the name - if not, this is a good time to stop and debug. 

5. Now we're going to install some helpful libraries. Run `conda install numpy scipy matplotlib` to install NumPy, SciPy and Matplotlib. If it asks any questions that say `[y]/n`, type `y` for yes. 

6. Run `spyder` to open the IDE that comes with Miniconda. In the IDE, type 
```import numpy
import scipy
import matplotlib
```
and run the code. If there aren't any errors, we're good! If there are, time to debug. 

7. Time for OpenCV! Run `conda install -c menpo opencv3`. Again, follow the prompts till it's installed. 
