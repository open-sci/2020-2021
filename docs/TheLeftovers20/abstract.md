<b>Purpose</b> <br>
The primary purpose of this research is to find the publishers responsible for the missing citations in COCI (the OpenCitations Index of Crossref open DOI-to-DOI citations) by sending incorrect metadata to Crossref, the publishers to whom such invalid citations point to, and the number of previously invalid citations which are currently valid. Further, the additional aim of the present research is to provide material for future and deeper research on the same subject matter. In particular, we focus on keeping track of the main trends of evolution on the validity of citational data and on providing data to facilitate publishers' identification. 

<b>Study design/methodology</b><br>
In order to study the invalid citations, we use an already generated CSV file which is available online, containing - for each citation - the valid citing DOI and the invalid cited DOI. First of all, through a DOI API request we check whether the validity state of the cited DOI has changed, and then we use DOIs' prefixes for CROSSREF API requests, in order to identify the responsible and referenced publishers.

<b>Findings</b><br>
For each individual publisher, we retrieve the number of incorrect given citations metadata sent, and the number of invalid citations received, to which we decided to add the information about the number of addressed and received citations validated with the software we developed, and its list of prefixes. We also extracted the total number of invalid citations that have since been corrected. Any further material provided as result of this research, such as the lists of validated and still invalid citations, is meant to incentivate future improvements of the studies on this field. 

<b>Originality/value</b><br>
The results of this research may point us to publishers who generally send out incorrect citation metadata and, inversely, those who generally receive invalid citations. These findings can first of all raise awareness of the accuracy of certain publishing houses in managing their metadata (or lack thereof). Moreover, finding these trends and showcasing the labor of the corrections may lead to increasingly valid citations if the proper measures are taken. 

<b>Research limitations/implications</b><br>
Based on the available data for COCI, there may be a slight bias in our sample, causing some publishers to be incorrectly represented.
