Download Link: https://assignmentchef.com/product/solved-ve492-homework-8
<br>
<h1>Question 1: Maximum Likelihood Estimation</h1>

We will begin with a short derivation. Consider a probability distribution with a domain that consists of @ different values. We get to observe total samples from this distribution. We use to represent the number of the samples for which outcome occurs. Our goal is to estimate the probabilities o b b @ b of each of the events. The probability of the last outcome, @, equals b <sup>@ b</sup><sub>ob </sub>.

In <em>maximum likelihood estimation</em>, we choose the that maximize the likelihood of the observed samples,

For this derivation, it is easiest to work with the log of the likelihood. Maximizing log-likelihood also maximizes likelihood, since the quantities are related by a monotonic transformation. Taking logs we obtain

Setting derivatives with respect to           equal to zero, we obtain @        b equations in

That is, the maximum likelihood estimation of can be found by solving a linear system of @ b equations in @ b unknowns. Doing so shows that the maximum likelihood estimate corresponds to simply the count for each outcome divided by the total number of samples. I.e., we have that:

<strong><em>Notice: Please write each sub-question in one row, that is, there will be 3 rows for this question. And please use irreducible fractions for your answer.</em></strong>

<strong><em>Sample Answer:</em></strong>

<strong><em>1,1/2,1/3,1/4</em></strong>

<strong><em>2/5 (instead of 4/10),1/3,4/7 3/8,3/7,3/5</em></strong>

<strong>Part 1.</strong>

Now, consider a sampling process with 3 possible outcomes: R, G, and B. We observe the following sample counts:

<table width="196">

 <tbody>

  <tr>

   <td width="70">outcome</td>

   <td width="42">R</td>

   <td width="42">G</td>

   <td width="42">B</td>

   <td colspan="2" width="359"> </td>

  </tr>

  <tr>

   <td width="70">count</td>

   <td width="42">3</td>

   <td width="42">1</td>

   <td width="42">7</td>

   <td colspan="2" width="359"> </td>

  </tr>

  <tr>

   <td colspan="6" width="556">1)        What is the total sample count    ?2)        What are the maximum likelihood estimates for the probabilities of each</td>

  </tr>

  <tr>

   <td colspan="5" width="294">outcome? o o o<strong>Part 2.</strong></td>

   <td width="262"> </td>

  </tr>

  <tr>

   <td colspan="5" width="294">Now, use <em>Laplace smoothing </em>with strength outcome.ܣწ oܣწ oܣწ o<strong>Part 3.</strong></td>

   <td width="262">o წ to estimate the probabilities of each</td>

  </tr>

  <tr>

   <td colspan="6" width="556">Now, consider Laplace smoothing in the limit . Fill in the corresponding probability estimates.</td>

  </tr>

  <tr>

   <td width="70"></td>

   <td width="42"></td>

   <td width="42"></td>

   <td width="42"></td>

   <td width="98"></td>

   <td width="80"></td>

  </tr>

 </tbody>

</table>

o           ܣo                 ܣo                 ܣ

<h1>Question 2: Poisson Parameter Evaluation</h1>

We will now consider maximum likelihood estimation in the context of a different probability distribution. Under the Poisson distribution, the probability of an event occurring @ o times is:

@ o             t

Here     is the parameter we wish to estimate. The distribution is plotted for several values of         below.

On a sheet of scratch paper, work out the maximum likelihood estimate for , given observations of several .

<strong>Hints</strong>: start by taking the product of the equation above over all the , and then taking the log. Then, differentiate with respect to , set the result equal to 0, and solve for in terms of the .

You observe the samples <sub>b </sub>o t <sub>b </sub>o წ <sub>წ </sub>o t o o b . What is your maximum likelihood estimate of ?

<strong><em>Sample Answer (rounded to 3 decimal places):</em></strong>

<strong><em>0.160</em></strong>

<h2>Question 3: Naive Bayes</h2>

In this question, we will train a Naive Bayes classifier to predict class labels as a function of input features .

