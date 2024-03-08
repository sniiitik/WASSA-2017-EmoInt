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

