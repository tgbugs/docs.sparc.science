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
All files belong to a dataset on the DAT-Core platform. A dataset contains both files and metadata and can be selectively shared with other users of the platform. You can create datasets through the web application or using one of the [client tools](https://developer.blackfynn.io). Click [here](https://help.blackfynn.com/en/articles/1489153) to see more detailed information on how to create datasets on the DAT-Core platform.

## Step 2: Uploading files
Once you have created a dataset, you can upload files to this dataset. You can create folders to separate files in a logical structure. After files are uploaded, you can associate files with metadata records. There are number of ways to upload files:

### Upload files using the browser
Within a dataset, you can navigate to the 'Files' tab. This is the main location where all files are organized. 

{% include image.html file="dat_core_file_tab.png" alt="file upload" %}

In the 'Files' tab, you can create folders to organize your files on the platform. Click on the "New Folder" button to create a new folder. You can navigate into a folder by clicking on the folder in the file browser.

To upload files, you can drag files from your local machine directly into the file browser panel. A popup window will show the files that will be uploaded. Note that two of the files in the example below are combined as they belong to the same timeseries package.

{% include image.html file="dat_core_upload_modal.png" alt="file upload" %}

Click 'Start Upload' to begin uploading the files. During the upload process, you can safely hide the popup window as files will continue to be uploaded in the background. Once files are uploaded to the platform, they will show up in the file browser. If you drag a folder into the upload window, all nested folders will also be uploaded and the folder hierarchy will be maintained on the platform.

Depending on the file format, the platform will process the data to enable the data to be viewed in the browser based data viewer. Processing of the data can take a while and you will be notified when this has completed.

For more information, see the [File Upload Documentation for Blackfynn](https://help.blackfynn.com/en/articles/2539046) 

### Upload folders/files using the Blackfynn CLI.
Blackfynn provides a Command Line Interface that can be used for uploading both small and very large datasets. Detailed information can be found here:

[Uploading files with the Blackfynn CLI](https://developer.blackfynn.io/agent/agent_tutorial2.html)

### Upload files using Python
You can use the Open Source Blackfynn Python Library to upload files to the DAT-Core platform.  In Python, you will first need to import the library and establish a connection to the platform. Then retrieve or create a dataset. The dataset object has a method to upload files to the dataset as the following example highlights. Note that uploading large files is currently not supported for Python, please use the Blackfynn Agent to programmatically upload large files. The Python client will rely on the Agent for uploading files in future releases.

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


## SODA: Software for Organizing Data Automatically

The idea for SODA emanated during the December 2018 SPARC Hackathon. It is a software intended to simplify the organization and submission process of SPARC datasets by handling complex and/or repetitive tasks through an intuitive and interactive interface. With SODA, users will be able to organize, generate metadata, validate, and submit datasets according to the SPARC Data Standards. SODA will be distributed as a desktop application for Windows, MAC OS, and Linux. It is currently under development and will be released progressively as features are incorporated. In October 2019, SODA will assist users in organizing their files/folders automatically, generating their metadata conveniently, and submitting their datasets to Blackfynn. In December 2019, users will be able to push and organize files/folders of a dataset directly on Blackfynn thus avoiding the need to create duplicate files locally. In February 2020, it will be possible to validate datasets using the validator developed by the Curation Team. In April 2020, users will be able to manipulate and annotate datasets on Blackfynn. In May 2020, SODA will permit to rapidly convert file format into a SPARC-defined standard format.

For more information please contact [Bhavesh Patel](mailto:bpatel@calmi2.org).