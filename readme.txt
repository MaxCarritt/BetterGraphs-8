1. Import the zip file into your project.

2a. If you are using MySQL as your projects database:
Under Vison Windows, open BetterGraphs/BG_Setup.
Put your designer in full read write mode (project drop down menu). Place the window into preview mode.
Click the "Create tables in MySQL database" button. Click yes on all the prompts. 
Now that the tables are created, go to step 3. 

2b. If you're not using MySQL, you will need to adapt the included sql queries to your database, and create the tables yourself. 

3. Optional: You will probably want to make your clients clear their graphs on client startup, so that anything done in the designer doesn't show up when a client is opened.
Go to Vision\Client Events. 
Add "project.BetterGraphs.clearGraphPoints()" to your startup client event script.

4. Set Project Properties in designer to allow Legacy Database Access. 

5. Use the "Add Trend Icon" template in your templates and windows. Just pass it any historized tag path (it must be a string representation of the tag path, don't bind it directly to a tag.) Right click on that icon to add points to your graph. 

