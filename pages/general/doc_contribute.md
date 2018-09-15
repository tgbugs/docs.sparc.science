---
title: "Contributing to the documentation site"
keywords: documentation, github
sidebar: sparc_sidebar
toc: false
permalink: doc_contribute.html
summary: This document outlines how you can contribute to this website. Anyone can create a branch of this repository and add or modify any of the pages for this documentation by submitting a pull request to the master branch of the code. 
folder: general
---

## Contributing to the SPARC Documentation website
This document outlines how you can contribute to this website. This website is generated using [Jekyll](https://jekyllrb.com/) and the source-code is publically available here: [https://github.com/Blackfynn/docs.sparc.science](https://github.com/Blackfynn/docs.sparc.science)

Anyone can create a branch of this repository and add or modify any of the pages for this documentation by submitting a pull request to the master branch of the code. The DAT-Core manages the repository and will pull in any changes after they are validated.

## Workflow for adding documentation to the site
To submit a pull request with updates to the documentation site:
1. Create a your own branch from the GitHub repository. 
2. Install Jekyll on your computer if you want to locally test the updates.
3. Add, or edit pages following the guidelines below.
4. Commit your changes to your branch and push to GitHub.
5. Submit a pull request with a description of your changes.
6. The DAT-Core will merge your changes into the master branch which will update https://docs.sparc.science.

## Editing the documentation and testing the documentation locally
The SPARC documentation site is using the Jekyll Doc Theme. Full documentation for this theme is located here: [https://idratherbewriting.com/documentation-theme-jekyll/](https://idratherbewriting.com/documentation-theme-jekyll/). Follow the instructions in the link to setup Jekyll on your computer to locally test any changes that you make to the documentation site. The theme documentation also provides indepth instructions on how to make changes to the site. 

The theme is quite flexible. To keep the SPARC documentation site clean, please follow the following guidelines:
1. Only use Markdown to format your pages
2. Store pages in the 'pages' folder and create a meaningful hierarchy of folders if necessary
3. Store images in the 'images' folder
4. Do not create any new sidebars. Use the '_data/sidebars/sparc_sidebar.yml' sidebar.
5. Do not add any top-navigation.

## Questions
Contact the DAT-Core if you have any questions or suggestions. 
