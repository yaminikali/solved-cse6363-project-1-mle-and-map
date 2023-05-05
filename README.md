Download Link: https://assignmentchef.com/product/solved-cse6363-project-1-mle-and-map
<br>
<h1>MLE and MAP</h1>

<ol>

 <li>In class we covered the derivation of basic learning algorithms to derive a model for a coin flip task. Consider a similar problems where we monitor the occurrence of a network event <em>e </em>in a time interval. Assuming that the event’s occurrence is according to a Poisson distribution, we want to learn the best model for the parameter, <em>λ </em>of the distribution given a data set of observed arrival counts. The Poisson distribution for an arrival count <em>k </em>is given by:</li>

</ol>

We are assuming here that the different data points are independent, i.e. that the time intervals that were used to determine them were independently distributed over a longer time interval.

<ol>

 <li>Derive the performance function and the optimization result for analytic MLE optimization for a model learning algorithm that returns the MLE for the parameter <em>λ </em>of the model given a data set <em>D </em>= {<em>k</em><sub>1</sub><em>,…k<sub>n</sub></em>}. Make sure you show your steps.</li>

 <li>Apply the learning algorithm from a) to the following dataset:</li>

</ol>

<em>D </em>= {2<em>,</em>5<em>,</em>0<em>,</em>3<em>,</em>1<em>,</em>3}<em>.</em>

<ol>

 <li>Derive the optimization for a MAP approach using the conjugate prior, the Gamma distribution. The Gamma distribution is:</li>

</ol>

Note that <em>α </em>and <em>β </em>are constants and that there still is only one parameter, <em>λ</em>, to be learned. Show your derivation and the result for the data in part <em>b</em>) and values for <em>α </em>and <em>β </em>of 2 and 1, respectively.

2020 Manfred Huber        Page 1 CSE 6363 – <em>Machine Learning </em>Homework 1: MLE, MAP, and Basic Supervised Learning

<h1>K Nearest Neighbor</h1>

<ol start="2">

 <li>Consider the problem where we want to predict the gender of a person from a set of input parameters, namely height, weight, and age. Assume our training data is given as follows:</li>

</ol>

<em>D </em>= { ((170<em>,</em>57<em>,</em>32)<em>,         W</em>)<em>, </em>((190<em>,</em>95<em>,</em>28)<em>,            M</em>)<em>, </em>((150<em>,</em>45<em>,</em>35)<em>,  W</em>)<em>, </em>((168<em>,</em>65<em>,</em>29)<em>,            M</em>)<em>, </em>((175<em>,</em>78<em>,</em>26)<em>,  M</em>)<em>,</em>

((185<em>,</em>90<em>,</em>32)<em>, M</em>)<em>, </em>((171<em>,</em>65<em>,</em>28)<em>,             W</em>)<em>, </em>((155<em>,</em>48<em>,</em>31)<em>, W</em>)<em>,</em>

((165<em>,</em>60<em>,</em>27)<em>, W</em>)<em>, </em>((182<em>,</em>80<em>,</em>30)<em>,            M</em>)<em>, </em>((175<em>,</em>69<em>,</em>28)<em>, W</em>)<em>, </em>((178<em>,</em>80<em>,</em>27)<em>,            M</em>)<em>, </em>((160<em>,</em>50<em>,</em>31)<em>, W</em>)<em>,</em>

((170<em>,</em>72<em>,</em>30)<em>,        M</em>)<em>, </em>}

<ol start="5">

 <li>Using Cartesian distance as the similarity measurements show the results of the gender prediction for the following data items for values of <em>K </em>of 1, 3, and 5. Include the intermedia steps (i.e. distance calculation, neighbor selection, prediction).</li>

</ol>

(162<em>,</em>53<em>,</em>28)<em>,</em>(168<em>,</em>75<em>,</em>32)<em>,</em>(175<em>,</em>70<em>,</em>30)<em>,</em>(180<em>,</em>85<em>,</em>29)

<ol>

 <li>Implement the KNN algorithm for this problem. Your implementation should work with different training data sets and allow to input a data point for the prediction.</li>

 <li>Repeat the prediction using KNN when the age data is removed (i.e. when only the first two features in the input data are available). Try to determine (using multiple target values) which data gives you better predictions. Show your intermediate results.</li>

</ol>