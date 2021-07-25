# **Applying Benfords's Law to Image Tampering**

**Table of Contents:** 
1. Introduction
2. Question and Hypothesis
3. Benford's Law
4. Workflow
5. Analysis and Findings
6. References

**1. Introduction**

Benford’s Law, also known as the Law of First Digits, named after physicist Frank Benford, who worked on the theory in 1938. The mathematical theory is based on the findings that the probabilities of first digits are not uniformly distributed so that each of the digits from 1 to 9 is equally likely to appear. Instead, the first digits are arranged in such a way that the digit 1 is the most frequent, followed by 2, 3, and so in a successively decreasing manner down to 9. More precisely, the law gives a prediction of the frequency of leading digits using base-10 logarithms that predicts specific frequencies which decrease as the digits increase from 1 to 9. Attached below in a graph and a table which demonstrate the distribution of Benford's Law (figure i and figure ii). 

Figure i: 
Figure ii:
Insert Graph and table 

Benford’s Law can recognize the probabilities of highly likely or highly unlikely frequencies of numbers in a large numeric data set. Those who are not aware of this theory and intentionally manipulate numbers (e.g., in a fraud) are susceptible to getting caught by the application of Benford’s Law. In the real world, Benford's Law can be applied to financial statements, 
The application of image tampering will be furthur explored during this project.

**2. Question and Hypothesis**

Question: Can the tampering of images be predicted based on their DCT coefficients following Benford's Law. 

H0 (null hypothesis): The tampering of an image can be predicted with Benford's law. 
H1 (alternate hypothesis): The tampering of an image cannot be predicted with Benford's law. 

**3. Benford's Law**



**4. Workflow**

o track and monitor the workflow for this project, a trello board was used. The process started with finding a topic and a database that would be able to answer my questions. This database was based through data cleaning and wrangling with python, to then be firstly explored within python and then passed into tableau. Once trends, questions and possible graphics were identified, the next step was to try to explain the data through a story using a dashboard.

Trello board: https://trello.com/b/UodgngIy/ironhack-final-project

**6. References**

dataset:  I. Amerini, L. Ballan, R. Caldelli, A. Del Bimbo, G. Serra. “A SIFT-based forensic method for copy-move attack detection and transformation recovery”, IEEE Transactions on Information Forensics and Security, vol. 6, issue 3, pp. 1099-1110, 2011. 

