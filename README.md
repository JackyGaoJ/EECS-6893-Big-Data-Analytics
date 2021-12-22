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
pip install pandas-gbq
pip install jupyter
pip install notebook
pip install fuzzywuzzy
pip install tqdm
pip install tweepy
pip install geopy
pip install textblob
```

4. Once every package is installed, open a new environment terminal, and type ``` jupyter notebook ``` to open Jupyter Notebook

5. Open the file ```main.ipynb```, and run each cell. When you run the cell contains:
~~~python
if __name__ == "__main__":
    main()
~~~
The system will open a webpage ```main.html```

6. Type anything to invoke the system. And follow the dialogue of our system to get recommendations!

7. You could type ```restart``` to restart the system 
8. All process
![Alt Text](gifs/all-process.gif)
# Some Clarification:
1. There is a limit of requests for Hotel API. We have already run out of it this month. And there is some issue about GCP BigQuery (One of our teammates's accound was blocked by Google), thus our previous uploaded data could not be accessed. So we modified our codes that user could only find hotels in zipcode 10025 and 10001.
2. Analyzing Tweets takes a long time (maybe 10 hours or longer), so we update it periodically. You could refer to Twitter folder, there is a README. We have already run it recently and stored data in .csv files so that you do not need to run it again.
3. Due to Google GCP Bigquery's slow upload, we have already uploaded much data into tables in BigQuery to save your time