We are given the following 15 training points:

<table width="553">

 <tbody>

  <tr>

   <td width="35">b</td>

   <td width="35">1</td>

   <td width="35">1</td>

   <td width="35">1</td>

   <td width="35">1</td>

   <td width="35">1</td>

   <td width="35">1</td>

   <td width="35">1</td>

   <td width="35">0</td>

   <td width="35">1</td>

   <td width="35">1</td>

   <td width="35">1</td>

   <td width="35">0</td>

   <td width="35">1</td>

   <td width="35">1</td>

   <td width="35">0</td>

  </tr>

  <tr>

   <td width="35">b</td>

   <td width="35">0</td>

   <td width="35">0</td>

   <td width="35">0</td>

   <td width="35">1</td>

   <td width="35">0</td>

   <td width="35">0</td>

   <td width="35">0</td>

   <td width="35">0</td>

   <td width="35">0</td>

   <td width="35">1</td>

   <td width="35">0</td>

   <td width="35">0</td>

   <td width="35">0</td>

   <td width="35">0</td>

   <td width="35">1</td>

  </tr>

  <tr>

   <td width="35">წ</td>

   <td width="35">0</td>

   <td width="35">0</td>

   <td width="35">0</td>

   <td width="35">0</td>

   <td width="35">0</td>

   <td width="35">0</td>

   <td width="35">0</td>

   <td width="35">0</td>

   <td width="35">0</td>

   <td width="35">0</td>

   <td width="35">1</td>

   <td width="35">0</td>

   <td width="35">1</td>

   <td width="35">0</td>

   <td width="35">0</td>

  </tr>

  <tr>

   <td width="35"> </td>

   <td width="35">A</td>

   <td width="35">A</td>

   <td width="35">A</td>

   <td width="35">A</td>

   <td width="35">A</td>

   <td width="35">A</td>

   <td width="35">A</td>

   <td width="35">A</td>

   <td width="35">A</td>

   <td width="35">A</td>

   <td width="35">B</td>

   <td width="35">B</td>

   <td width="35">B</td>

   <td width="35">B</td>

   <td width="35">C</td>

  </tr>

 </tbody>

</table>

<strong><em>Note: Please write your answer for each table in one row, that is, there will be 10 rows for this question. Besides, please use values rounded to 3 decimal places.</em></strong>

<strong><em>Sample Answer:</em></strong>

<strong><em>0.160,0.170,0.160</em></strong>

<strong><em>…</em></strong>

<strong><em>…</em></strong>

<strong><em>…</em></strong>

<strong><em>A</em></strong>

<strong><em>…</em></strong>

<strong><em>0.200,0.211,…</em></strong>

<ul>

 <li>What is the maximum likelihood estimate of the prior ?</li>

</ul>

<table width="195">

 <tbody>

  <tr>

   <td width="56"> </td>

   <td width="138"> </td>

  </tr>

  <tr>

   <td width="56">A</td>

   <td width="138"> </td>

  </tr>

  <tr>

   <td width="56">B</td>

   <td width="138"> </td>

  </tr>

  <tr>

   <td width="56">C</td>

   <td width="138"> </td>

  </tr>

 </tbody>

</table>

<ul>

 <li>What are the maximum likelihood estimates of the conditional probability distributions? Fill in the tables below (the second and third are done for you).</li>

</ul>

<table width="521">

 <tbody>

  <tr>

   <td width="167">


    <table width="131">

     <tbody>

      <tr>

       <td width="28">b</td>

       <td width="28"> </td>

       <td width="75">b</td>

      </tr>

      <tr>

       <td width="28">0</td>

       <td width="28">A</td>

       <td width="75"> </td>

      </tr>

      <tr>

       <td width="28">1</td>

       <td width="28">A</td>

       <td width="75"> </td>

      </tr>

      <tr>

       <td width="28">0</td>

       <td width="28">B</td>

       <td width="75"> </td>

      </tr>

      <tr>

       <td width="28">1</td>

       <td width="28">B</td>

       <td width="75"> </td>

      </tr>

      <tr>

       <td width="28">0</td>

       <td width="28">C</td>

       <td width="75"> </td>

      </tr>

      <tr>

       <td width="28">1</td>

       <td width="28">C</td>

       <td width="75"> </td>

      </tr>

     </tbody>

    </table></td>

   <td width="200"></td>

   <td width="154"></td>

  </tr>

 </tbody>

