---
title: "Submitting a dataset to SPARC"
keywords: documentation, github
sidebar: sparc_sidebar
permalink: submit_data.html
summary: This page outlines the steps for submitting a dataset, getting the data curated, releasing the data under embargo, and eventually making the data publicly available. 
folder: general
---

## Steps for submitting a dataset

This documentation only applies to investigators that are funded throught the NIH SPARC effort. Each investigator has user-credentials under the account *SPARC Consortium* on the DAT-Core. All datasets that are SPARC related should be submitted to this account even though the investigator might have an separate *private* Blackfynn account. Dataset submission is required within 30 days of completing a project milestone (according to the [SPARC Material Sharing Policy](https://commonfund.nih.gov/sparc/materialsharing)). {% include image.html file="sparc_workflow.png" alt="workflow" %}


### 1. Creating a draft dataset
There are a couple of easy steps to submit a dataset:

1. Create a dataset on the DAT-Core (*SPARC Consortium* account on Blackfynn) by clicking the `New Dataset` button in the top-right corner of the webapplication and provide a **Dataset Name** and a short **Dataset Subtitle** describing the dataset. Then, click on `Create Dataset`. {% include image.html file="dataset_list_datcore.png" alt="workflow" %} You now created a *private* dataset that only you, as the dataset owner, can see.

2. Change the ownership of the dataset to the PI of the lab. This is a SPARC requirement and ensures that the PI is the only person who can publish the dataset. To do this, click on the `Permissions` tab, and add the PI to your dataset as a *manager*. Then click on the `manager` label next to his/her name and select `Make Owner`. You will no longer be the owner of the dataset, but still have *manager* permissions. {% include image.html file="dataset_permissions.png" alt="workflow" %}

3. Add permissions to your **Award team** (contact the DAT-Core if you need help adding people to your award team) and the **Curation team**. Select your award-team from the dropdown menu, and add with the appropriate permissions, and add the *SPARC Data Curation Team* with *manager* permissions. {% include image.html file="dat_core_permissions2.png" alt="workflow" %} You have now allowed your award-team and the curation team to see, and edit the dataset.

4. Upload files to the dataset according to the [SPARC guidelines](https://docs.google.com/presentation/d/1EQPn1FmANpPsFt3CguU-JOQVMMlJsNXluQAK_gb2qVg/edit#slide=id.p1).  The SPARC Dataset Structure (version 1.2.3) may be [downloaded as a zip file](https://github.com/SciCrunch/sparc-curation/releases/tag/dataset-template-1.2.3) or you may create it on your own. For help with working with the SPARC Dataset Structure, which is based on the [BIDS specification](http://bids.neuroimaging.io/), contact **sparc@neuinfo.org**. More information on how to upload files can be found [here](file_upload_dat_core.html) {% include image.html file="dat_core_files.png" alt="workflow" %}Complete the metadata templates that are included in the downloadad *SPARC Dataset Structure* zip-file. Experimental metadata specified by the SPARC Data Standards Committee based on the Minimal Information for a Neuroscience Dataset (MINDS) specification and are captured in the following files: 1) submission.xlsx, 2) dataset_description.xlsx, 3) subjects.xlsx, and 4) samples.xlsx. An annotated list of these fields can be found [here](https://docs.google.com/spreadsheets/d/1e61r3F2weausmBhqFK8RlYLviC3rya44so5m15mPRTw/edit#gid=108617967).

5. Provide a detailed description of your dataset using the description editor on the DAT-Core. This description will be highly visible once your dataset is published. {% include image.html file="description_dataset_datcore.png" alt="workflow" %} 

6. Add a nice banner image that will be associated with the dataset and will be visisble once the dataset is published. Click on the `Upload Banner Image` in the `Settings` or `Overview` page. {% include image.html file="banner_dataset.png" alt="workflow" %} 

7. Select a license that you want to associate with the dataset once published. Click on the `license` dropdown menu in the `Dataset Settings` page. {% include image.html file="license_datcore.png" alt="workflow" %} 

8. Finally, you will need to submit a protocol to [Protocols.io](https://docs.google.com/presentation/d/1WhoLvOVRIbCzu3x30Dd0O1cC09ZGT4g0IFOf4Eq7yfI/edit#slide=id.p) as part of the SPARC group. 

**NOTE:** There are other things that need to be entered into the DAT-Core before a dataset can be published such as: 1) the contributors, and 2) a list of tags. However, the curation team will help with adding these to the dataset from the CSV templates that you will provide as part of the uploaded files.

**NOTE:** You are free to add additional metadata in the [DAT-Core Metadata database](https://help.blackfynn.com/en/collections/1941429). If you do this, **do not** use the following model names: 1) Term, 2) Subject, 3) Protocol, 4) Researcher, 5) Summary, or 6) Sample as these will be overritten by the SPARC curation process. 


### 2. Placing your data in Embargo
Now that you have created a dataset and you are ready for the data curation to help with further curation and validation of the data, you need to share your data with the rest of the consortium.

1. Add the **SPARC Embargoed Data Sharing Team** to your dataset with **viewer** permissions. This allows any SPARC investigator who has signed the SPARC Non-disclosure form to see your data. {% include image.html file="embargoe_datcore.png" alt="workflow" %} 

### 3. Publishing your dataset
When the dataset is ready to be published, the dataset owner can publish the dataset and make it publicly available. There are two steps required for dataset publication: 1) Protocol publication on Protocols.io, and 2) Dataset Publication on the DAT-Core.


1. Make your protocol public on Protocols.io
The first step to making your data public is to make sure your protocols are made public on [Protocols.io](https://protocols.io). Perform the following steps:

    1. Log into protocols.io, and publish your dataset’s protocol(s) by clicking the orange PUBLISH button.{% include image.html file="protocols_ss.png" alt="protocol" %}

    2. Get a DOI for your protocol by clicking the orange GET DOI button.

    3. Give the curators a couple days to update your protocol URL to the DOI in your dataset_description file, or go ahead and do it yourself.  To do it yourself, update the URL(s) to your protocol(s) by editing the Blackfynn "Protocol" metadata record.

    3. Update the *protocol* record(s) in the DAT-Core to correctly store the newly generated DOI. To do this, click on the `Records` tab in the dataset, and select the `protocol` model if this exist. Then, click on the protocol that you want to update and click the `edit` button. Update the `URL` field with the correct DOI URL anc click on `Save`. {% include image.html file="model_records.png" alt="protocol" %}

    4. Upon receiving confirmation from the curation team that your dataset has been fully curated and is ready to publish, continue to the steps below.


2. Make your dataset public on the DAT-Core
Publishing your Blackfynn datasets will make your data publicly available for the world to see. The dataset will be findable and accessible on [Blackfynn Discover](https://discover.blackfynn.com) and the [SPARC Portal](https://data.sparc.science).

    1. Make sure the following information is correct for the dataset:

        - Dataset Title
        - Dataset SubTitle
        - Dataset Describtion
        - Dataset Contributors
        - Dataset Tags
        - Dataset License (must select **CC-BY license**, per SPARC policy)
        - The Banner Image (.jpg or .png)
        - The URLS in the *Protocol* records.

    2. Go to the *Settings* tab for the dataset on the DAT-Core.

    3. Have the owner of the dataset click on `Publish to Blackfynn Discover` button. It is required for the owner to have an [ORCID ID](https://orcid.org/) associated with their user-profile. Publishing a dataset will automatically request a Data Object Identifier (DOI) through [DataCite](https://datacite.org/) if you had not reserved one before. You can always publish an updated version of the dataset if needed at a later time, or un-publish a dataset if needed. {% include image.html file="publish_to_discover.png" alt="discover" %}

## Summary
This document outlined the steps required to submit and publish a SPARC dataset. Please feel free to reach out to the DAT-Core or Curation team with specific questions about the workflow. 


