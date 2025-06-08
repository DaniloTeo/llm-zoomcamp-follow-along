## Q1. Running Elastic
Run Elastic Search 8.17.6, and get the cluster information. If you run it on localhost, this is how you do it:
`curl localhost:9200`
What's the `version.build_hash` value?
**A: the value is "42f05b9372a9a4a470db3b52817899b99a76ee73"**

## Q2. Indexing the data
Index the data in the same way as was shown in the course videos. Make the course field a keyword and the rest should be text.

Don't forget to install the ElasticSearch client for Python.

pip install elasticsearch
Which function do you use for adding your data to elastic?
**A: index**

## Q3. Searching
Now let's search in our index.

We will execute a query "How do execute a command on a Kubernetes pod?".

Use only question and text fields and give question a boost of 4, and use "type": "best_fields".

What's the score for the top ranking result?
**A: 44.55 more precisely**

## Q4. Filtering
Now ask a different question: "How do copy a file to a Docker container?".

This time we are only interested in questions from machine-learning-zoomcamp.

Return 3 results. What's the 3rd question returned by the search engine?
**A: How do I copy files from my local machine to docker container?**

## Q5. Building a prompt
What's the length of the resulting prompt? (use the len function)?
**A: 2261**


## Q6. Tokens
**A: number of tokens used by Gemini is 557**