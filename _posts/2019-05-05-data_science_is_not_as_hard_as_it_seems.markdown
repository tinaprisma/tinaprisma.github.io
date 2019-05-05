---
layout: post
title:      "Data Science Is Not As Hard As It Seems"
date:       2019-05-05 17:27:00 +0000
permalink:  data_science_is_not_as_hard_as_it_seems
---


This post was originally published here: https://medium.com/@valentina_92897/data-science-is-not-as-hard-as-it-seems-9c886d5920c8

Although data science may seem like a daunting field, a beginner is able to write scripts to accomplish useful tasks within a short timeframe. For the first project at the Flatiron Data Science Immersive, I analyzed the text of Shakespeare’s Macbeth. It was satisfying to have the ability to create an effective script using a couple of basic skills.
Terms like web-scraping and text analysis sound very technical and out of reach for those of us who are not computer scientists. I was pleasantly surprised to find out that, with a bit of effort and some practice, these skills are not difficult to learn.

I started studying data science part-time about three months ago. Fortunately, we live in a time where education is available online! As an educator and entrepreneur, finding an online program offering the flexibility I needed was a true blessing.

My friends have asked me, ‘how are you going to learn such a difficult skill online?’ Well, I would argue that the online format is incredibly more efficient than having to drive somewhere to learn. At the end of the day, writing code is a very intimate task that involves only the computer and a person. Anything outside of that, becomes an external distraction.

Has it been hard? Absolutely not! Learning to code is like learning a new language in many ways. First, you use words, of course. Then, you quickly find out if the person you are talking to understands you or not. The computer tells you in no uncertain terms if your script works or not. Like language, the message may be unskillfully crafted and thus misunderstood. Unlike human-to-human communication, however, computers are objective interpreters and the responsibility lies in the person crafting the message to be extremely precise. (At least for now, who knows what artificial intelligence will do in the future).

For the first mini-project in Flatiron, we were tasked with finding the most common words within the text of Macbeth. To begin, the text was scrapped from Project Gutenberg’s website. How to scrape? Well, it just takes two lines in this case.

import requests
macbeth = requests.get(‘http://www.gutenberg.org/cache/epub/2264/pg2264.txt').text
This script gets the text from gutenberg.org and stores it as a string within the variable ‘macbeth’. After this, we are able to manipulate that string in various ways to complete the text analysis.k

In order to count how frequently a particular word is used in the text, the first thing to do is to split the text into a list of strings where each word becomes one object within the list. Then, we iterate through the list (scan each string at a time), and then an if statement filters whether or not a particular word has passed through the iterator or not. If the answer is no, then we count the word as its first instance. If the answer is yes, we add 1 to the count. It’s quite simple, really.

To visualize the findings of the analysis, I created a simple bar graph. The most common words used in the text are mostly prepositions such as ‘the’, ‘and’, ‘to’, ‘of’, and nouns such as ‘I’, ‘you’, and ‘he’. This is not surprising as this is characteristic of the English language.

![](Although data science may seem like a daunting field, a beginner is able to write scripts to accomplish useful tasks within a short timeframe. For the first project at the Flatiron Data Science Immersive, I analyzed the text of Shakespeare’s Macbeth. It was satisfying to have the ability to create an effective script using a couple of basic skills.
Terms like web-scraping and text analysis sound very technical and out of reach for those of us who are not computer scientists. I was pleasantly surprised to find out that, with a bit of effort and some practice, these skills are not difficult to learn.

I started studying data science part-time about three months ago. Fortunately, we live in a time where education is available online! As an educator and entrepreneur, finding an online program offering the flexibility I needed was a true blessing.

My friends have asked me, ‘how are you going to learn such a difficult skill online?’ Well, I would argue that the online format is incredibly more efficient than having to drive somewhere to learn. At the end of the day, writing code is a very intimate task that involves only the computer and a person. Anything outside of that, becomes an external distraction.

Has it been hard? Absolutely not! Learning to code is like learning a new language in many ways. First, you use words, of course. Then, you quickly find out if the person you are talking to understands you or not. The computer tells you in no uncertain terms if your script works or not. Like language, the message may be unskillfully crafted and thus misunderstood. Unlike human-to-human communication, however, computers are objective interpreters and the responsibility lies in the person crafting the message to be extremely precise. (At least for now, who knows what artificial intelligence will do in the future).

For the first mini-project in Flatiron, we were tasked with finding the most common words within the text of Macbeth. To begin, the text was scrapped from Project Gutenberg’s website. How to scrape? Well, it just takes two lines in this case.

import requests
macbeth = requests.get(‘http://www.gutenberg.org/cache/epub/2264/pg2264.txt').text
This script gets the text from gutenberg.org and stores it as a string within the variable ‘macbeth’. After this, we are able to manipulate that string in various ways to complete the text analysis.k

In order to count how frequently a particular word is used in the text, the first thing to do is to split the text into a list of strings where each word becomes one object within the list. Then, we iterate through the list (scan each string at a time), and then an if statement filters whether or not a particular word has passed through the iterator or not. If the answer is no, then we count the word as its first instance. If the answer is yes, we add 1 to the count. It’s quite simple, really.

To visualize the findings of the analysis, I created a simple bar graph. The most common words used in the text are mostly prepositions such as ‘the’, ‘and’, ‘to’, ‘of’, and nouns such as ‘I’, ‘you’, and ‘he’. This is not surprising as this is characteristic of the English language.

![](https://cdn-images-1.medium.com/max/1200/1*vNCa2OhapRY977Rh3ens9Q.png)

So, you see, thanks to the use of Python libraries, a beginner is able to create useful scripts quickly. If you are thinking about changing your career to data science, it is a good time to make the pivot as it is an emerging career and there are lots of jobs in the market now. Learning the skills necessary, especially if you already have some technical training, is not as difficult as you may imagine it to be.http://)

So, you see, thanks to the use of Python libraries, a beginner is able to create useful scripts quickly. If you are thinking about changing your career to data science, it is a good time to make the pivot as it is an emerging career and there are lots of jobs in the market now. Learning the skills necessary, especially if you already have some technical training, is not as difficult as you may imagine it to be.
