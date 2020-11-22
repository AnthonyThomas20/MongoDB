## MongoDB installation on Windows ##

Install MongoDB Enterprise server from https://www.mongodb.com/try/download/enterprise. 
We need Enterprise server as we need SSL support in order to connect to our Atlas cluster.

I had installed the latest version 4.4.2 (as on creating this file) and found that system requiremnts were not correct which I couldn't configure.
So, I switched to version 3.4.24 which worked completely fine for me. Also do select the checkbox for installing mongoDB Compass during the installation process.

Also add the mongoDB path in the system environment variables which may look like:- C:\Program Files\MongoDB\Server\3.4\bin and move this path to the top. 
Type mongodb --version in the command line to verify the installation.

*Next go to Importing data into MongoDB in this repo.*
