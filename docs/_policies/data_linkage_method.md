---
layout: page
title: Data Linkage Method
permalink: /policies/data_linkage_method
parent: Data Access and Privacy Policies
nav_order: 36
---

## Method of Data Linkage
To fulfill a data request an approved request, individual record data from participating agency’s systems are linked at the unit record level to determine patterns over time.  

After a data request has been approved in accord with the P20 WIN Data Request Process, Participating Agencies whose data is a part of the request shall send files to DOL which contain only limited PII for matching the records that are needed to satisfy the approved Data Request. In addition to limited PII, each input file shall contain a generic unique identifier for each person record.  The generic unique identifier will bear no resemblance to or contain any part of an individual’s education data.  

Upon receipt of all required input data sets, DOL shall utilize data matching software approved by the Data Governing Board to identify matches between the data sets.  Once the matching is complete, DOL will strip the PII from the matched data file.  The stripped PII and the PII in the original data files shall be destroyed.  The resulting file, containing a matrix of the synthetic unique identifiers that reflects how the original data sets can be linked, shall be sent to the approved requestor for the completion of the approved data request. Destruction of the original files used for matching will occur within 5 business days after DOL receives confirmation from the Data Steward Committee members whose data were a part of the Data Request that the matching activity for the given Data Request is complete. Data destruction will occur within 24 hours of notification for any data set that includes data from an institution that is a member of the Connecticut Conference of Independent Colleges.  

In all cases, Participating Agencies send PII data from their systems for matching to DOL and to the Operating Group for Disclosure Review before any data is shared with the approved requestor via a secure file transfer protocol (SFTP).   

All files should be in text format.  Both comma and tab delimited are fine.

Files will all be named with a common format:
-	File with data for matching = P20_Qxxxx_CSCU_match_vx.
-	File with data for analysis = P20_Qxxxx_CSCU_analysis_vx.
-	Qxxxx = the P20 WIN number of the request
-	CSCU = the abbreviation of the sending entity.  This could be UCONN, or OEC, etc.
-	Vx = the version of the file (e.g. v2 or v3)

The match file should be formatted according to the agreed upon standard.  If a file contains dates, they should be formatted as YYYYMMDD.

Agencies should follow these formatting requirements when creating a file set for data matching. This chart includes all of the possible fields for data matching; however, they may not all be used. Researchers and agency analysts should use the spreadsheet titled “Requested Data Elements” to identify which fields are necessary to conduct the match for each data request.

| Data Element Name | Definition                                                                                                                  | Format       | Comment                                                                                       |
|-------------------|-----------------------------------------------------------------------------------------------------------------------------|--------------|-----------------------------------------------------------------------------------------------|
| LastName          | Last name of student                                                                                                        | Text         | Okay as is                                                                                    |
| MiddleName        | Middle name of student                                                                                                      | Text         | Okay as is                                                                                    |
| FirstName         | First name of student                                                                                                       | Text         | Okay as is                                                                                    |
| DOB               | Date of birth of student                                                                                                    | YYYYMMDD     |                                                                                               |
| Gender            | Gender of student                                                                                                           | Text         | M = male<br>F = female<br>U = unknown                                                         |
| HighSchoolCode    | College Board High School assigned to the high school (e.g. 070323 = RHAM High School)                                     | Include leading zero |                                                                                       |
| HighSchoolName    | Test name of student’s high school                                                                                          | Text         |                                                                                               |
| SASID             | State Assigned Student Identification Number                                                                                | Text         | There are no leading zeros                                                                    |
| SSN               | Social Security Number                                                                                                      | Include leading zero | Only when linking to wage data                                                         |
| Synthetic ID*     | Each agency creates a specific, one-time use, meaningless, fake ID assigned to each individual in a data set to facilitate analysis once the personally identifiable data used for matching has been deleted. | Text         |                                                                                               |
