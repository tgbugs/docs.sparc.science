---
title: "Uploading files to the DAT-Core"
keywords: documentation, github
sidebar: sparc_sidebar
permalink: file_upload_dat_core.html
summary: This page outlines the various ways that files can be uploaded to the DAT-Core. 
folder: general
---


## Introduction
SPARC investigators are required to upload their scientific files to the DAT-Core. There are multiple ways for users to upload files to the platform. Here, we describe the various options and provide links to tutorials describing step by step instructions to upload files.

## Step 1: Creating a dataset
All files belong to a dataset on the DAT-Core platform. A dataset contains both files and metadata and can be selectively shared with other users of the platform. You can create datasets through the web application or using one of the [client tools](https://developer.blackfynn.io). Click [here](http://help.blackfynn.com/blackfynn-web-application/importing-and-managing-data/creating-and-deleting-datasets) to see more detailed information on how to create datasets on the DAT-Core platform.

## Step 2: Uploading files
Once you have created a dataset, you can upload files to this dataset. You can create folders to separate files in a logical structure. After files are uploaded, you can associate files with metadata records. There are number of ways to upload files:

### Upload files using the browser
Within a dataset, you can navigate to the 'Files' tab. This is the main location where all files are organized. 

{% include image.html file="dat_core_file_tab.png" alt="file upload" %}

In the 'Files' tab, you can create folders to organize your files on the platform. Click on the "New Folder" button to create a new folder. You can navigate into a folder by clicking on the folder in the file browser.

To upload files, you can drag files from your local machine directly into the file browser panel. A popup window will show the files that will be uploaded. Note that two of the files in the example below are combined as they belong to the same timeseries package.

{% include image.html file="dat_core_upload_modal.png" alt="file upload" %}

Click 'Start Upload' to begin uploading the files. During the upload process, you can safely hide the popup window as files will continue to be uploaded in the background. Once files are uploaded to the platform, they will show up in the file browser. 

Depending on the file format, the platform will process the data to enable the data to be viewed in the browser based data viewer. Processing of the data can take a while and you will be notified when this has completed.

For more information, see the [File Upload Documentation for Blackfynn](http://help.blackfynn.com/blackfynn-web-application/uploading-files-to-a-dataset) 

### Upload files using the Blackfynn Agent
The Blackfynn Agent is a command line interface (CLI) that is available for Windows, Linux and Mac OS. It allows users to interact with the platform programmatically using the command line. The Blackfynn Agent is currently in Beta and will over time replace the Python based CLI. 

To upload data using the Blackfynn Agent you will have to first install the agent. After installing and configuring the tool, you can upload files using the ```upload``` command. 

```bash
./blackfynn_agent upload ~/Desktop/ --dataset {datasetId}
``` 

Tutorials on how to install and configure the agent, as well as how to upload data using the agent can be found in the [Blackfynn Developer documentation](https://developer.blackfynn.io/agent/) for the CLI.

### Upload folders/files using the Python CLI (Nested Folder Upload)
The Blackfynn Python client includes a CLI which enable users to interact with the platform from the command line. Users should [install the python client](https://developer.blackfynn.io/python/). After the client is installed, users will be able to use the ```bf``` command in the terminal to interact with the platform. Make sure to follow the python installation instructions and setup 

```bash
# Setup your profile using your API key/secret if this is the first time running the python CLI
$ bf profile create <newProfile>

# Specify which dataset should be used
$ bf use <datasetName>

# Upload a folder or file to the platform. The folder hierarchy will be maintained on the platform
$ bf upload <file/directory>

# For more information, look at the CLI help documentation
$ bf --help

``` 

### Upload files using Python
You can use the Open Source Blackfynn Python Library to upload files to the DAT-Core platform.  In Python, you will first need to import the library and establish a connection to the platform. Then retrieve or create a dataset. The dataset object has a method to upload files to the dataset as the following example highlights.

```python
 # import Blackfynn
 from blackfynn import Blackfynn

 # create a client instance
 bf = Blackfynn()

 # create a dataset
 ds = bf.create_dataset('Timeseries Dataset')

 # upload data (3 files)
 ds.upload('example_data/test.edf', 'example_data/testData.nev', 'example_data/testData.ns2')

```

More information can be found in the [Blackfynn developers documentation for Python](https://developer.blackfynn.io/python) and the sourcecode for the Python Library [here](https://github.com/blackfynn/blackfynn-python).

### Upload files using MATLAB
Finally, you can also upload files using the MATLAB client. The MATLAB client relies on the Blackfynn Agent to upload the files so you will have to both install the MATLAB client as well as the Blackfynn Agent. The ```upload``` command is a method of the ```BFDataset``` class and can be used as follows:

```R
>> bf = Blackfynn();
>> ds = bf.datasets(1)

BFDataset with properties:

    description: 'This is a dataset for the second tutorial.'
         models: [1×3 BFModel]
          items: [0×0 BFBaseDataNode]
           name: 'tutorial2'
           type: 'DataSet'

>> ds.upload('~/Downloads/example_data');
```

A detailed tutorial on how to upload data using MATLAB can be found in the [Blackfynn developers documentation for MATLAB](https://developer.blackfynn.io/matlab) and the sourcecode for the MATLAB client can be found [here](https://github.com/Blackfynn/blackfynn-matlab).



