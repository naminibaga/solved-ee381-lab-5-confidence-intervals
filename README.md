Download Link: https://assignmentchef.com/product/solved-ee381-lab-5-confidence-intervals
<br>
Assume that you are measuring a statistic in a large population of size <em>N</em>. The statistic has  mean µand standard deviation σ. Drawing a sample of size <em>n</em>  from the population,

produces a distribution for the sample mean ( <em>X </em>)  with:

<sup>                                                                                         </sup><sup>                   2                      2 </sup>σ<sup>2                                       </sup>σ

<em>E X</em>[ ]=µ µ<em>X                                                                                                                               </em>      and        <em>E X</em>[( −µ σ<em><sub>X </sub></em>) ] = <em><sub>X </sub></em>=  ⇒σ<em><sub>X </sub></em>=     <em>n      </em>

In this project we will explore the relation of <em>X </em>to the population mean µ.

<ul>

 <li>As a first example consider a barrel of a million ball bearings (i.e. population size</li>

</ul>

<em>N </em>=1,000,000) where someone has actually weighed all one million of them and found the exact mean to be µ=100 grams and the exact standard deviation to be σ=12grams. This is obviously an unrealistic assumption, but assume for the time being that these parameters have been measured exactly.

<ul>

 <li>Now pick a sample of size <em>n</em> (for example <em>n</em>=5 ) of bearings from the barrel, weigh</li>

</ul>

<em>X X</em><sup>1 </sup>+ + + +<sup>2 </sup><em>X X</em><sup>3 4 </sup><em>X</em><sup>5</sup>

them and find the mean of the sample, <em>X</em><sub>5 </sub>=                                          .

5

<ul>

 <li>Next take a larger sample (for example <em>n</em>=10) and find the new mean</li>

</ul>

<em><sup>X</sup></em><sub>10 </sub>= <em>X X</em>1 + + +2 L <em>X</em>10 .

10

<ul>

 <li>Continue this process for larger and larger <em>n </em>, until <em>n</em>=</li>

 <li>Plot the points (<em>n X</em>, <em><sub>n</sub></em>)using a point marker (for example a blue ‘x’) as shown in  Figure 1.</li>

</ul>




<ul>

 <li>Next for each value of <em>n </em>, calculate the standard deviation of the sample from σ σ= and plot:</li>

</ul>

σ

<ul>

 <li>The values of µ±96as a function of  <em>n </em>, shown as the red curves in</li>

</ul>

Figure 1a. <em>These curves define the 95% confidence interval, </em>which means that approximately 95% of the sample means will fall within the two red curves in Figure 1a. This can also be visually confirmed by looking at how many of the sample means fall outside of the red curves (approx. 5%). <em> </em>

σ

<ul>

 <li>The values of µ± 58as a function of <em>n </em>, shown as the green curves</li>

</ul>

in the Figure 1b. <em>These curves define the 99% confidence interval, </em>which means that approximately 99% of the sample means fall within the green curves in Figure 1b.




<em> </em>




(a)                                                                       (b)




Figure 1. Sample mean as a function of the sample size




<strong>0.2.</strong> <strong> </strong>

<h3>0.3. Using  the sample mean to estimate the population mean</h3>




In reference to the previous section, it is obviously unrealistic to think that anyone actually measured the exact mean and standard deviation of all one million ball bearings.  More realistically, you would not have any idea what the mean or standard deviation was, and you would need to weigh random samples of different sizes (for example <em>n</em>= 5, 35, or 100bearings) and then draw reasonable conclusions about the weight

distribution of all one million bearings.

To simulate this problem, generate a barrel of a million ball bearings with weights normally distributed, with a mean µ and a standard deviation σ.

As an example, take a sample of <em>n</em> bearings from the population of <em>N </em>=1,000,000.  Then calculate the mean of the sample:




<em>X X</em>1 + + +2 L <em>X</em><em>n</em>

<em>X </em>=

<em>n</em>




The standard deviation of the sample mean can be calculated by:

