---
title: 'Forest: A Python data analysis library for high-throughput digital phenotyping'
tags:
  - high-throughput
  - digital phenotyping
  - smartphone
  - AWS
  - Tableau
authors:
  - name: Jukka-Pekka Onnela^[Principal Investigator and corresponding author.]
    orcid: 0000-0001-6613-8668
    affiliation: 1
  - name: Authors 
    affiliation: 1
  - name: Anna Beukenhorst
    affiliation: 1
affiliations:
 - name: Department of Biostatistics, Harvard T.H. Chan School of Public Health, Harvard University
   index: 1
date: 12 February 2021
bibliography: paper.bib

---

# Summary

The phenotype of an organism is a collection of traits, such as enzyme activity, hormone levels, and behavior. Many researchers are increasingly advocating a more substantial role for large-scale phenotyping as a route to advances in the biomedical sciences. Of the many different phenotypes, social, behavioral and cognitive phenotypes have traditionally been challenging for phenomics because of their temporal nature, context dependence, and the lack of tools for measuring them objectively in naturalistic settings. Pen-and-paper surveys are still widely used to solicit these phenotypes although they suffer from well-documented biases. We have introduced the concept of digital phenotyping as the “moment-by-moment quantification of the individual-level human phenotype in situ using data from personal digital devices.” The ubiquity of smartphones presents an opportunity to capture social, behavioral, and cognitive markers in free-living settings, offering a scalable solution to the phenotyping problem.

# Statement of need

Beiwe is a data collection platform for high-throughput digital phenotyping. This open-source (BSD-3) multi-language software has been in development and use since 2013, and it consists of two native front-end applications, one for Android (written in Java) and another for iOS (written in Swift & Objective-C). The Beiwe back-end, which is based on Amazon Web Services (AWS) cloud computing infrastructure, has been implemented primarily in Python 3.6, but it also makes use of Django (for ORM) and Flask (for API and web server). It also uses several AWS services, primary S3 (for flat file storage), EC2 (servers), Elastic Beanstalk (scaling servers), and RDS (PostgreSQL).

Beiwe is intended for use in research. Essentially all software development kits (SDKs) made by companies like Apple and Google generate unvalidated behavioral summary measures using closed proprietary algorithms that do not meet the high standards of reproducible science. In contrast, Beiwe collects raw sensor and device usage data, which enables pooling of data across studies and re-analyses of data as new methods become available. Every aspect of data collection is fully customizable, including which sensors to sample, how frequently to sample them, whether to add Gaussian noise to GPS location, whether to use Wi-Fi or cellular data for uploads, how frequently to upload data, specification of surveys and their response options and skip logic, etc. All study settings are captured in a JSON-formatted configuration file to enhance transparency and repdocuibility of studies. Beiwe has been and continues to be used in a number of scientific studies on three continents in various areas ranging from XXX [@Pearson:2017] to YYY [@Pearson:2017] and [@Pearson:2017].

# Acknowledgements

The Principal Investigator, Dr. Jukka-Pekka Onnela, is extremely grateful for his NIH Director’s New Innovator Award in 2013 (DP2MH103909) for enabling the crystallization of the concept of digital phenotyping and the construction of the Beiwe platform. He is also grateful to his past and present mentees, mentors, collaborators, and staff; and to the Zagaran team for their expert software engineering.

# References