</table>

<ul>

 <li>Now consider a new data point ( <sub>b </sub>o n <sub>b </sub>o n <sub>წ </sub>o b). Use your classifier to determine the joint probability of causes and this new data point, along with the posterior probability of given the new data:</li>

</ul>

<table width="276">

 <tbody>

  <tr>

   <td width="69"> </td>

   <td width="101">b on</td>

   <td width="43">b on</td>

   <td width="63">წ ob</td>

  </tr>

  <tr>

   <td width="69">A</td>

   <td width="101"> </td>

   <td width="43"> </td>

   <td width="63"> </td>

  </tr>

  <tr>

   <td width="69">B</td>

   <td width="101"> </td>

   <td width="43"> </td>

   <td width="63"> </td>

  </tr>

  <tr>

   <td width="69">C</td>

   <td width="101"> </td>

   <td width="43"> </td>

   <td width="63"> </td>

  </tr>

  <tr>

   <td width="69"> </td>

   <td width="101">b on</td>

   <td width="43">b on</td>

   <td width="63">წ ob</td>

  </tr>

  <tr>

   <td width="69">A</td>

   <td width="101"> </td>

   <td width="43"> </td>

   <td width="63"> </td>

  </tr>

  <tr>

   <td width="69">B</td>

   <td width="101"> </td>

   <td width="43"> </td>

   <td width="63"> </td>

  </tr>

  <tr>

   <td width="69">C</td>

   <td width="101"> </td>

   <td width="43"> </td>

   <td width="63"> </td>

  </tr>

 </tbody>

</table>

<ul>

 <li>What label does your classifier give to the new data point? (Break ties alphabetically). Write capital letters only.</li>

 <li>Now use Laplace Smoothing with strength o წ to estimate the prior for the same data.</li>

</ul>

<table width="214">

 <tbody>

  <tr>

   <td width="57"> </td>

   <td width="157"> </td>

  </tr>

  <tr>

   <td width="57">A</td>

   <td width="157"> </td>

  </tr>

  <tr>

   <td width="57">B</td>

   <td width="157"> </td>

  </tr>

  <tr>

   <td width="57">C</td>

   <td width="157"> </td>

  </tr>

 </tbody>

</table>

<ul>

 <li>Use Laplace Smoothing with strength o წ to estimate the conditional probability distributions below (again, the second two are done for you).</li>

</ul>

<table width="446">

 <tbody>

  <tr>

   <td width="170">


    <table width="153">

     <tbody>

      <tr>

       <td width="31">b</td>

       <td width="36">Y</td>

       <td width="87">b</td>

      </tr>

      <tr>

       <td width="31">0</td>

       <td width="36">A</td>

       <td width="87"> </td>

      </tr>

      <tr>

       <td width="31">1</td>

       <td width="36">A</td>

       <td width="87"> </td>

      </tr>

      <tr>

       <td width="31">0</td>

       <td width="36">B</td>

       <td width="87"> </td>

      </tr>

      <tr>

       <td width="31">1</td>

       <td width="36">B</td>

       <td width="87"> </td>

      </tr>

      <tr>

       <td width="31">0</td>

       <td width="36">C</td>

       <td width="87"> </td>

      </tr>

      <tr>

       <td width="31">1</td>

       <td width="36">C</td>

       <td width="87"> </td>

      </tr>

     </tbody>

    </table></td>

   <td width="275"></td>

  </tr>

 </tbody>

</table>

