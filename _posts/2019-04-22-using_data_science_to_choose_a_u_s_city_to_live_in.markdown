---
layout: post
title:      "Using Data Science to Choose a U.S. City to Live In"
date:       2019-04-22 07:07:40 +0000
permalink:  using_data_science_to_choose_a_u_s_city_to_live_in
---


This was originally published on medium.com

https://medium.com/@valentina_92897/using-data-science-to-choose-a-u-s-city-to-live-in-e7c0ec477061


I am going to share with you my first project in data science. I am very excited to be officially ‘done’ because, if all goes well, this is the final step to complete the IBM Data Science Professional Certification (available in Coursera).

An honest (maybe too honest?) caveat: This is the culmination of about three months of part-time study and is by no means the product of an expert. I will also tell you that, considering my other responsibilities, I am proud of what I have done. Why am I saying this? Because I know some of you may need encouragement. It is possible to pivot into another career in your thirties, ladies and gentleman.

Let’s now talk about living in Houston, Texas. Don’t get me wrong; there are many advantages. I moved here after graduating from Stanford for a job as a geophysicist in the oil and gas industry, and it was dandy until I chose to go back to school. This time, it was an MBA.

I did the MBA in Houston for various reasons. After graduation, I started a private tutoring business and got recruited to teach in a local community college. Still in Houston now. I miss California (a lot!).

So back to data science. I discovered this career path gradually. First, I consulted at a local visualization software company while enrolled in the MBA program. This was my first stint with Python. I liked it. So I continued programming as a hobby and as part of the tutoring business. I learned about Arduino and the Hummingbird robotics kits. I organized a coding summer camp for teens. It was a blast.

In this process of discovery, I wondered what I could do with my technical skills and business acumen beyond teaching. I missed the intellectual challenge and frankly, I simply enjoy coding and working with numbers in depth. Then I found out about data science and met with a friend who pivoted from geophysics into this field. I’m grateful for his generosity in sharing tips on how I may embark on a similar journey (Hi, Justin Gosses!).

I soon started the IBM coursework and now I am presenting the final report. Part of the exercise is to incorporate Foursquare data in our analysis, but apart from that, we were given full freedom of choice on the topic to explore.

Since I am a bit ambivalent about living in Houston, I decided to explore data from other cities and see if there was an objective way to evaluate whether or not I would enjoy living somewhere else. Modeling personal preferences, I soon found out, is extremely difficult. Yet, there were some interesting findings that can be shared in brief.

The data from Foursquare, which may be called within a Jupyter notebook using Python, is free to use within a daily quota limit. The limit is quite generous — I never hit the quota even though I downloaded 42 thousand records several times daily for several days.

To download this data, I first chose about 40 U.S. cities of interest and about 20 categories of Foursquare venues such as “park”, “art studio”, “farmers’ market”. These venues were organized into 5 categories, filtered, and formatted appropriately for plotting using Plotly (Fig. 1). Note: for an interactive version of the Notebook, visit here.

Fig 1b. Number of venues matching personal interests in various U.S. cities (continued)

Fig 1b. Number of venues matching personal interests in various U.S. cities (continued)
I was surprised to find New York City on the top of the list. I don’t think of the city as a major outdoorsy location, but when I reflected on it, I do remember visiting many parks and beautiful places on my previous visits. I was not surprised to see several California cities in the top 10.

The next challenge was to scrape temperature and precipitation data from the NOAA.gov climate website. I was happy to find that the data was available for download in CSV format and that the patterns of the URLs were predictable (and thus scriptable). I wrote a couple of functions to download the data to the cloud and then produced a few beautiful plots showing the total annual range of temperatures in the peak of the Summer and Winter seasons (Fig. 2) and total annual precipitation from 2000–2018 (Fig. 3).


Fig. 2. Summer and Winter Temperatures in a select group of U.S. Cities from 2000–2018 (Farenheit, vertical axis).
Based on these data, Austin gets hotter than Houston in the summer (is that really possible?). Denver gets much colder than I thought, too. San Francisco again wins with the mildest, less fluctuating temperatures.


Fig. 3. Total Annual Precipitation (Inches) for various U.S. cities from 2000–2018.
The precipitation data were less exciting. Maybe the plots turned out to be a little boring. But you can see that Houston wins in volume of rain per year. Again, not surprising.

Next, I considered other factors such as effective tax rates and standard of living per dollar in each city. I found out that the effective tax rates tend to be higher in Western states, yet the most striking statistic was this: to have the same standard of living in San Francisco in comparison to Houston, you need to have twice as much dough. That is a HUGE difference.

To elevate the analysis, I chose to create a classification model to predict whether or not, given certain features, I would personally like a city. I used a sample size of 41 cities and two features: number of outdoors venues and number of cultural venues. I trained the model with 32 samples and tested on 9.

The result? Out of the 9 cities tested, 6 were predicted correctly (Fig. 4).


Fig. 4. Confusion matrix showing 6 out of 9 total samples were predicted correctly.
Given that the number of samples and features were limited given data and time available for this analysis, the result was not terrible. It is still an unsatisfactory predictor overall for preference with a log loss value of 0.67.

Am I choosing to move based on this data? Not at the moment. I am still polishing my data science skills (just joined the Flatiron School Data Science Bootcamp). It’s been a worthwhile enterprise to pursue this initial certification, and I hope that this example of a final report may inspire you to think about data science as a more approachable field.