<em>S</em>ˆ ˆ =(<em>X X</em>− )2 + (<em>X </em>−<em>X </em>)2 + +L (<em>X </em>−<em>X </em>)2 1/2 σ<em>n </em>= , where <em>S </em> 1 2 <em>n </em>

                             <em>n</em>−1                             




The question is: <em>Can the value of X </em><em>, which is calculated for a sample of size n , be used to estimate the mean </em>µ<em>of the population of N </em>=1,000,000<em>bearings?</em>

The answer is given in terms of confidence intervals, typically the 95% and 99% confidence intervals.




<strong><u>Large samples</u> </strong>(<em>n</em>≥ 30)<strong>.</strong>

<em>X </em>−µ

Consider the standardized variable <em>z </em>=. Based on the Central Limit Theorem, it is σ<em><sub>n</sub></em>

known that for large samples the standardized variable <em>z</em> will approach the normal distribution.




<strong>The 95% confidence interval for large samples. </strong><em>The 95% confidence interval</em> is determined by the critical values [−<em>z</em><em><sub>c </sub></em>,<em>z</em><em><sub>c </sub></em>]such that

<em>P</em>{− &lt; &lt;<em>z</em><em><sub>c            </sub>z z</em><em><sub>c</sub></em>}= 0.95

From the tables of the normal distribution it is seen that these critical values correspond to <em>z</em><em><sub>c </sub></em>=1.96 and − −=<em>z</em><em><sub>c </sub></em>1.96. Hence:







<em>P z</em>{− &lt; &lt;<em><sub>c </sub>z z</em><em><sub>c</sub></em>}= 0.95

which is written as

                      <em>X </em>−µ 

⇒<em>P</em> 1.96− &lt;        1.96&lt;  0.95=    <em>P X</em>{⇒ 1.96σ µ−<em><sub>n </sub></em>&lt; &lt; +<em>X </em>1.96σ<em><sub>n</sub></em>} 0.95=

                   σ<em>n                             </em>




  <em>            S</em>ˆ              <em>            S</em>ˆ 

<em>P X</em> −1.96       &lt; &lt; +µ <em>X </em>1.96      = 0.95



<em>       S</em>ˆ If you define:  µ<sub>Lower </sub>= <em>X    </em>1.96−  and µ<sub>Upper </sub>= <em>X         </em>1.96+  , then the above equation is

written as:

<em>P</em>{µ µ µLower &lt; &lt; Upper}= 0.95

This equation can be interpreted as follows:

<em>Based on a sample of size n , we are 95% confident that the mean </em>µ<em>of the population </em>

<em>lies in the interval   </em>[µ µ<sub>Lower </sub><sup>, </sup><sub>Upper</sub>]<em>. </em>

<em> </em>

Another way to interpret this statement is:

<ul>

 <li>Obtain a large number of different samples, of size <em>n</em> each</li>

</ul>

<em>                  S</em>ˆ

<ul>

 <li>For each of these samples calculate <em>X</em> and σ<em><sub>n </sub></em>=</li>

 <li>For each of these samples generate the corresponding intervals</li>

</ul>

[µ µLower , Upper]

<ul>

 <li>Then <em>the mean </em>µ<em>of the population will be contained in 95% of these intervals</em></li>

</ul>




For example if you obtain 500 samples of size <em>n</em> each, and you create the corresponding 500 intervals [µ µ<sub>Lower </sub>, <sub>Upper</sub>], then 475 of these intervals (95% of 500) will contain the population mean µ<em>.  </em>




<strong>The 99% confidence interval for large samples. </strong><em>Similarly, the 99% confidence interval</em> is determined by the  critical values [−<em>z</em><em><sub>c </sub></em>,<em>z</em><em><sub>c </sub></em>]such that

<em>P</em>{− &lt; &lt;<em>z</em><em><sub>c            </sub>z z</em><em><sub>c</sub></em>}= 0.99