<ul>

 <li>Now consider again the new data point ( <sub>b </sub>o n <sub>b </sub>o n     <sub>წ </sub>o b ). Use the</li>

</ul>

Laplace-Smoothed version of your classifier to determine the joint probability of causes and this new data point, along with the posterior probability of given the new data:

<table width="276">

 <tbody>

  <tr>

   <td width="69"> </td>

   <td width="101">b o n</td>

   <td colspan="2" width="50">b o n</td>

   <td colspan="2" width="57">წ o b</td>

  </tr>

  <tr>

   <td width="69">A</td>

   <td width="101"> </td>

   <td colspan="2" width="50"> </td>

   <td colspan="2" width="57"> </td>

  </tr>

  <tr>

   <td width="69">B</td>

   <td width="101"> </td>

   <td colspan="2" width="50"> </td>

   <td colspan="2" width="57"> </td>

  </tr>

  <tr>

   <td width="69">C</td>

   <td width="101"> </td>

   <td colspan="2" width="50"> </td>

   <td colspan="2" width="57"> </td>

  </tr>

  <tr>

   <td width="69"> </td>

   <td colspan="2" width="102">b o n</td>

   <td colspan="2" width="50">b o n</td>

   <td width="55">წ o b</td>

  </tr>

  <tr>

   <td width="69">A</td>

   <td colspan="2" width="102"> </td>

   <td colspan="2" width="50"> </td>

   <td width="55"> </td>

  </tr>

  <tr>

   <td width="69">B</td>

   <td colspan="2" width="102"> </td>

   <td colspan="2" width="50"> </td>

   <td width="55"> </td>

  </tr>

  <tr>

   <td width="69">C</td>

   <td colspan="2" width="102"> </td>

   <td colspan="2" width="50"> </td>

   <td width="55"> </td>

  </tr>

  <tr>

   <td width="69"></td>

   <td width="101"></td>

   <td width="2"></td>

   <td width="48"></td>

   <td width="2"></td>

   <td width="55"></td>

  </tr>

 </tbody>

</table>

<ul>

 <li>What label does your (Laplace-Smoothed) classifier give to the new data point? (Break ties alphabetically). Write a single capital letter.</li>

</ul>

<h2>Question 4: Datasets</h2>

When training a classifier, it is common to split the available data into a training set, a hold-out set, and a test set, each of which has a different role.

<strong><em>Sample Answer:</em></strong>

<strong><em>A</em></strong>

<strong><em>A</em></strong>

<strong><em>A</em></strong>

<ul>

 <li>Which data set is used to learn the conditional probabilities?

  <ol>

   <li>Training Data</li>

   <li>Hold-Out Data</li>

   <li>Test Data</li>

  </ol></li>

 <li>Which data set is used to tune the Laplace Smoothing hyperparameters?

  <ol>

   <li>Training Data</li>

   <li>Hold-Out Data</li>

   <li>Test Data</li>

  </ol></li>

 <li>Which data set is used for quantifying performance results?

  <ol>

   <li>Training Data</li>

   <li>Hold-Out Data</li>

   <li>Test Data</li>

  </ol></li>

</ul>

<h2>Question 5: Linear Separability</h2>

Consider the data in the figure below.

The data is plotted as a function of two features, <sub>b </sub>and <sub>b</sub>. As plotted, the data is not linearly separable. Which of the following candidate features <sub>წ </sub>, when added, would cause the data to be linearly separable? Choose all possible answer(s).

<ol>

 <li>წ o b</li>

 <li><sub>წ </sub>o sin  <sub>b</sub></li>

 <li>წ o b<sub>b </sub>b<sub>b</sub></li>

 <li>წ o bb</li>

 <li>წ o b</li>

 <li><sub>წ </sub>o b</li>

 <li><sub>წ </sub>o <sub>b </sub>b</li>

 <li><sub>წ </sub>o b if <sub>b </sub>䁮 䁮쳌 and <sub>b    </sub>䁮 䁮 n            香䁥   ā</li>

</ol>