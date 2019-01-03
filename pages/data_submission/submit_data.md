---
title: "SPARC Data curation steps"
keywords: documentation, github
sidebar: sparc_sidebar
permalink: submit_data.html
summary: This pages outlines the workflow for submitting data to the SPARC DAT-Core. 
folder: general
---

## Steps for publishing data in DAT-Core

{% include image.html file="sparc_workflow.png" alt="workflow" %}

Inveistgators will have 1 year from the time a milestone is completed to publish the resulting dataset (step 4). A data set is published when it is available for viewing and download by the public and has been assigned a digital object identifier (DOI). During that year, the data set will move through several stages, characterized by access rights and curatorial actions. Investigators will have 30 days from the completion of the milestone to formally submit their data to the SPARC Data Repository (DAT-CORE).  Submission of data is defined as sharing data with the curation team (step 2 above).  

### Creating a draft dataset
**Timeline:** At any time, users can create a draft dataset within the SPARC Consortium organization in preparation for submitting the data to SPARC DAT-CORE. 

**Who has access to the data:** Draft data is private and is accessible only to those that you specifically invite to access the data. Neither Blackfynn, the curation team nor NIH can access the data unless you invite them.

**Who owns the data:** The investigator that submitted the data or the person who is assigned as the owner of the dataset.

**Process:**  During this step, investigators upload a data set that represents the completion of a milestone according to the standards esablished by SPARC. 

A dataset is defined as follows: The set of data files, supporting documents and metadata produced as the result of completing a milestone.  At time of submission, the  dataset may be considered complete, that is no new data will will be collected, or it may represent a batch or slice of data that is part of a larger data set being collected over several milestones. 

You may choose to use some of the SPARC data repository features for organizing your data; however, the data and metadata standards established by SPARC, as outlined below, must be followed before the dataset is submitted for curation.

**Steps for creating a draft dataset:**
- Create and name a dataset in the SPARC data repository
- Provide a short description for the dataset
- Upload files and organize the dataset according to the requirements of the SPARC Data Standards Committee and Data Curation Team.
- Share the data with the curation team and NIH

**SPARC dataset requirements** Each dataset will comprise the following:
- A protocol that has been [submitted to Protocols.io](https://docs.google.com/presentation/d/1WhoLvOVRIbCzu3x30Dd0O1cC09ZGT4g0IFOf4Eq7yfI/edit#slide=id.p) as part of the SPARC group
- Data files organized in folders according to [SPARC guidelines](https://docs.google.com/presentation/d/1EQPn1FmANpPsFt3CguU-JOQVMMlJsNXluQAK_gb2qVg/edit#slide=id.p1).  The SPARC Dataset Structure may be [downloaded as a zip file](https://drive.google.com/open?id=1mtZ5sL1lYcA2zHVsrYOKVeH2X-VlJT6P) or you may create them on your own. For help with working with the SPARC Dataset Structure, which is based on the [BIDS specification](http://bids.neuroimaging.io/), contact **sparc@neuinfo.org**.
- Metadata files and documentation organized according to the SPARC Dataset Structure.  Templates are provided in the zip file (docs file) and include the following:
  - [Submission metadata](https://drive.google.com/open?id=1OhXmssY9GK8ebOmrvib1B9xbeqoVEOBA)
  - [Dataset description for publication](https://drive.google.com/file/d/1-VqBo63oKlxVdt8nNnbzVK0NxAHwc8-L/view?usp=sharing)
  - A representative figure that will be made published along with the descriptive metadata
  - Experimental metadata specified by the SPARC Data Standards Committee based on the Minimal Information for a Neuroscience Dataset (MINDS) specification.  MINDs metadata fields have been incorporated into the [subjects](https://drive.google.com/open?id=1IDo5INrqtIu1sTJW2mICzuGEAKqv5eGg) and [samples](https://drive.google.com/open?id=1ROCsuBjMWBDmCTpTGZsUQDDgYtm-nqYG) templates available in the zip file.  An annotated list of these fields can be found [here](https://docs.google.com/spreadsheets/d/1e61r3F2weausmBhqFK8RlYLviC3rya44so5m15mPRTw/edit#gid=108617967).

### Submit dataset to Data Curation Team
**Timeline:** A dataset is considered submitted, once it has been shared with the Data Curation Team.  Dataset submission is required within 30 days of completing a project milestone (according to the SPARC Material Sharing Policy)

**Who has access to the data:** The data is accessible to you and designated individuals, as well as the data curation team and NIH. 

**Who owns the data:** The investigator that submitted the data or the person who is assigned as the owner of the dataset, but the curation team will have write permission to harmonize the metadata and file structure as needed.

**Process:** The Data Curation Team will work with the investigators to curate the dataset. Curation includes capturing the metadata, mapping it to the standardized models developed by the SPARC Data Standards Committee, and integrating it into the SPARC Integrated Dataset.

**Required steps for the data owner:**
- Share the dataset with the SPARC Data Curation team on the DAT-Core platform
- Work with the curation team to implement required curation

### Release data to the SPARC consortium
**Timeline:** As soon as the curation process has been completed, the investigator is expected to release the data under embargo to the SPARC consortium.

**Who has access to the data:** The data is now shared with all members of the SPARC Embargoed Data team who have signed the CDA. A segment of the metadata (as defined by the SPARC Data Sharing Committee) will be available to the public at this time. SPARC members who have signed the CDA will be able to access the full metadata and request access to the data files, by permission of the ownder.

**Who owns the data:** Data sets that are released are owned by the individual investigator for the purposes of provided access upon request.  However, data sets under embargo are read only, as they are now available for others in the SPARC consortium to reuse.   

**Process:** The dataset is now considered to be an embargoed dataset and will be assigned a provisional DOI by the DAT-CORE so that it can be referenced in any manuscripts in preparation. Embargoed datasets are “read-only” access to all members of the SPARC Consortium organization who have signed the CDA. If any modifications to the data or metadata are required, e.g., an error is detected, changes must be made by the administrator and a new version must be released that documents the change from the original.    

**Required steps for the data owner:**
- The owner will need to change the ‘sharing’ setting to include the **SPARC Embargoed Data Sharing Group** with read-only priviledges.

### Publishing submitted dataset into public domain 
**Timeline:** Within one year of the completion of the milestone, or at the time of online publication of a paper using the dataset, whichever comes first, the data will be released to the public portal and assigned an open license in accordance with the SPARC Data Sharing policy.

**Who has access to the data:** The dataset is now publicly available in accordance to the terms of the license chosen.

**Who owns the data:** The investigator that submitted the data or the person who is assigned as the owner of the dataset.  The owner will have provided proper citation metadata so that the reuse of the data can be appropriately credited.

**Process:** When datasets are shared publicly, the data will receive a digital object identifier (DOI), which can be used to reference the data in publications.

**Required steps for the data owner:**
- The data set will be automatically published at one year post milestone, if not published earlier by the investigator, e.g., as part of a publication or because s/he wants to.  The Open Data Library is a public facing web application to make available and distribute public datasets on the Blackfynn platform. It is slated for development in 2019. 


##  Schematic representation of SPARC Data on the DAT-Core

The figure below is a schematic representation of the workflow described above. It highlights how data is generated by individual investigators, is curated by the curation team, and shared as an embargoed dataset with the **SPARC Embargoed Data Sharing Group** . It shows how the data is made available to the public over time, and how the Integrated Dataset intersects with the individual datasets created by the investigators.

{% include image.html file="dat_core_diagram.png" alt="workflow" %}
