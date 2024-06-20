---
title: "Bulk Edit"
linkTitle: "Bulk Edit"
date: 2024-05-09
weight: 550
---

**This section of the documentation contains links to external sites. Please be advised that these external sites are not maintained by the FOLIO Documentation Group and may be aligned with a different FOLIO release.**


The Bulk Edit app allows a user to apply changes to multiple FOLIO records simultaneously. 


Bulk edit can apply changes to these record types:


* **Inventory - holdings**
* **Inventory - instances**
* **Inventory - items**
* **Users**


## Permissions


The permissions listed below allow you to interact with the Bulk Edit app and determine what you can or cannot do within the app. Permissions are assigned to users in the Users app. If none of these permissions are assigned to a user, they are unable to see the Bulk Edit app or any related information. 


Bulk edit permissions, combined with other functional app permissions, allow a user to access specific areas of the Bulk Edit app. Depending on how your library runs bulk edit jobs, users may also need permissions in other modules, such as Export Manager, Inventory, Users, and Settings. For more information about permissions, see [Users \> Permissions](../users/#permissions). 


The following are the permissions for the Bulk edit app:


- **Bulk edit: In App - Edit user records.** This permission allows the user to edit multiple user records in the Bulk Edit app. 
- **Bulk edit: Can build query**: This permission allows the user to build and test a query, and preview matched records in the Bulk edit app. 
- **Bulk edit: Can view logs** This permission allows the user to download and view logs in the Bulk Edit app.
- **Bulk edit: In app - Edit inventory records** This permission allows the user to edit a field in multiple inventory records in the Bulk Edit app. 
- **Bulk edit: In app - View inventory records** This permission allows the user to view a list of inventory records in the Bulk Edit app. 
- **Bulk edit: Local - Edit user records** This permission allows the user to edit a field in multiple user records in Bulk Edit using the CSV approach.
- **Bulk edit: Local - View user records** This permission allows the user to view a list of identified user records in Bulk Edit using the CSV approach.


## Bulk edit methods


The Bulk edit app provides two methods for editing records: 


* **Bulk edit**: The **Bulk edit** approach is also referred to as **In-app**. This approach allows the user to set criteria for the bulk edit by uploading a list of record identifiers from a .csv file. Once the records are identified and matched, **Bulk edit** allows the user to designate an action for these records and commit the changes to the records in FOLIO’s user interface. 


* **Bulk edit (Local)**: The **Bulk edit (Local)** approach is also referred to as **CSV**. This approach uses a .csv file to display records matching a selected **Record identifier**. Changes are made to the records and saved in the .csv file, and committed to FOLIO by uploading the edited .csv file. 


Note that Microsoft Excel processes .csv files in ways that may change data unexpectedly, especially date and time fields. Reviewing the .csv data in a text editor helps ensure that no unexpected changes are made to records when using **Bulk edit (Local)**.


## Inventory - holdings


### Identify records


The Bulk edit app accepts only .csv files for upload. Files should include only one column of record identifiers. If the file contains more than one column, the upload will not be successful and a *Something went wrong* message will display. 


To set the criteria and identify records for bulk edit, follow these steps:


1. In the **Set criteria** pane, ensure **Record types** is set to **Inventory - holdings**.
2. In the **Set criteria** pane, select the **Record identifier** from the drop-down list. The record identifier you select should correspond to the type of record identifier in the .csv file.
3. Either **Drag and drop** your .csv file into the **Select a file** box, or click **or choose file** to locate the file on your computer. The .csv file automatically uploads and searches for matching **Holdings** records.


### Preview matched records


Once the file upload is complete, the matching **Holdings** records are listed in the **Preview of record matched** pane. To customize the column headings in the preview, click the **Actions** button. To add, check the box next to the column heading; to remove, uncheck the box or leave it empty. 


### Errors


The **Error** accordion contains a list of errors found when searching for the matched records, if any, and displays the errors in two columns:


* **Record identifier.** The identifier for the record that produced the error
* **Reason for error.** The reason the search did not result in a matched record. 


### Start bulk edit


Inventory - holdings records may be changed by using the Bulk edit or In-app approach. The fields that can be changed in holdings records using this approach include **temporary holdings location**, permanent holdings location, and suppress from discovery. 


To start a bulk edit on the matched records, follow these steps: 


1. Click the **Actions \> Start bulk edit**.
2. Under **Options**, click the drop-down list and select the field you want to edit.
3. Under **Actions**, click **Select action** and select the action you want to apply to the item records.
4. To edit an additional field during the same bulk edit job, click the plus sign near the end of the row. Another row will appear under the existing row(s).
5. To delete a row, click the trash icon at the end of the row you want to delete. The row is deleted. 
6. Click **Confirm changes**. A new window will appear with a preview of the first 10 records to be changed.
7. To return to the bulk edit, click **Keep editing**. The window will close and you can continue editing.
8. To preview the entire list of records, click **Download preview**. A .csv file is downloaded to your local device.
9. To run the bulk edit job, click **Save & close**. The window closes and the banner at top of the **Bulk edit** pane displays the number of records successfully changed.
10. To download the list of changed records, click the **Actions** button at the top right of the pane.
11. Select **Download changed records (CSV)**. The .csv file is downloaded to your local device. 


#### Temporary holdings location 


To bulk edit the temporary holdings location of the matched records, follow these steps:


1. Under **Options**, select **Temporary holdings location** from the drop-down list.
2. Click **Actions** to select **Replace with** or **Clear field**. 
3. For **Replace with**, click **Select Location** and select the temporary holdings location from the drop-down list or use the **Location look-up**.
4. For **Clear field**, proceed to step 5.
 Click **Confirm changes**. 
5. The **Preview of records to be changed** will pop up with options of **Keep editing**, **Download preview**, or **Commit changes**.
6. The changes will be applied to the item records once **Commit changes** is clicked.


#### Permanent holdings location 


To bulk edit the permanent holdings location of the matched records, follow these steps:


1. Under **Options**, select **Permanent holdings location** from the drop-down list.
2. Click **Actions** to select **Replace with** or **Clear field**. 
3. For **Replace with**, click **Select Location** and select the permanent holdings location from the drop-down list or use the **Location look-up**.
4. Click **Confirm changes**. 
5. The **Preview of records to be changed** will pop up with options of **Keep editing**, **Download preview**, or **Commit changes**.
6. The changes will be applied to the item records once **Commit changes** is clicked.

## Inventory - instances

### Identify records

The **Bulk edit** app accepts only .csv files for upload. Files should include only one column of record identifiers. If the file contains more than one column, the upload will not be successful and a *Something went wrong* message will display. 

In the **Set criteria** pane, ensure **Record types** is set to **Inventory - instances**.
In the **Set criteria** pane, select the **Record identifier** from the drop-down list. The record identifier you select should correspond to the type of record identifier in the CSV file uploaded.
Either drag and drop your CSV file into the box, or click **or choose file** to locate the file on your computer. The .csv file automatically uploads and searches for matching **Items** records.

### Preview matched records

Once the file upload is complete, the matching **Instances** records are listed in the **Preview of record matched** pane. To customize the column headings in the preview, click the **Actions** button. To add, check the box next to the column heading; to remove, uncheck the box or leave it empty. 

### Download Matched Records (CSV)

1. Click the **Actions** button.
2. From the drop-down menu, select **Download matched records (CSV)**.
3. Open the file on your local device.
4. Edit the records and save the file on your local device. Make sure you save the file in CSV format.

### Download Errors (CSV)

The **Error** accordion contains a list of errors found when searching for the matched records, if any, and displays the errors in two columns:

**Record identifier.** The identifier for the record that produced the error
**Reason for error.** The reason the search did not result in a matched record. 

### Start bulk edit

Inventory - instances may be changed by using the Bulk edit or In-app approach. The actions that can be done in instance records with this approach include **Staff suppress** and **Suppress from discovery**. 

To start a bulk edit on the matched records, follow these steps:

1. Click the **Actions** button.
2. From the drop-down menu, select **Start bulk edit**. 
3. Under **Options**, click the drop-down list and select the option you want to execute.
4. Under **Actions**, click **Select action** and select the action you want to apply to the instance records.
5. To edit another field during the same bulk edit job, click the plus sign near the end of the row. Another row will appear under the existing row(s).
6. To delete a row, click the trash icon at the end of the row you want to delete. The row is deleted. 
7. Click **Confirm changes**. A new window will appear with a preview of the first 10 records to be changed.
8. To return to the bulk edit, click **Keep editing**. The window will close and you can continue editing.
9. To preview the entire list of records, click **Download preview**. A .csv file is downloaded to your local device.
10. To run the bulk edit job, click **Commit changes**. The window closes and the banner at top of the Bulk edit pane displays the number of records successfully changed.
11. To download the list of changed records, click the **Actions** button at the top right of the pane.
12. Select **Download changed records (CSV)**. The .csv file is downloaded to your local device. 

#### Staff suppress

To suppress the matched item records from staff view in the Bulk edit app, follow these steps:

1. In the **Bulk edit** window, select **Staff suppress** from the **Select option** drop-down list.
2. Select the appropriate Action from the Select action drop-down list.
   * **Set true**: Suppresses the matched item records from staff view in the Bulk edit app.
   * **Set false**: Unsuppresses the matched item records from staff view in the Bulk edit app.
3. Click **Confirm changes**to apply the changes to the matched item records.
4. An *Are you sure?* message appears in a new window with a **Preview of records to be changed**. An alert appears at the top of the window: *(Number of) records will be changed if the Commit changes button is clicked. You may choose Download preview to review all changes prior to saving.
5. Click **Keep editing** to return to the Bulk edits window, **Download preview** to preview the changes before saving, or **Commit changes** to run the bulk edit.

#### Suppress from discovery

To suppress the matched instance records from discovery in the Bulk edit app, follow these steps:

 1. In the **Bulk edit** window, select **Suppress from discovery** from the **Select option** drop-down list.
 2. Select the appropriate Action from the Select action drop-down list.
    * **Set true**: Suppresses the matched instance records from discovery.
    * **Set false**: Unsuppresses the matched instance records from discovery.
 3. Once an action is selected, the Data defaults to apply the same **Set true** or **Set false** action to all holdings records and all items records. Click the appropriate checkbox(es) if you do not want the selected action to be applied to the holdings records and/or item records, 
 4. Click **Confirm changes** to apply the changes to the matched ins records.
 5. An *Are you sure?* message appears in a new window with a **Preview of records to be changed**. An alert appears at the top of the window: *(Number of) records will be changed if the Commit changes button is clicked.* You may choose Download preview to review all changes prior to saving.
 6. Click **Keep editing** to return to the Bulk edits window, **Download preview** to preview the changes before saving, or **Commit changes** to run the bulk edit. The changes will be applied to the matched item records once **Commit changes** is clicked. 


## Inventory - items


### Identify records


The **Bulk edit** app accepts only .csv files for upload. Files should include only one column of record identifiers. If the file contains more than one column, the upload will not be successful and a *Something went wrong* message will display. 


1. In the **Set criteria** pane, ensure **Record types** is set to **Inventory - items**.
2. In the **Set criteria** pane, select the **Record identifier** from the drop-down list. The record identifier you select should correspond to the type of record identifier in the CSV file uploaded.
3. Either drag and drop your CSV file into the box, or click **or choose file** to locate the file on your computer. The .csv file automatically uploads and searches for matching **Items** records.


### Preview matched records


Once the file upload is complete, the matching **Items** records are listed in the **Preview of record matched** pane. To customize the column headings in the preview, click the **Actions** button. To add, check the box next to the column heading; to remove, uncheck the box or leave it empty. 


### Download Matched Records (CSV)


1. Click the **Actions** button.
2. From the drop-down menu, select **Download matched records (CSV)**.
3. Open the file on your local device.
4. Edit the records and save the file on your local device. Make sure you save the file in CSV format.


### Download Errors (CSV)


The **Error** accordion contains a list of errors found when searching for the matched records, if any, and displays the errors in two columns:

- **Record identifier.** The identifier for the record that produced the error
- **Reason for error.** The reason the search did not result in a matched record. 


### Start bulk edit


Inventory - items may be changed by using the Bulk edit or In-app approach. The fields that can be changed in item records with this approach include **Administrative note**, **Check in note**, **Check out note**, **Item notes**, **Item status**, **Loan type**, **Location**, and **Suppress from discovery**. 

For more information about item record status changes available in Bulk Edit, see [Supported Item Record Status Changes](https://folio-org.atlassian.net/wiki/x/U5VW).


To start a bulk edit on the matched records, follow these steps:

1. Click the **Actions** button.
2. From the drop-down menu, select **Start bulk edit**. 
3. Under **Options**, click the drop-down list and select the field you want to edit.
4. Under **Actions**, click **Select action** and select the action you want to apply to the item records.
5. To edit another field during the same bulk edit job, click the plus sign near the end of the row. Another row will appear under the existing row(s).
6. To delete a row, click the trash icon at the end of the row you want to delete. The row is deleted. 
7. Click **Confirm changes**. A new window will appear with a preview of the first 10 records to be changed.
8. To return to the bulk edit, click **Keep editing**. The window will close and you can continue editing.
9. To preview the entire list of records, click **Download preview**. A .csv file is downloaded to your local device.
10. To run the bulk edit job, click **Commit changes**. The window closes and the banner at top of the Bulk edit pane displays the number of records successfully changed.
11. To download the list of changed records, click the **Actions** button at the top right of the pane.
12. Select **Download changed records (CSV)**. The .csv file is downloaded to your local device.


#### Administrative note


To bulk edit the **Administrative note** in the matched records, follow these steps:


1. Under **Options**, select **Administrative note** from the drop-down list.
2. Click **Actions** to select the action you want to apply from the drop-down list.
   
    - **Add note.** Input note text you want added. 
    - **Remove all** will delete any administrative notes in the item records..
    - **Find** Input note text you want to find. Select **Replace with** and input new text or select **Remove** to remove the text.
    - **Change note type.** Select the new note type.

      
3. Click **Confirm changes**. The selected action will be applied to the matched item records.
4. The **Preview of records to be changed** will pop up with options of **Keep editing**, **Download preview**, or **Commit changes**.
5. The changes will be applied to the item records once **Commit changes** is clicked.


#### Check in note


To bulk edit the **Check in note** in the matched records, follow these steps:


1. Under **Options**, select **Check in note** from the drop-down list.
2. Click **Actions** to select the action you want to apply from the drop-down list.
   
    - **Mark as staff only** marks the item note as viewable by staff only. 
    - **Remove mark as staff only** removes the staff only designation for the item note.
    - **Add note.** Input note text you want added. 
    - **Remove all** will delete any check in notes in the item records.
    - **Find** input note text you want to find. Select **Replace with** and input new text or select **Remove** to remove the text.
    - **Change note type.** Select the new note type you want.

      
3. Click **Confirm changes**. The selected action will be applied to the item records.
4. The **Preview of records to be changed** will pop up with options of **Keep editing**, **Download preview**, or **Commit changes**.
5. The changes will be applied to the matched item records once **Commit changes** is clicked.


#### Check out note


To bulk edit the **Check out note** in the matched records, follow these steps:


1. Under **Options**, select **Check out note** from the drop-down list.
2. Click **Actions** to select the action you want to apply from the drop-down list.
   
    - **Mark as staff only** marks the item note as viewable by staff only. 
    - **Remove mark as staff only** removes the staff only designation for the item note.
    - **Add note.** Input note text you want added. 
    - **Remove all** will delete any check in notes in the item records.
    - **Find**. Input note text you want to find. Select **Replace with** and input new text or select **Remove** to remove the text.
    - **Change note type.** Select the new note type you want.

      
3. Click **Confirm changes**. The selected action will be applied to the item records.
4. The **Preview of records to be changed** will pop up with options of **Keep editing**, **Download preview**, or **Commit changes**.
5. The changes will be applied to the matched item records once **Commit changes** is clicked.


#### Item notes


To bulk edit an **item note** in the matched records, follow these steps:


1. In the **Bulk edit** window, select the appropriate item note from the **Select option** drop-down list. The following types of item notes may be changed in the Bulk edit app:

    - **Action note**
    - **Binding**
    - **Copy note**
    - **Electronic bookplate**
    - **Provenance**
    - **Reproduction**

2. Click **Actions** to select the action you want to apply from the drop-down list. Actions available in the Bulk edit app include:

    - **Mark as staff only** marks the item note as viewable by staff only. 
    - **Remove mark as staff only** removes the staff only designation for the item note.
    - **Add note.** Input note text you want added. 
    - **Remove all** will delete any selected **item notes** from the item records.
    - **Find**. Input note text you want to find. Select **Replace with** and input new text or select **Remove** to remove the text.
    - **Change note type.** Select the new note type you want.


3. Click **Confirm changes**. The selected action will be applied to the matched item records..
4. The **Preview of records to be changed** will pop up with options of **Keep editing**, **Download preview**, or **Commit changes**.
5. The changes will be applied to the matched item records once **Commit changes** is clicked.


#### Item status


To bulk edit the **item status** field in the matched records, follow these steps:


1. In the **Bulk edit** window, select **Item status** from the **Select option** drop-down list. 
2. For **item status**, **Replace with** is the only **Action** allowed in bulk edit and is pre-selected by default.
3. Click **Actions** to select the item status you want to apply from the drop-down lis
4. Click **Confirm changes**. The new item status will be applied to the item records.
5. The **Preview of records to be changed** will pop up with options of **Keep editing**, **Download preview**, or **Commit changes**.
6. The changes will be applied to the item records once **Commit changes** is clicked.


#### Loan type


To bulk edit the **loan type** in the matched records, follow these steps:


1. In the **Bulk edit** window, select the appropriate loan type from the **Select option** drop-down list. The following loan types may be changed in the Bulk edit app:

    - **Permanent loan type**
    - **Temporary loan type**

2. Click **Actions** to select the action you want to apply from the drop-down list. 

    - For **permanent loan type**, **Replace with** is the only **Action** allowed in bulk edit and is pre-selected by default. 
    - For **temporary loan type**, **Replace with** and **Clear field** are the actions available in bulk edit. 
    - **Replace with**. Replaces the loan type in the matched records with the loan type selected in the **Select loan type** drop-down list. 
    - **Clear field**. Removes the data in the loan type field of the matched records.


3. Select the new loan type from the **Select loan type** drop-down menu or use the **Filter options list** to select the new loan type.
4. Click **Confirm changes**. The selected action will be applied to the matched item records.
5. The **Preview of records to be changed** will pop up with options of **Keep editing**, **Download preview**, or **Commit changes**.
6. The changes will be applied to the matched item records once **Commit changes** is clicked.


#### Location


To bulk edit the **Location** in the matched records, follow these steps:


1. In the **Bulk edit** window, select the appropriate location from the **Select option** drop-down list. The following locations may be changed in the Bulk edit app:

    - **Permanent location**
    - **Temporary location**

2. Click **Actions** to select the action you want to apply from the drop-down list.


    - **Replace with**: Replaces the location field in the matched records with the location selected in the **Select loan type** drop-down list. 
    - **Clear field**. Removes the data in the location field. 


3. Click **Confirm changes**. The selected action will be applied to the matched item records.
4. The **Preview of records to be changed** will pop up with options of **Keep editing**, **Download preview**, or **Commit changes**.
5. The changes will be applied to the matched item records once **Commit changes** is clicked.


#### Suppress from discovery


To suppress the matched item records from discovery in the Bulk edit app, follow these steps:


1. In the **Bulk edit** window, select **Suppress from discovery** from the **Select option** drop-down list.
2. Select the appropriate Action from the **Select action drop-down** list.
   
    - Set true: Suppresses the matched item records from discovery.
    - Set false: Unsuppresses the matched item records from discovery.
      
3. Click **Confirm changes** to apply the changes to the matched item records.
4. An *Are you sure?* message appears in a new window with a **Preview of records to be changed**. An alert appears at the top of the window: *(Number of) records will be changed if the Commit changes button is clicked*. You may choose Download preview to review all changes prior to saving. Click **Keep editing** to return to the Bulk edits window, **Download preview** to preview the changes before saving, or **Commit changes** to run the bulk edit.
5. The changes will be applied to the matched item records once **Commit changes** is clicked.


## Users


### Identify records


The Bulk Edit app accepts only .csv files for editing record identifiers in a record. The .csv file used to set criteria must include only one column of record identifiers. 

The Bulk Edit app accepts only .csv files for identifying records. The .csv file used to set criteria must include only one column of record identifiers. 

There are two methods for identifying records for Bulk edit: **Identifier** and **Query**. 

### Identifier

To set criteria for bulk edit using **Identifier**, follow these steps: 

 1. In the **Set Criteria** pane, select the **Identifier** button.
 2. Select **Users** under **Record types**.
 3. Select the record identifier type from the  **Select record identifier** drop-down menu.
 4. The **record identifiers** for Users include:

 * **User UUIDs**
 * **User barcodes**
 * **External IDs**
 * **Usernames**
 5. **Drag and drop** your .csv file into the **Select a file with record identifiers** box, or click **or choose file** to upload the .csv file from your computer.

### Query

The **Query** function in the Bulk Edit app allows the user to build a query to identify records for bulk edit. 

To set criteria for bulk edit using **Query**, follow these steps: 

1. In the **Set Criteria** pane, click on the **Query** tab.
2. Select **Users** under **Record types**.
3. Click the **Build query** button to open the **Build query** modal.
4. Select a **Field** from the *Select field* drop-down menu or filter the selection by typing the field in the *Filter options list* text box.
5. Select an **Operator** from the *Select operator* drop-down list. The operators available for selection are based on the Field. 

 *  ==: Field equals selected or input Value.
 *  !=:  Field does not equal selected or input Value.
 *  Contains: Field appears in selected or input Value.
 *  Starts: Field starts with selected or input Value.
 *  \>: Field is greater than the selected or input Value.
 *  <: Field is less than the selected or input Value.
 *  \>=: Field is greater than or equal to the selected or input Value.
 *  <=: Field is less than or equal to the selected or input Value.
 *  Is null/empty: Field is blank; it contains no data.
 6. Select a **Value** from the *Select value* drop-down list or type the value in the Value text box.  The Values available for selection are based on the Field and Operator.
 7. Click on the **+ icon** to add additional lines to the query; Click on the **trash can icon** to delete a line from the query. 
 8. Once a query is built, it must be tested before the query can be run and saved. Click the **Test query** button to run the query and display a preview of matched records. The query string can be edited in the **Query string** field. If edited, another Test query must be done.
 9. If the Test query is successful, click the **Run query** button to run the query and preview the matched records in the **Bulk edit query** modal.


### Preview matched records

If the **Identifier** method is used to identify records for bulk edit, the number of records matched and the filename display at the top of the **Bulk edit** modal. 

If the **Query** method is used to identify records for bulk edit, a Test query displays the Query string and number of records retrieved at the top of the **Build query** modal. 

 If the **Query** is run, the query and a preview of matched records display in the **Bulk edit query** modal. 


In either method, the following information appears in the **Preview of record matched** pane:


- **Username.** The username of the user.
- **Barcode.** The barcode from the user record.
- **Status.** The status of the user.
- **Patron group.** The patron group assigned to the user. 
- **Last name.** The last name of the user.
- **First name.** The first name of the user.


To include or remove record identifier columns in the preview pane, click **Actions \> Show columns**, check the box next to the name of the record identifier to include as a column in the preview; or uncheck the box next to the name of the record identifier to remove the column from the preview.


### Download matched records


To download the matched records as a .csv file, follow these steps:


1. In the **Preview** pane, click **Actions \> Download matched records (CSV)**.
2. Depending on the web browser settings, the .csv file may be opened and/or saved. 


### Download errors


If there are errors in the matched records, a message indicating the filename, number of entries, number of records matched, and number of errors display in the **Errors** section. 


Any errors display in a two-column table in the **Errors** section. 


* **Record identifier.** The record identifier for the records that produced the error.
* **Reason for error.** The reason why the error was produced.


To download the errors as a .csv file, follow these steps:


1. In the **Preview** pane, select **Actions \> Download errors (CSV)**.
2. Depending on the web browser settings, the .csv file may be opened and/or saved. 


### Start bulk edit 

The data in the **Email**, **Expiration date**, and **Patron group** fields of matched user records can be replaced with new data by using the Bulk edit approach. Bulk edit may be performed on each of these fields individually or simultaneously. To bulk edit all three fields simultaneously, click the **+ icon** at the end of the row to add another bulk edit option. 

To start a bulk edit, follow these steps:

1. In the **Preview** pane, click **Actions > Start bulk edit**. The number of matched records and the filename of the .csv file display at the top of the **Bulk edit** window.
2. In the **Bulk edits** section, select **Email**, **Expiration Date**, or **Patron Group**.
 - For **Email**, bulk edit performs a find and replace in the email address field of the matched records. Thus, the **Actions** available are **Find (full field search)** and **Replace with** . Type the current data (text) in the **Find (full field search)** box. Type the new data (text) in the **Replace with** box. 
 - For **Expiration date**, bulk edit replaces the date in the Expiration date of the matched records. Thus, the **Actions** available are limited to **Replace with**.  Type the new expiration date in MM/DD/YYYY format in the **Data** box. 
 - For **Patron group**, bulk edit replaces the Patron group data in the matched records. Thus, the **Actions** available are limited to **Replace with**. Select the new Patron group from the **Data** drop-down menu. 
3. Click the **Confirm changes** button.
4. A message appears in the **Are you sure?**modal. The message *(Number of) records will be changed if the Commit changes button is clicked. You may choose Download preview to review all changes prior to saving.* A **Preview of records to be changed** is also displayed.
 - Click **Keep editing** to return to the Bulk edit window.
 - Click **Download preview** to download a .csv file of the proposed changes. 
 - Click **Commit changes** to run the bulk edit.
5. When the bulk edit is complete, a confirmation message, *(Number of) records have been successfully changed*, appears in the **Bulk edit** window. 
6. To change the column headings in the **Preview of record changed** table, click **Actions** and select or deselect the fields in the **Show columns** list as appropriate.
7. To download a .csv file of changed records, click **Actions > Download changed records (CSV)**. 


### Start bulk edit (Local)

The **Bulk edit (Local)** function allows the user to perform a bulk edit on records edited locally (external to FOLIO) by uploading a .csv file of the changed, or edited, records. 

Any field in matching user records can be changed by using the Bulk edit (Local) approach.

Note that Microsoft Excel processes .csv files in ways that may change data unexpectedly, especially date and time fields. Reviewing the .csv data in a text editor helps ensure that no unexpected changes are made to records with **Bulk edit (Local)**.

To use **Bulk edit (Local)** approach to apply changes to records, follow these steps: 

1. In the **Set criteria** pane, select Users as the **Record type** and select the appropriate **Record identifier**: User UUIDs, User barcodes, External IDs, or Usernames.
2. Upload a .csv file with the selected Record identifier by either using the **Drag and drop** option or clicking the **Choose file** button.
3. Select **Actions \> Download matched records (CSV)** to download a .csv file of matched user records; or select **Actions \> Download errors (CSV)** to download a .csv file of records that did not match your selected record identifier. 
4. Edit the downloaded .csv file and make changes to the user records in the file itself. Save the edited .csv file to your computer.
5. Select **Actions \> Start bulk edit (Local)**. 
6. In the **Bulk edit** window, **Drag and drop** the .csv file into the **Upload CSV file with edited records** box, or click **or choose file** to upload the .csv file from your computer. If the .csv file is uploaded successfully, the confirmation message, *(Name of File).csv successfully uploaded*, displays in a new window.
7. Click **Next**. The warning message, *(Number of) records will be updated if the **Commit changes** button is clicked.* appears in a new window.
8. Click **Commit changes**. Bulk edit will apply the local changes to the records in FOLIO.


## Logs
The Bulk edit app allows users to preview bulk edit logs based on set criteria and download a file associated with a bulk edit job. 

### Preview bulk edit logs


The options available for setting criteria include: **Statuses**, **Record types**, **Started**, **Ended**, and **User**.  


To set criteria and preview bulk edit logs, follow these steps:


1. Click on the **Identifier** tab in the **Set criteria** pane.
2. Under the **Statuses** accordion, select the status for the bulk edit log by checking the appropriate box:  

    - **New**
    - **Retrieving records**
    - **Saving records**
    - **Data modification**
    - **Reviewing changes**
    - **Completed**
    - **Completed with errors**
    - **Failed**

      
3. Under the **Record types** accordion, select the record type for the bulk edit log by checking the appropriate box:

    - **Inventory - holdings**
    - **Inventory - instances**
    - **Inventory - items**
    - **Users**

      
4. In the **Started** accordion, use the **calendar icon** or type in the date using the YYYY-MM-DD format in the **From** and **To** fields to limit the preview by the start date of the bulk edit. Click **Apply**.
5. In the **Ended** accordion, use the **calendar icon** or type in the date using the YYYY-MM-DD format in the **From** and **To** fields to limit the preview by the end date of the bulk edit. Click **Apply**.
6. In the **Users** accordion, select the user, or FOLIO account, that ran the bulk edit job from the **Choose user** drop-down list.
7. A preview list of bulk edit logs displays in the **Bulk edit logs** pane. The number of bulk edit logs in the preview displays at the top of the pane as *(number of) records found*. The column headings display the following criteria for each bulk edit log:

    - **Record type**: type of records changed in the bulk edit job
    - **Status**: status of the bulk edit job
    - **Editing**: method of bulk edit used - **In App** or **Local**
    - **# of records**: number of records retrieved for bulk edit
    - **Processed**: number of records changed in bulk edit job
    - **Started**: start date and start time of bulk edit job
    - **Ended**: end date and end time of bulk edit job
    - **Run by**: user or FOLIO account used to run the bulk edit job
    - **ID**: system-generated number assigned to the bulk edit job


### Download a bulk edit log file


In the Bulk edit app, a file used to run a bulk edit job can be downloaded and saved from the **Bulk edit logs** pane.


To download a file associated with a bulk edit log, follow these steps:


1. In the **Bulk edit logs** pane, click on the ellipses in the **Actions** column next to the appropriate bulk edit log. 
2. Select the appropriate action from the **Download** drop-down list. The types of files available for download include: 

    - **File that was used to trigger the bulk edit**
    - **File with the matching records**
    - **File with errors encountered during the record matching**
    - **File with the preview of proposed changes**
    - **File with updated records**.


3. Depending on the web browser, the file can be opened or saved to your computer.