From the tables of the normal distribution it is seen that these critical values correspond to <em>z</em><em><sub>c </sub></em>= 2.58 and − −=<em>z</em><em><sub>c </sub></em>2.58.

<em>            S</em>ˆ                        <em>            S</em>ˆ

Hence, if you define:  µ<sub>Lower </sub>= <em>X    </em>2.58−  and µ<sub>Upper </sub>= <em>X  </em>2.58+  , then you can write:

<em>P</em>{µ µ µLower &lt; &lt; Upper}= 0.99

which can be interpreted as follows:

<em>Based on a sample of size n , we are 99% confident that the mean </em>µ<em>of the population </em>

<em>lies in the interval   </em>[µ µ<sub>Lower </sub><sup>, </sup><sub>Upper</sub>]<em>. </em>

<strong><u>Small samples</u> </strong>(<em>n</em>&lt; 30).

<em>X </em>−µ

When the sample size is small, the standardized variable  does not approach the σ<em><sub>n</sub></em>

normal distribution, since the Central Limit Theorem does not hold for small <em>n </em>.

<em>X </em>−µ

In this case the standardized variable  <em>T </em>= follows the <em>Student’s t distribution</em> σ<em><sub>n</sub></em>

with ν=<em>n </em>1− degrees of freedom.




<strong>The 95% confidence interval for small samples. </strong><em>The 95% confidence interval</em> is determined by the critical values [−<em>t</em><em><sub>c </sub></em>,<em>t</em><em><sub>c </sub></em>]such that

<em>P</em>{− &lt; &lt;<em>t</em><em><sub>c           </sub>z  t</em><em><sub>c</sub></em>}= 0.95

Note that the critical values [−<em>t</em><em><sub>c </sub></em>,<em>t</em><em><sub>c </sub></em>]depend on two values: (i) the probability value (0.95) and (ii) the degrees of freedom (ν).

Example: sample size <em>n</em>= 5 . In that case ν= − =<em>n </em>1 4 degrees of freedom. For the 95% confidence interval, the critical value is:   <em>t</em><em><sub>c </sub></em>= <em>t</em><sub>0.975 </sub>2.78=, as seen from the <em>Student’s t distribution</em> tables.

<em>      S</em>ˆ         <em>          S</em>ˆ  Hence, if you define:  µ<sub>Lower </sub>= <em>X   </em>2.78−  and µ<sub>Upper </sub>= <em>X        </em>2.78+  , then the above

equation is written as:

<em>P</em>{µ µ µLower &lt; &lt; Upper}= 0.95

which can be interpreted as follows:

<em>Based on a sample of size n</em>=5<em>, we are 95% confident that the mean </em>µ<em>of the population </em>

<em>lies in the interval   </em>[µ µ<sub>Lower </sub>, <sub>Upper</sub>]<em>. </em>

<strong>The 99% confidence interval small samples. </strong><em>Similarly the 99% confidence interval</em> is determined by the critical values [−<em>t</em><em><sub>c </sub></em>,<em>t</em><em><sub>c </sub></em>]such that

<em>P</em>{− &lt; &lt;<em>t</em><em><sub>c           </sub>z  t</em><em><sub>c</sub></em>}= 0.99

Example: sample size <em>n</em>=5 . In that case ν= − =<em>n </em>1 4 degrees of freedom. For the 99% confidence interval, the critical value is:   <em>t</em><em><sub>c </sub></em>= <em>t</em><sub>0.995 </sub>4.60=, as seen from the <em>Student’s t distribution</em> tables.

<em>      S</em>ˆ         <em>          S</em>ˆ  Hence, if you define:  µ<sub>Lower </sub>= <em>X   </em>4.60−  and µ<sub>Upper </sub>= <em>X        </em>4.60+   , then the above

equation is written as:

<em>P</em>{µ µ µLower &lt; &lt; Upper}= 0.99

which can be interpreted as follows:

<em>Based on a sample of size n</em>= 5<em>, we are 99% confident that the mean </em>µ<em>of the population </em>

