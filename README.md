# **Applying Benfords's Law to Image Tampering**

**Table of Contents:** 
1. Introduction
2. Question and Hypothesis
3. Workflow
4. Analysis and Findings
5. References

**1. Introduction**

Benford’s Law, also known as the Law of First Digits, named after physicist Frank Benford, who worked on the theory in 1938. The mathematical theory is based on the findings that the probabilities of first digits are not uniformly distributed so that each of the digits from 1 to 9 is equally likely to appear. Instead, the first digits are arranged in such a way that the digit 1 is the most frequent, followed by 2, 3, and so in a successively decreasing manner down to 9. More precisely, the law gives a prediction of the frequency of leading digits using base-10 logarithms that predicts specific frequencies which decrease as the digits increase from 1 to 9. The formula of a certain digit "d" being the first digit of a number, given by the following equation. Where, P (D = d) is the probability that the first digit is equal to d, and d is an integer ranging from 1 to 9. 

<div style="text-align:center"><img width="555" alt="Formula_Benford" src="https://user-images.githubusercontent.com/83591280/126907220-af2953b7-5261-47d3-bcb1-a505c866e818.png"></div>

Attached below in a graph and a table which demonstrates the distribution of Benford's Law (figure i):

<img width="648" alt="Screen Shot 2021-07-26 at 10 46 26 PM" src="https://user-images.githubusercontent.com/83591280/127056892-0d288e27-b65f-41c7-8049-907249f1c23e.png">

Benford’s Law can recognize the probabilities of highly likely or highly unlikely frequencies of numbers in a large numeric data set. Those who are not aware of this theory and intentionally manipulate numbers (e.g., in a fraud) are susceptible to getting caught by the application of Benford’s Law. In the real world, Benford's Law can be applied to countless data sets such as financial statements, city populations, fibonacci series, elections, music and even in images. This website tests Benford's law in real world scenarios. https://testingbenfordslaw.com/population-of-us-cities-2009. The application of Benford's Law playing a role in the prediction of image tampering will be furthur explored during this project.

All images are composed of thousands of pixel numbers that follow a 8-bit data value with the range of 0 to 255. These numbers can be extracted within python and evaluated with the discrete cosine transform (DCT). DCT is a technique applied to image pixels in spatial domain in order to transform them into a frequency domain in which redundancy can be identified. According to ..., DCT will follow Benford's Law and the more an image has been compressed and tampered the more the first digits skew away from Benford's distribution. In this day and age, images are easily modified and photoshopped which includes cloning, healing, retouching, and splicing, therefore a image tampering identification tool is crucial.

**2. Question and Hypothesis**

Question: Can the tampering of images be predicted based on their DCT coefficients following Benford's Law. 

H0 (null hypothesis): The tampering of an image can be predicted with Benford's law. 
H1 (alternate hypothesis): The tampering of an image cannot be predicted with Benford's law. 

**4. Workflow**

This project was tracked and monitored with a trello board (attached below). The process started with finding a topic and a database that would be able to answer my questions about Benfords's Law and its applications to the real world. The database MICC-F220 was used for this project which is composed by 220 images; 110 are tampered and 110 originals (Amerini et al., 2011). This dataset was made with the objective of being applied to machine learning programs to have a clear distintion of tampered and not tampered images, and therefore is adequate for this model. A extensive code was created to extract the DCT coefficients of each image and calculate the frequency of distribution of first digits. In python, the DCT was only able to be extracted if the dimension of the image was an even number, and for that reason a code was execited to filter on the images with even numbers which reduced the dataset. A dataframe was created in python with the image id, image dataset, frequencies of first digit distribution, and if it was tampered or not. The dataframe was wrangled and explored within python, and then a decision tree machine learning model was applied to predict the tampering of future images. 

Trello board: https://trello.com/b/UodgngIy/ironhack-final-project
Dataset of images: http://www.micc.unifi.it/downloads/MICC-F220.zip

**5. Analysis and Findings**



**6. References and Links**

  I. Amerini, L. Ballan, R. Caldelli, A. Del Bimbo, G. Serra. “A SIFT-based forensic method for copy-move attack detection and transformation recovery”, IEEE Transactions on Information Forensics and Security, vol. 6, issue 3, pp. 1099-1110, 2011. 

