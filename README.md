# aphrodite

aphrodite information system

## KoBo Forms

There is one KoBo Form for each group of the following accommodation/residence types

1. ESTIA Accommodation (both mainland and islands)
2. Mainland Self-Accommodated
3. Islands Self-Accommodated and RICs

## Excel Files for pulling data from KoBo via the API

One excel files for each Kobo. Each file has a table structure that is consistent with the data structure format (all tables need to have same structure so that data can be compiled into one table). There are nine (9) different tables that bring together the data from the KoBo form.

Assessment data
Risk Category 1 (one row per individual/family member)
Risk Category 1 (one row per individual/family member)
Risk Category 1 (one row per individual/family member)
Risk Category 1 (one row per individual/family member)
Risk Category 1 (one row per individual/family member)
Risk Category 1 (one row per individual/family member)
Support document(s) - hyperlink to the uploaded support documents. These files can be word documents, PDF files, scanned (jpg, png, etc.), and in some cases even an outlook email attached as a MSG file.
Related Registration Group

### Main excel file

The main excel file is the one that compiles all the data from the above described files into one files. Also it builds the relationship between the tables via the UUID of the "assessment data" table.

## MS Access Databases

There are three MS Access databases.
One database for all KoBo data, which pulls the data from the main excel file. Also it contains the macros to rebuild the tables from the main excel file into MS Access local tables. This last step is done to improve on the performance improvements.

One database is for pulling the data from proGres. It contain all the individual data with the Individual ID and Group ID as in proGres based on which the data is matched with the information from the KoBo.

## Main Access database a.k.a. Aphrodite

This database pulls the data from the above mentioned databases and adds the information on the Committee Decisions and the exit compliance based on the exit decisions.
