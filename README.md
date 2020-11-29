# MovieLibrary
MovieLibrary project for YearOne

Hello! This is the final version of the MovieLibrary project that I made.
Here are the steps to use the application: 

1. The project was created using Visual Studio 2019, so please open it with that version.
2. After opening the project, please build it.
3. The Web.config file is what controls whether the application will use the in-memory Test database or the Production SQL database.
  To change between these two, change the value of the key labeled "Mode" on line 20 to "SampleData" for the Test database or "ADO" for the SQL database.
  
3a. If checking these values is necessary, please open the "RepositoryFactory.cs" file, which will also note what I have written above.

3b. No further configuration is necessary to use the Test database; however, to use the SQL database, please look at steps 4 and following.

3c. To start the app, press the IIS Express button at the top of Visual Studio. Currently, the application has been extensively tested on Chrome and works satisfactorily.

3d. If only the Test database will be used, skip to 7 to learn how to use the application.

4. Before using the SQL version of the application, please run the SQL files present in MovieLibrary/Movie Web App/sql.

4a. The files were written and created in MS SQL Server Management Studio. 

4b. Please ensure you are connecting to MS SQL Server using localhost credentials.

5. The order to execute the files is as follows:
    1. MovieLibraryCreate.sql
    2. MovieLibrarySampleData.sql
    3. MovieLibrarySecurity.sql
    4. MovieLibrarySprocs.sql

6. Now you are ready to use the SQL Database. Please switch the key listed in step 3 to "ADO" if you have not done so already and start the application. 

7. Upon starting up the application, you will see a navbar at the top left. This can be used to return to the main screen at any time.

8. The Add Movie button allows a movie to be added to the database once the necessary data is filled out. 

8a. Once that page is filled and validates correctly, press Add Movie on the Add Movie page to finalize adding it to the database.

8b. press Cancel at any time to return to the main screen.

9. Next, you should see Search, Title, and Search Term. 

9a. Pressing Search without any search terms will retrieve all movies in the respective database. 

9b. Clicking on Title will allow you to modify the type of search to perform. Currently, one can search by Title, Rating (G, PG, PG-13, etc), Director, and Release Year.

9c. Once results have appeared, they can be ordered in ascending or descending order by clicking the column header (EX. Clicking on Title will order by title, Director by           director, etc). Currently, Title, Release Date, Director, Thumbs Up, and Thumbs Down can be ordered.

9d. Clicking on the Thumbs Up or Thumbs Down column for a given movie row will increment on the frontend as well as the backend, without refresh.

9e. To bring up the Details page, click on the Title column for a given movie row. 

10. On the Details page, the Thumbs Up and Thumbs Down values can be altered by clicking on the row in which they appear. For example, clicking on the label or the number will increment the value. 

11. Press Edit to go to the Edit Movie page for a given movie after searching. 

12. Once values are changed and validate correctly, press the Edit Movie button to confirm edits.

12a. Once again, pressing Cancel at any time will return to the MovieLibrary screen.

13. After searching, pressing Delete will bring up an alert to confirm deletion. 

13a. Pressing OK will delete the movie and bring up a dialog to click through, informing the user of deletion.

13b. Pressing Cancel will halt the operation and erase the alert box.

13c. Modifications to the Test database will be reverted on closing and reopening the app. 

13d. Reverting modifications to the SQL database will require rerunning the MovieLibrarySampleData.sql script.

14. This ends the description of setup and functions.
