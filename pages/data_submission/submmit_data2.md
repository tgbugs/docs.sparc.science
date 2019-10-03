---
title: "Submitting a dataset to SPARC"
keywords: documentation, github
sidebar: sparc_sidebar
permalink: submit_data2.html
summary: This page outlines the workflow for submitting a dataset, getting the data curated, releasing the data under embargo, and eventually making the data publicly available. 
folder: general
---

## Steps for submitting a dataset

{% include image.html file="sparc_workflow.png" alt="workflow" %}
Dataset submission is required within 30 days of completing a project milestone (according to the [SPARC Material Sharing Policy](https://commonfund.nih.gov/sparc/materialsharing)).

### 1. Creating a draft dataset
There are a couple of easy steps to submit a dataset:

1. Create a dataset on the DAT-Core by clicking the `New Dataset` button in the top-right corner of the DAT-Core webapplication and provide a **Dataset Name** and a short **Dataset Subtitle** describing the dataset. Then, click on `Create Dataset`. {% include image.html file="dataset_list_datcore.png" alt="workflow" %} You now created a *private* dataset that only you, as the dataset owner, can see.

2. Change the ownership of the dataset to the PI of the lab. This is a SPARC requirement and ensures that the PI is the only person who can publish the dataset. To do this, click on the `Permissions` tab, and add the PI to your dataset as a *manager*. Then click on the `manager` label next to his/her name and select `Make Owner`. You will no longer be the owner of the dataset, but still have *manager* permissions. {% include image.html file="dataset_permissions.png" alt="workflow" %}

3. Add permissions to your **Award team** (contact the DAT-Core if you need help adding people to your award team) and the **Curation team**. Select your award-team from the dropdown menu, and add with the appropriate permissions, and add the *SPARC Data Curation Team* with *manager* permissions. {% include image.html file="dat_core_permissions2.png" alt="workflow" %} You have now allowed your award-team and the curation team to see, and edit the dataset.

4. Upload files to the dataset according to the [SPARC guidelines](https://docs.google.com/presentation/d/1EQPn1FmANpPsFt3CguU-JOQVMMlJsNXluQAK_gb2qVg/edit#slide=id.p1).  The SPARC Dataset Structure (version 1.2) may be [downloaded as a zip file](https://github.com/SciCrunch/sparc-curation/releases/tag/dataset-template-1.2.1) or you may create it on your own. For help with working with the SPARC Dataset Structure, which is based on the [BIDS specification](http://bids.neuroimaging.io/), contact **sparc@neuinfo.org**. More information on how to upload files can be found [here](file_upload_dat_core.html) {% include image.html file="dat_core_files.png" alt="workflow" %}

5. Create metadata Excel files according to the SPARC standard. 
  - Metadata files and documentation organized according to the SPARC Dataset Structure.  Templates are provided in the zip file (docs file) and include the following:
  - [Submission metadata](https://github.com/SciCrunch/sparc-curation/blob/dataset-template-1.1/resources/DatasetTemplate/submission.xlsx)
  - [Dataset description for publication](https://github.com/SciCrunch/sparc-curation/blob/dataset-template-1.1/resources/DatasetTemplate/dataset_description.xlsx)
  - Experimental metadata specified by the SPARC Data Standards Committee based on the Minimal Information for a Neuroscience Dataset (MINDS) specification.  MINDS metadata fields have been incorporated into the [subjects](https://github.com/SciCrunch/sparc-curation/blob/dataset-template-1.1/resources/DatasetTemplate/subjects.xlsx) and [samples](https://github.com/SciCrunch/sparc-curation/blob/dataset-template-1.1/resources/DatasetTemplate/samples.xlsx) templates available in the zip file.  An annotated list of these fields can be found [here](https://docs.google.com/spreadsheets/d/1e61r3F2weausmBhqFK8RlYLviC3rya44so5m15mPRTw/edit#gid=108617967).

6. Provide a detailed description of your dataset using the description editor on the DAT-Core. This description will be highly visible once your dataset is published. {% include image.html file="description_dataset_datcore.png" alt="workflow" %} 

7. Add a nice banner image that will be associated with the dataset and will be visisble once the dataset is published. Click on the `Upload Banner Image` in the `Settings` or `Overview` page. {% include image.html file="banner_dataset.png" alt="workflow" %} 

8. Select a license that you want to associate with the dataset once published. Click on the `license` dropdown menu in the `Dataset Settings` page. {% include image.html file="license_datcore.png" alt="workflow" %} 

9. Finally, you will need to submit a protocol to [Protocols.io](https://docs.google.com/presentation/d/1WhoLvOVRIbCzu3x30Dd0O1cC09ZGT4g0IFOf4Eq7yfI/edit#slide=id.p) as part of the SPARC group. 

**NOTE:** There are other things that need to be entered into the DAT-Core before a dataset can be published such as: 1) the contributors, and 2) a list of tags. However, the curation team will help with adding these to the dataset from the CSV templates that you will provide as part of the uploaded files.


### 2. Placing your data in Embargo
Now that you have created a dataset and you are ready for the data curation to help with further curation and validation of the data, you need to share your data with the rest of the consortium.

1. Add the **SPARC Embargoed Data Sharing Team** to your dataset with **viewer** permissions. This allows any SPARC investigator who has signed the SPARC Non-disclosure form to see your data. {% include image.html file="embargoe_datcore.png" alt="workflow" %} 

### 3. Publishing your dataset
When the dataset is ready to be published, the dataset owner can publish the dataset and make it publicly available. Follow the [publication steps](/publish_data.html) for more information.