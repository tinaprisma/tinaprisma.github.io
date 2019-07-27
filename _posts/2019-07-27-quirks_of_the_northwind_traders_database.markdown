---
layout: post
title:      "Quirks of the Northwind Traders Database"
date:       2019-07-27 21:12:14 +0000
permalink:  quirks_of_the_northwind_traders_database
---

Original post here:
https://medium.com/@valentina_92897/quirks-of-the-northwind-traders-database-3504ddb7646d

In 1992, Microsoft created a company database from a fictitious company, Northwind Traders, to provide its newly-released MS Access users with a test case. The database contains several tables describing the company’s international trade of grocery goods. Because it is an open-sourced dataset, it has been widely used since then as an economic way to practice queries in various applications.
What is less well understood is whether the database contains realistic data or just mumbo-jumbo. Were the developers involved in generating the numerical data in a hurry or did they embed more thought into their task?
To answer this question, I used statistics to analyze several queries on a SQL version on this data. The first concerned whether products were differently priced for different markets around the world. The answer was, well, disappointing yet not surprising. The price distributions were strikingly similar no matter which region of the world I researched.

Results from the two sample t-tests. No significant difference exists between the distributions.
What about delivery wait times? The database includes dates for product order and delivery dates, so the wait times were easily calculated using some dataframe magic. The results, while also disappointingly similar, had a couple of interesting examples. Number of deliveries around the world varied from thousands to less than hundreds. Deliveries to the British Isles were very limited. Even in this scenario, given enough t-test trials, the mean p-value obtained is still above the significant level, indicating that essentially, the distributions are not different.

Results from the two-sample t-tests. No significant difference was found
The developers were likely aware of this boring quality of the dataset. My guess is that they were more interested in quickly generating an example for marketing and educational purposes and moving on to more pressing work.
Nevertheless, it is nice to have an open-sourced dataset to work with. That said, I think it would be beneficial for bootcamps and others to use datasets with more realistic insights to be gained so to keep students more engaged!
