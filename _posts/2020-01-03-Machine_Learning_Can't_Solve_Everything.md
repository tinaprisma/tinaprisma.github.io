
I had great fantasies at the beginning of my new job about creating complex classification machine learning models to answer some of the most pressing questions in my field.

Then I woke up to find:

- No labels for the model training step
- Data without normal distributions
- Unclear definition of signal vs. noise

### No labels for the model training step

My role as manager in the transaction monitoring team is to come up with logic to detect out of pattern transactions for a major credit card company. We are not looking for fraud. Detecting fraud is relatively easier, subce once you detect it, you have a label. For us, we might never find out what the case outcome is. 

Without labels, there is no training data. 

### Data without normal distributions

Sometimes we deal with data with thousands of features but thousands of records. To reliable use machine learning algorithms, data scientists need access to millions to billions of records. Classification and regression algorithms work only when the data is normally distributed, and usually this occurs once the sample is large enough. A smaller sample space usually means non-normal data, thus, the use of statistics should be limited to non-parametric methods.

### Unclear definition of signal vs. noise

The type of transactions we are looking for are usually related to human behaviors that have an undetermined goal. What distinguishes a normal transaction vs an abnormal transaction pattern? This is a very difficult question to answer when we do not know the intent of the transacting party.

### So how do I accomplish anything at my job?

I am learning the myriad ways in which transactions are used. I am using my own experience in the business world and frankly, I am reading about the habits of certain people.  I have been surprised to find out what  transactional patterns may elucidate about a particular party. In some instances, we are succesful. In many, we are not sure what the outcome of our investigations are. In the process, though, we are looking. So keep that in mind! 
