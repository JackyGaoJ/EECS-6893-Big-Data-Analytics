# EECS 6893 Group 28 Final Project

## About This Project 
// Todo
================
# Require Environment:
Make sure your time/location range is the same as New York Time

If on Windows, right click the date and time on the lower right.
Click "Adjust Date/Time".
Click "Sync now."

1. Install Anaconda Navigator
https://www.anaconda.com/products/individual


2. Build a Python 3.8 Environment
![Alt Text](gifs/Instruction_anaconda.gif)

3. Open previous built enviroment's Terminal and Install required packages
```
pip install --upgrade "ibm-watson>=5.3.0"
conda install pandas-gbq --channel conda-forge
conda install geopandas
pip install tweepy
pip install jupyter
pip install notebook
```

4. Once every package is installed, open a new environment terminal, and type ``` jupyter notebook ``` to open Jupyter Notebook

5. Open the file ```demo.ipynb```, and run each cell. When you run the cell contains:
~~~python
if __name__ == "__main__":
    main()
~~~
The system will open a webpage ```main.html```

6. Type anything to invoke the system. And follow the dialogue of our system to get recommendations!

7. You could type ```restart``` to restart the system 

