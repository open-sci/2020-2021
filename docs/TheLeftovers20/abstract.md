<b>Purpose</b> <br>
The purpose of this research is to find the publishers responsible for the missing citations in COCI (the OpenCitations Index of Crossref open DOI-to-DOI citations) by sending incorrect metadata to Crossref, the publishers to whom such invalid citations point to, and the number of previously invalid citations which are currently valid.

<b>Study design/methodology</b><br>
In order to find the invalid citations, we use an already generated CSV file, containing the DOIs of invalid citations and their correct form, which is available online. These DOIs along with the COCI REST API can lead us to the responsible and referenced publishers.

<b>Findings</b><br>
We found for each individual published 1) the number of incorrect given citations metadata sent, and 2) the number of invalid citations received. We also extracted the total number of invalid citations that have since been corrected.

<b>Originality/value</b><br>
The results of this research may point us to publishers who generally send out incorrect citation metadata and, inversely, those who generally receive invalid citations. These findings can first of all raise awareness of the accuracy of certain publishing houses in managing their metadata (or lack thereof). Moreover, finding these trends and showcasing the labor of the corrections may lead to increasingly valid citations if the proper measures are taken.

<b>Research limitations/implications</b><br>
Based on the available data for the COCI, there may be a slight bias in our sample, causing some publishers to be incorrectly represented.
