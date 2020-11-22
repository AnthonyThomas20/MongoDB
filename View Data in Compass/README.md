## View data in MongoDB Compass ##

1. On the cluster section of the Atlas homepage, click on Connect button.
2. Click on "Connect your application".
3. Change DRIVER and VERSION according to requirement. I didn't change anything though and left it as it is. (In my case, DRIVER: Node.js and VERSION: 3.6 or later.
4. Copy the given command. It looks something like this: 
mongodb+srv://analytics:<password>@mflix.dfpey.mongodb.net/<dbname>?retryWrites=true&w=majority
5. Change <password> to your password.
6. Open MongoDB compass and click on Connect.
7. Paste the above modified command into the given dialog box and click Connect. 
8. Four databases are loaded where mflix containing our data is one of them.
  
It will look something like this:

![image](https://user-images.githubusercontent.com/54772502/99899769-ea8f9f00-2cd1-11eb-8748-97948bdc6626.png)

Clicking on mfix -> movies_initial we can observe our data in Compass.

![image](https://user-images.githubusercontent.com/54772502/99899864-5eca4280-2cd2-11eb-85d3-4a0380dcb1a9.png)
