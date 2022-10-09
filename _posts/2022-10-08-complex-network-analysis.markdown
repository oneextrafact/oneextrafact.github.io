---
layout: posts
title:  "Review - Complex Network Analysis in Python"
date:   2022-10-08 12:15:18 -0400
categories: review
tags: python graph-analysis
---


[Complex Network Analysis in Python][book-url]: Recognize → Construct → Visualize → Analyze → Interpret 

![Book Cover](/assets/images/dzcnapy.jpg)

In 2010, after a vicious snowstorm shut down New York City streets for a few days, citizens started asking questions about how their streets were plowed. This information was stored in a set of WordPerfect docs that had been created almost a generation previously. I was put on a team of Sanitation Department employees to move the information from those documents into a modern format so that we could publish paper and electronic maps. The wrinkle was that the plow instructions were in "street stretch" format. A typical instruction was "Plow on Broadway from 32nd to 28th St". This "on-from-to" (OFT) is a relatively straightforward direction for a plow operator to follow, but not at all straightforward to describe to a computer. There was an existing City API that we could call with OFT, but it could only get one block at a time. The City has over 100,000 blocks! How were 5 people going to do this? 

At the same time I was reading [Contemporary Mathematics][contemporary-url], which I'd had the good fortune to pick up at my local library. I couldn't even tell you why I picked it up, other than a general feeling that I was running into a lot of problems that I didn't have the mental tools to think about it. I'd already used it to solve a thorny problem with "Fair Allocation" (a tale for another time!). As I was thinking about my team's problem - the need to move something along a street stretch between two intersections - it jogged my memory of something called "Graph Theory" from the textbook. I realized that NYC's street network was a massive graph, and I was looking for a special kind of shortest path between two intersections. Not the shortest path between the intersections, but the shortest path that used streets with the name of our target on street. This tool could do everything, including keeping on the path if the name of the street changed for a block or so between the target intersections. I built a tool for the team using networkx in Python, and we were able to get the data we needed in about a month of hard work. I've had a special place in my heart for graph and network analysis ever since. 

And so I've had my eye on Dmitry Zinoviev's book, Complex Network Analysis in Python, for quite some time. I recently had some work at my present job that I thought might benefit from a graph perspective, and I turned to this book for inpsiration. I was very glad that I did! Dmitry has a very engaging style and a knack for intuitive explanations of network analysis concepts. The book includes a lot of practical follow along exercises, including an examination of the Panama Papers and a really neat semantic network of Othello (500 year spoiler alert: Iago is the protaganist!). I learned a lot, especially about metrics such as centrality that can help to find important information with a network. Dmitry makes a strong case for networkx as a primary analysis library, but also provides generous coverage to other tools such as iGraph that could be useful in more specific circumstances. He has great information about network visualization tools such as Gephi that can render much more attractive visualizations of your networks than are currently possible with NetworkX. 

This is not a first Python book, you wouldn't get much out of it without knowing the basics first. But, if you are curious about network analysis and graph theory and want to add these to your toolkit, this would be a great book for you to jump in.


[contemporary-url]: https://www.amazon.com/Contemporary-Mathematics-Business-Consumers-MindTap/dp/0357026446
[book-url]: https://pragprog.com/titles/dzcnapy/complex-network-analysis-in-python/
