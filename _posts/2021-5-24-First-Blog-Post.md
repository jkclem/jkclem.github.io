---
layout: post
title: First Blog Post
---

Given this is my first blog post, I am blogging about something that has had more than enough digital ink spilled over it; data science vs. statistics.

# What do you think being a data scientist is about?  

To me, data science is applied statistics in industry. Some people stress the tools make data scientists different than statisticians, but I disagree. When statisticians stopped calculating statistics by hand, they didn’t stop being statisticians. I don’t see why using Python instead of SAS to implement the same methodology makes one person a data scientist and another a statistician. “Data scientist” jobs typically require more programming ability than traditional statistician jobs, but that is because the development environment is different. 

Some people stress the difference is data scientists are more focused on machine learning, while statisticians only care about inference. I think that is untrue as well. Deep and reinforcement learning typically aren’t taught in statistics departments, but virtually all statistics departments teach classes focused on predictive methods and conduct research into new statistical learning algorithms.

But this is all just my opinion.

# What do you see as the major duties and/or knowledge areas?  

The main duty is to extract value from data. This sounds simple enough, but requires a variety of skills. In my taxonomy, the skills fall into 5 umbrella categories: formalizing the task, data retreival and wrangling, data exploration, analysis, and delivering value.

## Formalizing the Task

You need to be able to formalize the question you need to answer or what you need to predict. Then you need to decide what data you need to accomplish your task. This requires solid consulting skills to get at what your stakeholder really wants to know.

## Data Retrieval and Wrangling

Once you have that in mind, you need to be able to retrieve, clean, and format the data, which will likely involve using SQL for tabular data. You may also need to use a site’s API or scrape the web to set up your own database. Once you have your data, you need to check everything is in the proper format, re-check for missing or strange values and determine how to handle them, and figure out how to handle irregular data types. Ideally, you know how your data is collected, so you are aware of biases in the data collection process.

This is all based on if you are using observational data. If your question requires an experiment like A/B testing, you need to know something of experimental design.

## Data Exploration

You need to know how to produce useful summaries and visualizations of the data. You need to understand the data and how it is distributed.

## Analysis

Once you have your clean formatted data and you’ve gotten a feel for it, you can start using your statistical knowledge to answer your question. Based on the question and the data, you need to decide on a technique. Can ANOVA answer your question? If it’s a prediction problem, is it classification or regression? What is the trade-off between interpretability and predictive performance?

Use a language like Python or R to either answer your question or prototype and evaluate models.

## Delivering Value

Now that you have your answer, give it to the stakeholder. Or if it is a model, productionize it or hand off your research to the team that handles that.

In summary, you need soft skills like consulting and hard skills like data wrangling and analytical ability and be able to express them in languages like SQL, Python, and R.

# What differences/similarities do you see between data scientists and statisticians?  

Data scientist roles might require more programming ability, but I think they are otherwise the same as statistician roles. Just the tools change.

# How do you view yourself in relation to these two areas?

Since I really just think the difference is the tools used, I consider myself in both camps. I use Python and SQL daily, but the problems I work on are solved with statistics.