<em>lies in the interval   </em>[µ µ<sub>Lower </sub>, <sub>Upper</sub>]<em>.</em>

1. Effect of sample size on confidence intervals

Create two plots as in Figure 1a and Figure 1b, showing the effect on sample size on the confidence intervals.

<strong>The values of the following parameters have been provided to you: </strong>

<ul>

 <li>Total number of bearings: <em>N </em>;</li>

 <li>Population mean: µ (grams);</li>

 <li>Population standard deviation: σ (grams) ;</li>

 <li>Sample sizes: <em>n</em>=1,2,L200</li>

</ul>

<strong>SUBMIT a report </strong>which includes the results and your code. You must follow the guidelines given in the syllabus regarding the structure of the report. Points will  be taken off if you do not follow the guidelines.

<h2>2. Using the sample mean to estimate the population mean</h2>




(A) Perform the following simulation experiment.  Use Table 1 to tabulate the results.

<ol>

 <li>Choose a random sample of <em>n</em>=5 bearings from the N bearings you created in the previous problem. Calculate the sample mean and the sample standard deviation:</li>

</ol>

<em>X </em>=1<sup>∑</sup><em>n X </em><em><sub>j</sub></em>  and <em>S</em>ˆ =

<em><sub>n </sub></em><em>j</em>=1

<ol start="2">

 <li>Create the 95% confidence interval using the normal distribution to fill in the first two entries in the top row. You realize, however, that this is not an appropriate distribution to use because you have a small sample <em>n </em>= 5 30&lt;</li>

</ol>

<em>           S</em>ˆ                  <em>S</em>ˆ

[µ µ<sub>Lower </sub>, <sub>Upper</sub>− =]             [<em>X          </em>1.96+ , <em>X            </em>1.96]

<em>n</em>

<ol start="3">

 <li>Check if the confidence interval includes the actual mean µof the population of N bearings. If it does, then Step 2 is considered a success.</li>

 <li>The appropriate distribution for small samples (<em>n</em>≤30) is the  t-distribution. Create the 95% confidence interval using the t-distribution with ν= − =<em>n     </em>1          4</li>

</ol>

<em>           S</em>ˆ                  <em>S</em>ˆ

[µ µLower , Upper− =]             [<em>X           t</em>0.975+ , <em>X            t</em>0.975]

<em>n</em>

At the 95% confidence level with ν=4 degrees of freedom, the value of <em>t</em><sub>0.975 </sub>can be found from the tables,  and it is  seen to be: <em>t</em><sub>0.975 </sub>= 2.78 . This is the value that will be used to determine  the 95% confidence interval:

<em>            S</em>ˆ                   <em>S</em>ˆ

[µ µ<sub>Lower </sub>, <sub>Upper</sub>− =]              [<em>X </em>2.78+ , <em>X </em>2.78]. For a different sample size,  the values of <em>n</em>

<em>t</em><sub>0.975 </sub>will be different than the ones above. You should find these values from the tdistribution tables, and you should modify the confidence intervals accordingly.

<ol start="5">

 <li>Check if the confidence interval includes the actual mean µof the population. If it does, then Step 4 is considered a success.</li>

 <li>Repeat the experiment for <em>M </em>=10,000times and count the number of successes.</li>

 <li>Enter the percentage of successful outcomes in Table 1.</li>

 <li>Repeat steps 1-7 above with <em>n</em>=5 and 99% confidence interval.</li>

 <li>After completing all of the above steps you will have filled out the first row of the table.</li>

</ol>




<ul>

 <li>Repeat part (A) with <em>n</em>=40 using the normal distribution and the t-distribution to complete the second row of the table.</li>

</ul>




<ul>

 <li>Repeat part (A) with <em>n </em>=120 using the normal distribution and the t-distribution to complete the third row of the table. You realize, however, that for a large sample (<em>n</em>&gt;30 ) the t-distribution will be very close to normal, so the differences between Student’s -t and Normal will be minimal.</li>

</ul>