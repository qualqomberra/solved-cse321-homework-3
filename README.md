Download Link: https://assignmentchef.com/product/solved-cse321-homework-3
<br>
<ol>

 <li>Derive recurrence relations of the following algorithms and solve themto decide the complexity of the algorithms. Which algorithm would you prefer for the same problem, elaborate your answer.

  <ul>

   <li>Algorithm alg1(L[0..n-1])</li>

  </ul></li>

</ol>

if (n==1) return L[0] else tmp = alg1(L[0..n-2]) if (tmp&lt;=L[n-1]) return tmp else return L[n-1]

<ul>

 <li>Algorithm alg2(X[l..r])</li>

</ul>

if (l==r) return X[l] else flr = floor((l+r)/2) tmp1 = alg2(X[l..flr]) tmp2 = alg2(X[flr+1..r]) if (tmp1&lt;=tmp2) return tmp1 else return tmp2

<ol start="2">

 <li>You are given a polynomial <em>p</em>(<em>x</em>) like</li>

</ol>

<em>p</em>(<em>x</em>) = <em>a<sub>n</sub>x<sup>n </sup></em>+ <em>a<sub>n</sub></em>−<sub>1</sub><em>x<sup>n</sup></em><sup>−1 </sup>+ <em>… </em>+ <em>a</em><sub>1</sub><em>x </em>+ <em>a</em><sub>0</sub><em>,</em>

and you are supposed to write a brute-force algorithm for computing the value of the polynomial at a given point <em>x</em><sub>0</sub>. Analyze the complexity of your brute-force algorithm, and discuss whether it is possible to design an algorithm that has better complexity. Don’t forget to implement your algorithm in Python.

<ol start="3">

 <li>You are asked to design a brute-force algorithm that counts the number ofsubstrings that start with a specific letter and end with another letter in a given text. For example, let the first letter be ’X’ and the last letter be ’Z’, there are four such substrings in TXZXXJZWX. Write your brute-force algorithm, analyze its complexity, and implement in Python.</li>

</ol>

1

<ol start="4">

 <li>A metric space consists of a set and a distance function. We are given ametric space that is made up of a set of <em>n </em>points in <em>k</em>-dimensional space and Euclidean distance function. Design a brute-force algorithm that gives the distance between the closest pair of points, and find the complexity of the algorithm.</li>

 <li>Profit rates of many companies have changed due to the epidemic. XYZis a retail company with many branches on the Marmaray line. The management of the company is trying to identify the regions where they make the most profit. For this purpose, they gather the profit-loss rates of their retail shops to the table. Entries on the table are sorted in Marmaray station order.

  <ul>

   <li>Write a brute-force algorithm that can find <strong>the most profitable cluster</strong>, provided that the cluster must contain a consecutive region. Explain the time complexity of the algorithm. For example, the most profitable cluster is (C-D-E-F) on table below.</li>

   <li>Write a divide and conquer algorithm that <strong>finds the maximum profit </strong>that belongs to the most profitable cluster (the cluster must contain a consecutive region), analyze its complexity, and write the Python code of the algorithm. For example, the maximum profit is 14 (C-D-E-F) on table below.</li>

  </ul></li>

</ol>

<table width="366">

 <tbody>

  <tr>

   <td width="52">A</td>

   <td width="52">B</td>

   <td width="52">C</td>

   <td width="52">D</td>

   <td width="52">E</td>

   <td width="52">F</td>

   <td width="52">G</td>

  </tr>

  <tr>

   <td width="52">3</td>

   <td width="52">-5</td>

   <td width="52">2</td>

   <td width="52">11</td>

   <td width="52">-8</td>

   <td width="52">9</td>

   <td width="52">-5</td>

  </tr>

 </tbody>

</table>