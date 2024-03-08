#WASSA-2017

Task: Given a tweet and an emotion X, determine the intensity or degree of emotion X felt by the speaker -- a real-valued score between 0 and 1. The maximum possible score 1 stands for feeling the maximum amount of emotion X (or having a mental state maximally inclined towards feeling emotion X). The minimum possible score 0 stands for feeling the least amount of emotion X (or having a mental state maximally away from feeling emotion X). The tweet along with the emotion X will be referred to as an instance. Note that the absolute scores have no inherent meaning -- they are used only as a means to convey that the instances with higher scores correspond to a greater degree of emotion X than instances with lower scores.

# Introduction
instructions on how to run the code conveniently using Google Colab with Google Drive and Github

### Google Colab
It’s a Jupyter notebook environment that requires no setup to use.
Moreover it gives you **free GPU** access to run your code.
Open Google Collab on your Browser

Then connect to the enviornment 

Download the Provided Dataset and upload on your Google Drive or in Local System

#### Accessing data on Google Drive
Code below mounts your Google Drive to 
`/content/drive/My Drive` directory.

In case `google.cloab` is not found it assumes that the notebook runs somewhere else and it doesn't mount the drive.
```python
try:
    from google.colab import drive
    drive.mount("/content/drive/", force_remount=True)
    google_drive_prefix = "/content/drive/My Drive"
    data_prefix = "{}/mnist/".format(google_drive_prefix)
except ModuleNotFoundError: 
    data_prefix = "data/"
```

Once you're done with accessing the Data on your notebook Simply Run the cells one by one (ensuring each cell to run smoothly)

