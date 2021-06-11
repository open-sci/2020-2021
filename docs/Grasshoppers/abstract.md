**Purpose** 

The purpose of this work is to find an automated process to repair invalid DOI names that have been collected by Silvio Peroni while processing data provided by Crossref (2021).

**Design/methodology/approach** 

The data needed for this research is provided as a CSV list containing more than 1 million invalid cited DOI names. First, to determine an automated process, the errors that characterize the wrong DOI names in the list need to be classified. Concentrating exclusively on the factual errors, such as additional or invalid characters, the DOI names that have become valid in the meantime can be removed. Then, a classification of those factual errors as prefix-, suffix- or other-type errors is proposed. By closer investigation and extension of already existing research in this field, this research classifies regular expressions that can be used to clean the different types of invalid DOI names: for example, by deleting additional strings at the end or the beginning. After the cleanup, the cleaned DOI names are checked for their validity again.

**Findings** 

This research was able to find automated processes based on regular expressions and correct the factual errors belonging to different subclasses. Applying the proposed algorithm to the mentioned dataset, around 16% of the DOI names proved valid afterwards. The largest part of those valid DOIs consists of those made valid by cleaning up suffix errors; however, many DOIs also proved valid without cleaning, being only temporarily invalid.

**Research limitations/implications** 

Checking if the DOI names are valid either consumes a lot of time or a high amount of RAM, since the process should be executed before and after the cleaning. Therefore, the described methods are only applicable on smaller datasets, unless the availability of the necessary resources is ensured. Also, there will always remain DOI names that cannot be made valid using automated processes. In these cases, it is important to find the publishers responsible for the incorrect references, which is done in a separate related project (Cioffi et al., 2021). 

**Originality/value** 

Building on existing research, this study extends and improves regular expressions targeted to clean DOI errors, to enhance the data quality in the COCI dataset. As the COCI project provides open access to reference lists of scientific works, the whole academic community can profit from this improvement in data quality. In addition, the methods submitted could be the base for further research in this field, allowing the correction of DOI name errors in other datasets, too.

**Keywords**: Open Access, I4OC, OpenCitations, citations, DOI, Crossref, COCI, data quality
