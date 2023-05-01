Download Link: https://assignmentchef.com/product/solved-ch231a-assignment11-longest-ordered-subarray
<br>
<h1></h1>

Consider the array <em>A </em>= (<em>a</em><sub>1</sub><em>,a</em><sub>2</sub><em>,…,a<sub>n</sub></em>). We call a subarray a succession of numbers in A where the position of any value in the subarray in the array is always bigger than the value of the previous one. Use dynamic programming to find a subarray of maximal ordered length of the array <em>A</em>. You can assume there are no duplicate values in the array. Your algorithm should find one optimal solution if multiple exist.

<h2>Example</h2>

For <em>A </em>= (8<em>,</em>3<em>,</em>6<em>,</em>50<em>,</em>10<em>,</em>8<em>,</em>100<em>,</em>30<em>,</em>60<em>,</em>40<em>,</em>80) the solution is: (3<em>,</em>6<em>,</em>10<em>,</em>30<em>,</em>60<em>,</em>80)

Your program should take an input and generate an output as follows: <strong>Sample input</strong>

8 3 6 50 10 8 100 30 60 40 80

<h2>Sample output</h2>

3 6 10 30 60 80

You can assume that the type of the input will be valid.

Your solution will be graded using multiple testcases, therefore following the input and output format is mandatory.

<h1><strong>Problem 11.2 </strong>Sum in triangles</h1>

Consider a triangle formed from <em>n </em>lines (1 <em>&lt; n </em>≤ 100), each line containing natural numbers in the interval [0<em>,</em>10000].

<ul>

 <li>(5 points) Use dynamic programming to determine the biggest sum of numbers existent on the path from the number in the first line and a number from the last line and print the respective path to the output. Each number in this path is seated to the left or to the right of the other value above it.</li>

 <li>(2 point) Analyze the runtime of your solution and compare it to the brute force approach.</li>

 <li>(1 point) Explain why a greedy algorithm does not work for this problem.</li>

</ul>

<h2>Example</h2>

The values are displayed for example in this manner:

7

3        8

8        1        0

2        7        4        4

4         5        2        6        5

For this example the resulting sum is 30.

Your program should take an input and generate an output as follows:

<h2>Sample input</h2>

7

3 8

8 1 0

2 7 4 4 4 5 2 6 5

<h2>Sample output</h2>

30

7 3 8 7 5

You can assume that the input will be valid.

Your solution will be graded using multiple testcases, therefore following the input and output format is mandatory.

<h1><strong>Bonus Problem 11.3 </strong>Scuba Diver</h1>

A scuba diver uses a special equipment for diving. He has a cylinder with two containers: one with oxygen and the other with nitrogen. Depending on the time he wants to stay under water and the depth of diving the scuba diver needs various amount of oxygen and nitrogen. The scuba diver has at his disposal a certain number of cylinders. Each cylinder can be described by its weight and the volume of gas it contains. In order to complete his task the scuba diver needs specific amounts of oxygen and nitrogen. Theoretically, the diver can take as many cylinders as he wants/needs. Use dynamic programming to find the minimal total weight of cylinders he has to take to complete the task and which those cylinders are. In case of several acceptable solutions, printing just one of them is enough.

<h2>Example</h2>

The scuba diver has at his disposal 5 cylinders described below. Each description consists of: volume of oxygen, volume of nitrogen (both values are given in liters) and weight of the cylinder (given in decagrams):

3 36 120

10 25 129

5 50 250

1 45 130

4 20 119

If the scuba diver needs 5 liters of oxygen and 60 liters of nitrogen then he has to take two cylinders of total weight 249 (for example the first and the second ones or the fourth and the fifth ones).

<h2>Input</h2>

The number of test cases <em>c </em>is in the first line of input, then <em>c </em>test cases follow separated by an empty line. In the first line of a test case there are two integers <em>t</em>, <em>a </em>separated by a single space, 1 ≤ <em>t </em>≤ 21 and 1 ≤ <em>a </em>≤ 79. They denote volumes of oxygen and nitrogen respectively, needed to complete the task. The second line contains one integer <em>n</em>, 1 ≤ <em>n </em>≤ 1000, which is the number of accessible cylinders. The following <em>n </em>lines contain descriptions of cylinders; <em>i</em><sup>th </sup>line contains three integers <em>t<sub>i</sub></em>, <em>a<sub>i</sub></em>, <em>w<sub>i </sub></em>separated by single spaces, (1 ≤ <em>t<sub>i </sub></em>≤ 21, 1 ≤ <em>a<sub>i </sub></em>≤ 79, 1 ≤ <em>w<sub>i </sub></em>≤ 800). These are respectively: volume of oxygen and nitrogen in the <em>i</em><sup>th </sup>cylinder and the weight of this cylinder.

<h2>Output</h2>

On the first line will be printed the total weight <em>w<sub>t </sub></em>and on the next line separated by spaces the index of the cylinders in order.

<h2>Sample input</h2>

1

5 60

5

3 36 120

10 25 129

5 50 250

1 45 130

4 20 119

<h2>Sample output</h2>

249

1 2

You can assume that the input values will fall in the ranges from before and you do not have to validate the input or repeat entering values.