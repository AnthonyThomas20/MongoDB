## Aggregation framework to summarize the values in the language field ##

1. **$group stage** - The identifier first stage, always begins with the dollar sign. 
A group stage groups its input documents by a specified identifier expression and applies any accumulator expressions supplied to each group. 
This identifier expression stipulates that we want each group produced to be identified by a dictionary containing a single field. 

2. The key for this field should be the string, language, and the value should be a distinct $language value. 
This type of expression in the MongoDB aggregation framework is a field path identifier. 

3. So for every distinct value of language in this collection, this pipeline will create a group and apply the specified accumulator to this group. 

4. Aggregate is being run on our movies_initial collection. Each document in the collection will be passed through this group stage. 
 
5. **$sum** - This expression means that for every document matching the identifier for a group, add one to a running count of the documents grouped around that identifier. 
 
6. Once all input documents have been processed through this group stage, the stage will admit as output one document for each group. 
Each of those documents will contain two fields an _id field specifying the distinct value for a language that group represents, 
and a count field that contains the number of documents in that group. 

7. The last statement in this script is our call to the **aggregate method.** 
Note that we're using our client connection to access the mflix database attribute of this connection and the movies_initial attribute of the mflix database. 
Finally, we're calling the aggregate method of movies_initial. 

8. Just two other things I want to point out:
I'm using the pprint package so that we can print out nicely formatted output
and importing this clear output function so that we can run this as many times as we like, and each time the prior output will be cleared for us. 

9. Given the way we've structured this pipeline, the result is the output of hundreds of documents, 
each representing a distinct value for language and the count of the number of documents in the movies_initial collection that have that value for language. 

10. This isn't as useful as it could be and doesn't address our question of how many distinct document values 
there are in any real useful way. In order to do that, we'll need to expand our pipeline with a couple more stages.
