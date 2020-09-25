# My experience with Pandas and Pyspark on the job
In my previous blog post, I discussed some of the challenges I faced with SQL when beginning my new job.  Now, the next challenge was to learn how to perform an analysis without using Pandas dataframes.

Pandas is the tool we use to analyse fairly limited datasets. This is not necessarily from a limitation from Pandas itself, rather, the bottleneck resides in the data extraction step.  If the data scientist wants to use Pandas tools to analyze big data, the first step will be to transform a PySpark dataframe into a Pandas dataframe. Following this step takes an impractical amount of time and requires high memory resources. It is likely that the infrastructure team will start sending angry emails if this is a consistent practice.

So how do we analyze big data, then? We use Spark dataframes. These work in a very different way to Pandas and frankly, I am still learning how to be more effective with them. The syntax and processing flow is very different. 

For one, you can't really QC your dataset as you would normally do when the sample space is more limited. As a scientist, I have been accustomed to make detailed observations of each minute detail on each data point I had. Now as a big data scientist, it's unmanagable to do so. The QC step needs to be automated, and statistical analysis is needed to pinpoint any errors. In addition, errors in a few samples, when you have big data, may be just a feature of your dataset, so your frame of mind needs to shift to think about the bigger picture. Errors become noise in the grander scheme of things.

Secondly, avoid expectations of extreme speed in processing times. Unfortunately, the nature of the distributed processing system means that even a query that outputs just a few results actually can take the same amount of time if you were extracting tens of thousands of samples.  Sometimes it may even take longer than in other, non-distributed systems.

Third, you'll have to study how to analyze data contained in Spark dataframes. A different processing flow will apply as well as different functions and syntax. As of yet, I haven't delved too deep into Spark dataframes because we currently use a different system (Teradata) to extract data, and it doesn't use a Spark context.

There is a recurring theme in my posts --essentially, be prepared to be surprised on your first data science job assignment. You may be asked to focus on things other than machine learning. Queries are going to be the majority of your work. You may not be even using distributed data processing systems at the beginning. Data science mastery is a journey, not a destination. I love how many cliches I have used in these blog posts!
