---
title: "Overview of SPARC Dataset Format"
keywords: documentation, github
sidebar: sparc_sidebar
permalink: sparc_data_format.html
summary: This page provides an overview of the SPARC data format.
folder: general
---

## Organization of a SPARC Dataset
SPARC data is organized into data sets, each containing many files.  A SPARC data set comprises the following data and structure:
- An experimental protocol that has been [submitted to Protocols.io](http://protocols.io) and curated.
- Data files organized in folders by the investigators and curated according to the [SPARC Dataset Structure](https://docs.google.com/presentation/d/1EQPn1FmANpPsFt3CguU-JOQVMMlJsNXluQAK_gb2qVg/edit#slide=id.p1).  The SPARC Dataset Structure was adapted from the [BIDS specification](https://bids-specification.readthedocs.io/en/latest/01-introduction.html). These files and folders include:
  - Dataset_description (csv): file contains the study metadata to describe the dataset, including but not limited to, a short description of the study, contributors, associated journal articles and a protocol.io URL. 
  - Sample file (csv): contains information about samples involved in the data collection.
  - Subject file (csv): contains information on every subject involved in the data collection
  - Subject and/or Sample folder, depending on the study design. These folders contain all folders and files for an individual subject or sample. 
  - Docs folder that contains all the supporting documents for the dataset, including but not limited to, a representative image.
 
### Example of data set organized according to SPARC Dataset structure
{% include image.html file="SPARC_Dataset_Overview.png" alt="Overview of SPARC Dataset" %}
 
## SPARC Metadata

Experimental metadata specified by the SPARC Data Standards Committee based on the Minimal Information for a Neuroscience Dataset (MINDS) specification.  MINDS metadata fields have been incorporated into the [subjects](https://drive.google.com/open?id=1IDo5INrqtIu1sTJW2mICzuGEAKqv5eGg) and [samples](https://drive.google.com/open?id=1ROCsuBjMWBDmCTpTGZsUQDDgYtm-nqYG) templates available in the zip file.  An annotated list of these fields can be found [here](https://docs.google.com/spreadsheets/d/1e61r3F2weausmBhqFK8RlYLviC3rya44so5m15mPRTw/edit#gid=108617967).
