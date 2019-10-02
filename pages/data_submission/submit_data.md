---
title: "SPARC Data curation steps"
keywords: documentation, github
sidebar: sparc_sidebar
permalink: submit_data.html
summary: This page outlines the workflow for submitting data to the SPARC DAT-Core, getting the data curated, released under embargo, and eventually making the data public. 
folder: general
---

## Steps for publishing data in DAT-Core

{% include image.html file="sparc_workflow.png" alt="workflow" %}


Investigators will have 1 year from the time a milestone is completed to publish the resulting dataset (step 4). A dataset is published when it is available for viewing and download by the public and has been assigned a digital object identifier (DOI). During that year, the dataset will move through several stages, characterized by access rights and curatorial actions. Investigators will have 30 days from the completion of the milestone to formally submit their data to the SPARC Data Repository (DAT-CORE).  Submission of data is defined as sharing data with the Data Curation Team (step 2).

### 1. Creating a draft dataset
**Timeline:** At any time, users can create a draft dataset within the SPARC Consortium organization in preparation for submitting the dataset.

**Who has access to the data:** Draft data is private and is accessible only to those who you specifically invite to access the data. Neither Blackfynn, the Curation Team, nor NIH can access the data unless you invite them.

**Who owns the data:** The investigator that submitted the data or the person who is assigned as the owner of the dataset.

**Process:** During this step, investigators upload a dataset that represents the completion of a milestone according to the standards esablished by SPARC.

A dataset is defined as follows: The set of data files, supporting documents, and metadata produced as the result of completing a milestone.  At time of submission, the  dataset may be considered complete (that is, no new data will will be collected), or it may represent a batch or slice of data that is part of a larger dataset being collected over several milestones. 

The data and metadata standards established by SPARC, as outlined below, must be followed before the dataset is submitted for curation.

**Steps for creating a draft dataset:**
- Create and name a dataset in the SPARC Data Repository (within the **SPARC Consortium Organization** on Blackfynn)
- Provide a short description for the dataset
- Upload files and organize the dataset according to the requirements of the SPARC Data Standards Committee and Data Curation Team (see below). For many users the easiest method is to drag the parent folder of the BIDS folder hierarchy into the DAT-Core platform. All files will be uploaded and the folder structure will be maintained.
- Share the data with the curation team and NIH

