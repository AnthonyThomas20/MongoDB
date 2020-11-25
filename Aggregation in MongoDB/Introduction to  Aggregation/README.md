## Introduction to Aggregation ##

1. The aggregation framework is a set of analytics tools within MongoDB, that allow you to run various types of reports or analysis on documents in one or more MongoDB collections. 
2. The aggregation framework is based on the concept of a pipeline. 
3. The idea with an aggregation pipeline is that we take input from a MongoDB collection and pass the documents from that collection through one or more stages, 
each of which performs a different operation on its inputs.  
And the inputs and outputs for all stages are documents,i.e. a stream of documents. 
4. An individual stage of an aggregation pipeline is a data processing unit. 
5. Each stage takes a stream of input documents, one at a time, processes each document one at a time, and produces an output stream of documents. Again, one at a time. 
6. And finally, at the end of the pipeline, output is produced that we can then do something with in our application. 

