## MongoDB ##

MongoDB is a cross-platform, document oriented database that provides, high performance, high availability, and easy scalability. 
MongoDB works on concept of collection and document.

**Database**

1. Database is a physical container for collections. 
2. Each database gets its own set of files on the file system. 
3. A single MongoDB server typically has multiple databases.

**Collection**

1. Collection is a group of MongoDB documents. 
2. It is the equivalent of an RDBMS table. 
3. A collection exists within a single database. 
4. Collections do not enforce a schema. 
5. Documents within a collection can have different fields. Typically, all documents in a collection are of similar or related purpose.

**Document**

1. A document is a set of key-value pairs. 
2. Documents have dynamic schema. Dynamic schema means that documents in the same collection do not need to have the same set of fields or structure, 
and common fields in a collection's documents may hold different types of data.

**Sample Document**

Following example shows the document structure of a blog site, which is simply a comma separated key value pair.

![image](https://user-images.githubusercontent.com/54772502/99897939-b1e8c900-2cc3-11eb-92d3-8c73f1b553bf.png)

*Reference* - https://www.tutorialspoint.com/mongodb/mongodb_overview.htm

*Please start navigating from Atlas Free-Tier Cluster in this repository.*
