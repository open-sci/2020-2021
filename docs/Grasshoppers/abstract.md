**Purpose**

The purpose of this work is to find an automated process to repair invalid DOIs that have been collected by the OpenCitations Index Of Crossref Open DOI-To-DOI References (COCI) while processing data provided by Crossref. 

**Design/methodology/approach**

The data needed for this work is provided by COCI as a CSV list containing invalid cited DOIs. With the goal to determine an automated process, we first need to classify the errors that characterize the wrong DOIs in the list. Our starting hypothesis is that there are two main classes of errors: factual errors, such as wrong characters, and DOIs that are not yet valid at the time of processing. The first class can be furtherly divided into errors due to forbidden characters, such as whitespaces, errors due to irrelevant strings added to the beginning or end of the correct DOI, or human-made errors. Once the classes of errors are addressed, we propose automatic processes to obtain correct DOIs from wrong ones. These processes involve the use of structured and unstructured information returned from DOI and Crossref APIs, as well as rule-based methods to correct invalid DOIs. 

**Findings**

For the DOIs containing factual errors, we were able to find automated processes to correct the errors belonging to different subclasses. In the end of our work, we are going to estimate how many correct DOIs and, therefore, citations are obtained. 

**Research limitations/implications**

There will always remain DOIs that cannot be made valid using automatic processes. In these cases, it is important to find the publishers responsible for the incorrect references, which is done in another related project. An important part of our work will consist of discussing possible drawbacks of our methods and further developments that can be made.

**Originality/value**

Trying to make reference lists of scientific works accessible to the public, the COCI project contributes to the open science movement. In this global movement towards openness in scientific research, the accountability and transparency of scientific enterprise are fundamental. By trying to improve the data quality in COCI, our work can be useful not only for COCI, but in a broader sense also for the open science movement and related research in the future.

**Keywords**: Open Access, I4OC, OpenCitations, citations, DOI, Crossref, COCI, data quality
