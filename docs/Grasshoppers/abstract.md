**Purpose**

The purpose of this work is to find an automated process to repair invalid DOI names that have been collected by the OpenCitations Index Of Crossref Open DOI-To-DOI References (COCI) while processing data provided by Crossref. 

**Design/methodology/approach**

The data needed for this work is provided by COCI as a CSV list containing more than 1 million invalid cited DOI names. With the goal to determine an automated process, we first need to classify the errors that characterize the wrong DOI names in the list. Our starting hypothesis is that there are two main classes of errors: factual errors, such as additional characters, and DOI names that were not yet valid at the time of processing. In a first step, we try to filter out the now valid DOI names using the DOI API. Then we propose a classification of the factual errors as prefix-, suffix- or other-type errors. By closer investigation and making use of already existing research in this field, we classify regular expressions that can be used to clean up the different types of invalid DOI names, for example deleting additional strings in the end or the beginning. After the cleanup, the cleaned DOI names are checked for their validity again. 

**Findings**

For the DOI names containing factual errors, we were able to find automated processes based on regular expressions to correct the errors belonging to different subclasses. It seems for now that only by cleaning up the suffix-type errors, we can correct more than 140 000 invalid DOI names. In the end of our work, we are going to estimate how many correct DOI names and, therefore, citations are obtained from the whole process. 

**Research limitations/implications**

There will always remain DOI names that cannot be made valid using automated processes. In these cases, it is important to find the publishers responsible for the incorrect references, which is done in a separate related project. An important part of our work will consist of discussing possible drawbacks of our methods and further developments that can be made.

**Originality/value**

Trying to make reference lists of scientific works accessible to the public, the COCI project contributes to the open science movement. In this global movement towards openness in scientific research, the accountability and transparency of scientific enterprise are fundamental. By trying to improve the data quality in COCI, our work can be useful not only for COCI, but in a broader sense also for the open science movement and related research in the future.

**Keywords**: Open Access, I4OC, OpenCitations, citations, DOI, Crossref, COCI, data quality
