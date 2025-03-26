---
layout: page
title: Standard naming convention for files and data elements
parent: Determination of requirements for data providers
permalink: /key_processes/data_provider_requirements/naming_conventions
nav_order: 13
---

# Standard naming convention for files and data elements

The file naming standard for data files transferred via SFTP is as follows:  

a. Agency acronym

b. Data Request Number listed in DSA

c. Date file was created (MM_DD_YYYY)

d. Contents of file (matching, analytical, key)

example: "DOL.000.01_01_2000.matching"

The table below identifies the most commonly requested data variables.

| Field/Data Element | Format | Possible Values | Definition | Comment | 
| ----- | ----- | ----- | ----- | ----- |
| SSN | Text or Varchar(9) | | Social security # | With leading zero |
| DOB | YYYYMMDD | YYYYMMDD | Date of Birth | As a text field |
| Gender |  Text or varchar(1) | M = male, F = female, U = unknown | Gender | |
| Race/Ethnicity | | | | |
| LastName | Text | | | |
| MiddleName | Text | | | |
| FirstName | Text | | | |
| SASID | Text or varchar(10) | | State Assigned Student Identification Number | |
| HighSchoolCode | Text or varchar(6) | | CollegeBoard HS assigned code | Include leading zero |
| Fake ID | | | A unique fake identifier to be used | |
