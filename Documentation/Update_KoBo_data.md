# How to update KoBo data for Aphrodite

## Step 1

Verify everything is working well with KoBo

## Step 2

Open the corresponding Excel file for the KoBo and under the Data tab click on the Update tool and then select "Update All". Once the query is finished running, save the changes and close the the file.

## Step 3

Open the main Excel file and repeat the same steps as in the Step 2. The procedure is the same, except in this case the data is being compiled from all the excel files stored in teh "dbfile" folder.

## Step 4

Ope the KoBo MS Access database. Find the "Rune all" macro and double-click to execute. Once all he queries have completed running, a message will pop up informing you that the process is completed and that you need to verify the you need to check the linked table "lnk_assessment" and local table "tbl_assessment" to make sure they are storing the same data.

That should be all!
