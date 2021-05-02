**Purpose** 

The purpose of this work is to find an automated process to repair invalid DOI names that have been collected by the OpenCitations Index Of Crossref Open DOI-To-DOI References (COCI) while processing data provided by Crossref. 

**Design/methodology/approach** 

The data needed for this work is provided by COCI as a CSV list containing more than 1 million invalid cited DOI names. With the goal to determine an automated process, we first need to classify the errors that characterize the wrong DOI names in the list. Concentrating on only the factual errors, like additional or invalid characters, we can filter out the DOI names that have become valid in the meantime. Then, we propose a classification of those factual errors as prefix-, suffix- or other-type errors. By closer investigation and extension of already existing research in this field, we classify regular expressions that can be used to clean up the different types of invalid DOI names, for example deleting additional strings at the end or the beginning. After the cleanup, the cleaned DOI names are checked for their validity again.  

**Findings** 

We were able to find automated processes based on regular expressions to correct the factual errors belonging to different subclasses. Applying our algorithm to a subset of the data, around 19% of the DOI names proved valid afterwards. The largest part of those valid DOIs consists of those made valid by cleaning up suffix errors, but also many DOIs proved valid without cleaning, having been only temporarily invalid. 

**Research limitations/implications** 

As the checking for validity of the DOI names that should be executed before and after the cleaning either consumes a lot of time or a high amount of RAM, our methods are only applicable on smaller datasets or having ensured the availability of the necessary resources. Also, there will always remain DOI names that cannot be made valid using automated processes. In these cases, it is important to find the publishers responsible for the incorrect references, which is done in a separate related project.  

**Originality/value** 

Building up on existing research, we extend and improve regular expressions to clean up DOI errors with the goal to enhance the data quality in the COCI dataset. As the COCI project provides open access to reference lists of scientific works, the whole academic community can profit from this improvement in data quality. In addition, our methods could be the base for further research in this field, permitting to also correct DOI name errors in other datasets. 

**Keywords**: Open Access, I4OC, OpenCitations, citations, DOI, Crossref, COCI, data quality
