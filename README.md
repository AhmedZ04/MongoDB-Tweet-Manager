# MongoDB-Tweet-Manager
# Code execution guide
Initialize the MongoDB environment by running "python3 load-json.py <db.json> <port_num>". This will create the MongoDB environment, create a tweets collection and then load tweets into it from the db.json file in batches of 10,000. You should see a succees message in the following format if the DB has been initialized correctly:

"Starting MongoDB server on port 27017 with dbpath: C:\Users\ahmed\MongoDB-Tweet-Manager\mongodb-data-76cacf61
MongoDB server started successfully.
Connected to MongoDB on port 27017
Existing 'tweets' collection dropped.
New 'tweets' collection created.
Inserted the final batch of 100 tweets.
All tweets have been inserted successfully!"

Note: load-json.py will look for the "MongoDB-Tweet-Manager" folder in order to correctly find the MongoDB data directory and initialize the MongoDB environment. If this repository is cloned and then renamed, you need to either change the default value directory_name parameter in the find_assignment_directory function of the load-json.py file to the new name of the folder containing the repository file or rename your folder to "MongoDB-Tweet-Manager".

Once the MongoDB database has been created and initialized, you may simply run the main program by typing "python3 tweet-manager.py" in the command line. Once the program runs, it will prompt you to enter the MongoDB port for the database you want to access. Type in the port that you ran "load-json.py" with here to enter the program and see the command dashboard. Make sure you have Python 3+ installed as the code logic is not designed to work with earlier versions of python.

This code is designed for **Unix-like environments ONLY**. There is no guarantee of it working on Windows or on other operating systems without alterations to the load-json.py logic. 
