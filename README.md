# **Applying Benfords's Law to Image Tampering**

**Table of Contents:** 
1. Introduction
2. Question and Hypothesis
3. Benford's Law
4. Workflow
5. Analysis and Findings
6. References

**1. Introduction**


**2. Question and Hypothesis**

The question this project wants to predict if images have been tampered based if their DCT coefficients follow Benford's Law. 

H0 (null hypothesis): A single hypothesis, e.g. an instance or specific candidate model that maps inputs to outputs and can be evaluated and used to make predictions.
H1 (hypothesis): A space of possible hypotheses for mapping inputs to outputs that can be searched, often constrained by the choice of the framing of the problem, the choice of model and the choice of model configuration.


**3. Benford's Law**

Benford’s Law, also known as the Law of First Digits, is based in the finding that the probabilities of first digits are not uniformly distributed so that each of the digits from 1 to 9 is equally likely to appear. Instead, the first digits are arranged in such a way that the digit “1” is the most frequent, followed by “2”, “3”, and so in a successively decreasing manner down to “9”. Attached below in a graph and a table which demonstrate the distribution of Benford's Law. More precisely, the law gives a prediction of the frequency of leading digits using base-10 logarithms that predicts specific frequencies which decrease as the digits increase from 1 to 9. 

Insert Graph and table 


**4. Workflow**

o track and monitor the workflow for this project, a trello board was used. The process started with finding a topic and a database that would be able to answer my questions. This database was based through data cleaning and wrangling with python, to then be firstly explored within python and then passed into tableau. Once trends, questions and possible graphics were identified, the next step was to try to explain the data through a story using a dashboard.

Trello board: https://trello.com/b/UodgngIy/ironhack-final-project

**6. References**

dataset:  I. Amerini, L. Ballan, R. Caldelli, A. Del Bimbo, G. Serra. “A SIFT-based forensic method for copy-move attack detection and transformation recovery”, IEEE Transactions on Information Forensics and Security, vol. 6, issue 3, pp. 1099-1110, 2011. 

