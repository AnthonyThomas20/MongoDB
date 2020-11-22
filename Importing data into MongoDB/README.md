## Importing data into MongoDB ##

We will use the movies_initial.csv which contains data for 46,014 movies which we will load into our free tier cluster "mflix" we just created.

1. In the Atlas page, under Clusters section, click on Connect button. In the dialog box that appears, click on "Connect with mongo shell".
2. Select "I have the mongo shell installed". Select mongo shell version. I selected 3.4 or later in my case.
3. Copy the given command.

It looks something like this:

mongo "mongodb://mflix-shard-00-00.dfpey.mongodb.net:27017,mflix-shard-00-01.dfpey.mongodb.net:27017,mflix-shard-00-02.dfpey.mongodb.net:27017/<dbname>?replicaSet=atlas-ku9fmk-shard-0" --ssl --authenticationDatabase admin --username analytics --password <password>

Make changes to mongoimport command based on the above copied command as follows:
1. Copy the cluster name that appears after replica set and place it in <CLUSTER> of the mongoimport command.
2. Copy the seed list that appears after :// till the /<dbname>
3. Change the password according to the password you have set.

Run the modified command in the terminal and ensure that the csv file is in the same destination.

You should get the following output.