**SPARC dataset requirements** Each dataset will comprise the following:
- A protocol that has been [submitted to Protocols.io](https://docs.google.com/presentation/d/1WhoLvOVRIbCzu3x30Dd0O1cC09ZGT4g0IFOf4Eq7yfI/edit#slide=id.p) as part of the SPARC group
- Data files organized in folders according to [SPARC guidelines](https://docs.google.com/presentation/d/1EQPn1FmANpPsFt3CguU-JOQVMMlJsNXluQAK_gb2qVg/edit#slide=id.p1).  The SPARC Dataset Structure (version 1.2.1) may be [downloaded as a zip file](https://github.com/SciCrunch/sparc-curation/releases/tag/dataset-template-1.2.1) or you may create it on your own. For help with working with the SPARC Dataset Structure, which is based on the [BIDS specification](http://bids.neuroimaging.io/), contact **sparc@neuinfo.org**.
- Metadata files and documentation organized according to the SPARC Dataset Structure.  Templates are provided in the zip file (docs file) and include the following:
  - [Submission metadata](https://github.com/SciCrunch/sparc-curation/blob/dataset-template-1.2.1/resources/DatasetTemplate/submission.xlsx)
  - [Dataset description for publication](https://github.com/SciCrunch/sparc-curation/blob/dataset-template-1.2.1/resources/DatasetTemplate/dataset_description.xlsx)
  - A representative figure that will be published along with the descriptive metadata
  - Experimental metadata specified by the SPARC Data Standards Committee based on the Minimal Information for a Neuroscience Dataset (MINDS) specification.  MINDS metadata fields have been incorporated into the [subjects](https://github.com/SciCrunch/sparc-curation/blob/dataset-template-1.2.1/resources/DatasetTemplate/subjects.xlsx) and [samples](https://github.com/SciCrunch/sparc-curation/blob/dataset-template-1.2.1/resources/DatasetTemplate/samples.xlsx) templates available in the zip file.  An annotated list of these fields can be found [here](https://docs.google.com/spreadsheets/d/1e61r3F2weausmBhqFK8RlYLviC3rya44so5m15mPRTw/edit#gid=108617967).

### 2. Submit dataset to Data Curation Team
**Timeline:** A dataset is considered submitted once it has been shared with the Data Curation Team.  Dataset submission is required within 30 days of completing a project milestone (according to the [SPARC Material Sharing Policy](https://commonfund.nih.gov/sparc/materialsharing)).

**Who has access to the data:** The data is accessible to you and designated individuals, as well as the Data Curation Team and NIH. 

**Who owns the data:** The investigator that submitted the data or the person who is assigned as the owner of the dataset, but the Curation Team will have write permission to harmonize the metadata and file structure as needed.

**Process:** The Data Curation Team will work with the investigators to curate the dataset. Curation includes capturing the metadata, mapping it to the standardized metadata models developed by the SPARC Data Standards Committee, and integrating it into the SPARC Integrated Dataset (a master dataset that incorporates all SPARC data that has been curated).

**Required steps for the data owner:**
- Share the dataset with the SPARC Data Curation Team on the DAT-Core platform
- Work with the Curation Team to implement required curation

### 3. Release data to the SPARC consortium
**Timeline:** As soon as the curation process has been completed, the investigator is expected to release the data under embargo to the SPARC Consortium.

**Who has access to the data:** The data is now shared with all members of the SPARC Embargoed Data Sharing Group team who have signed the CDA. A segment of the metadata (as defined by the SPARC Data Sharing Committee) will be available to the public at this time. SPARC members who have signed the CDA will be able to access the full metadata and request access to the data files, by permission of the ownder.

**Who owns the data:** Datasets that are released are owned by the individual investigator for the purpose of providing access upon request.  However, datasets under embargo are read only, as they are now available for others in the SPARC Consortium to reuse.   

**Process:** The dataset is now considered to be an embargoed dataset and will be assigned a provisional DOI by the DAT-CORE so that it can be referenced in any manuscripts in preparation. Embargoed datasets are “read-only” access to all members of the **SPARC Embargoed Data Sharing Group**. If any modifications to the data or metadata are required, e.g., an error is detected, changes must be made by the administrator and a new version must be released that documents the change from the original.    

**Required steps for the data owner:**
- The owner will need to change the ‘sharing’ setting to include the **SPARC Embargoed Data Sharing Group** with read-only privileges.

### 4. Publishing submitted dataset into public domain 
**Timeline:** Within one year of the completion of the milestone, or at the time of online publication of a paper using the dataset, whichever comes first, the data will be released to the public portal and assigned an open license in accordance with the SPARC Data Sharing policy.

**Who has access to the data:** The dataset is now publicly available in accordance to the terms of the license chosen.

**Who owns the data:** The investigator that submitted the data or the person who is assigned as the owner of the dataset.  The owner will have provided proper citation metadata so that the reuse of the data can be appropriately credited.

**Process:** The publishing steps are outlined in the [Publishing Data Steps](publish_data.html) page.

**Required steps for the data owner:**
- The dataset will be automatically published at one year post milestone, if not published earlier by the investigator, e.g., as part of a publication or because s/he wants to.


##  Schematic representation of SPARC Data on the DAT-Core

The figure below is a schematic representation of the workflow described above. It highlights how data is generated by individual investigators, curated by the Data Curation Team, and shared as an embargoed dataset with the **SPARC Embargoed Data Sharing Group**. It shows how the data is made available to the public over time.

{% include image.html file="SPARC_Submission_and_Publishing_Workflow.png" alt="workflow" %}
