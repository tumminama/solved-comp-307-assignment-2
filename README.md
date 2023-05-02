Download Link: https://assignmentchef.com/product/solved-comp-307-assignment-2
<br>



<em>Introduction to </em>AI

<strong> Neural and Evolutionary Learning</strong>

<em>30% of Final Mark </em>

<h1>1       Objectives</h1>

The goal of this assignment is to help you understand the basic concepts and algorithms of neural and evolutionary learning, use these algorithms to perform regression and classification tasks, and analyse the results to draw some conclusions. In particular, the following topics should be reviewed:

<ul>

 <li>Perceptron learning for binary classification,</li>

 <li>Multilayer feed forward neural network architectures and applications,</li>

 <li>Back (error) propagation algorithm and its variations,</li>

 <li>Tackling a problem with an existing neural network package,</li>

 <li>Evolutionary computing and learning paradigms,</li>

 <li>Genetic programming for solving real world applications particularly for regression and binary classification problems, and</li>

 <li>Tackling a problem with an existing genetic programming package.</li>

</ul>

These topics are (to be) covered in lectures 07–12. The online materials can also be checked.

In this assignment, neural networks refer to the standard multilayer feed forward neural networks trained by the back propagation algorithm. Genetic programming refers to the standard genetic programming approach with the tree-like structure for the evolved programs.

<h1>2       Question Description</h1>

<h2>Part 1: Perceptron for Binary Classification [20 marks]</h2>

In this part, you are required to implement and apply the simple Perceptron Learning Algorithm to a binary classification task.

<h3>Data Set</h3>

<table width="423">

 <tbody>

  <tr>

   <td width="105">Instance No.</td>

   <td width="78">Feature 1</td>

   <td width="78">Feature 2</td>

   <td width="78">Feature 3</td>

   <td width="83">Class/Target</td>

  </tr>

  <tr>

   <td width="105">1</td>

   <td width="78">0</td>

   <td width="78">0</td>

   <td width="78">1</td>

   <td width="83">0</td>

  </tr>

  <tr>

   <td width="105">2</td>

   <td width="78">0</td>

   <td width="78">1</td>

   <td width="78">0</td>

   <td width="83">1</td>

  </tr>

  <tr>

   <td width="105">3</td>

   <td width="78">1</td>

   <td width="78">0</td>

   <td width="78">1</td>

   <td width="83">1</td>

  </tr>

  <tr>

   <td width="105">4</td>

   <td width="78">1</td>

   <td width="78">1</td>

   <td width="78">0</td>

   <td width="83">0</td>

  </tr>

  <tr>

   <td width="105">5</td>

   <td width="78">1</td>

   <td width="78">1</td>

   <td width="78">1</td>

   <td width="83">0</td>

  </tr>

  <tr>

   <td width="105">6</td>

   <td width="78">1</td>

   <td width="78">0</td>

   <td width="78">0</td>

   <td width="83">1</td>

  </tr>

  <tr>

   <td width="105">7</td>

   <td width="78">0</td>

   <td width="78">1</td>

   <td width="78">1</td>

   <td width="83">1</td>

  </tr>

  <tr>

   <td width="105">8</td>

   <td width="78">0</td>

   <td width="78">0</td>

   <td width="78">0</td>

   <td width="83">0</td>

  </tr>

 </tbody>

</table>

<h3>Perceptron Algorithm</h3>

The algorithm for learning the weights of the perceptron was given in our lecture is:

<table width="415">

 <tbody>

  <tr>

   <td width="415">Until the perceptron is always right (or some limit):Present an example (+ve or -ve)If perceptron is correct, do nothing If -ve example and wrong(ie, weights on active features are too high) Subtract feature vector from weight vectorIf +ve example and wrong(ie, weights on active features are too low)Add feature vector to weight vector</td>

  </tr>

 </tbody>

</table>

<h3>Requirements</h3>

You can write your program in Java, C/C++, Python, or any other programming language. Note that <strong>you need to write your own code from scratch </strong>in this question.

In this part of the assignment, you should submit:

<ul>

 <li>Program code for your perceptron classifier (both source code and executable program runnable on the ECS School machines).</li>

 <li>Make a training set file with the appropriate format used in your program.</li>

 <li>txt describing how to run your program, and</li>

 <li>A report in PDF, text or DOC format. The report should:

  <ol>

   <li>Report the classification accuracy your perceptron learning algorithm after running 200 epochs.</li>

   <li>Analyse and describe reasons that your algorithm could not achieve better results.</li>

  </ol></li>

</ul>

<h2>Part 2: Neural Networks for Classification [30 marks]</h2>

In this part, you are required to use an existing neural network package to perform classification on the <em>wine </em>data set described below. Please note that you already used this data set in the previous assignment.

<h3>Problem Description</h3>

The <em>wine </em>data set is taken from the UCI Machine Learning Repository (http://archive.ics.uci.edu/ml/datasets.php). The data set contains 178 instances in 3 classes, having 59, 71 and 48 instances, respectively. Each instance has 13 attributes: <em>Alcohol, Malic acid, Ash, Alcalinity </em><em>of ash, Magnesium, Total phenols, Flavanoids, Nonflavanoid phenols, Proanthocyanins, Color </em><em>intensity, Hue, OD280%2FOD315 of diluted wines, Proline</em>. The data set is split into two subsets, one for training and one for testing.

<h3>Requirements</h3>

You should define a neural network architecture for this problem, determine related network learning parameters, use the training set wine-training to learn/train your neural network, then apply the learned/trained neural network to the test set wine-test.

While it is good to write your own program packages to implement the back (error) propagation algorithm for training the multilayer feed forward networks, it might take you quite a while to do so. So we recommend the following neural network simulators (packages) for doing this assignment. One is BPNN (in ANSI C), and one is scikit-learn (or Keras, in Python). More information/instructions for using these packages could be found in the course assignment page.

You can choose any of these existing packages/simulators to perform the task. You can also choose any other package, but please describe your choice in your report.

You should submit the following files electronically.

<ul>

 <li>new training set/test set file(s) with a correct format for the neural network package you have chosen, and</li>

 <li>A report in the PDF, text or DOC formats. The report should:

  <ol>

   <li>Determine and report the network architecture, including the number of input nodes, the numberof output nodes, the number of hidden nodes (assume only one hidden layer is used here). Describe the rationale of your choice.</li>

   <li>Determine the learning parameters, including the learning rate, momentum, initial weight ranges,and any other parameters you used. Describe the rationale of your choice.</li>

   <li>Determine your network training termination criteria. Describe the rationale of your decision.</li>

   <li>Report your results (average results of 10 independent experiment runs with different randomseeds) on both the training set and the test set. Analyse your results and make your conclusions.</li>

   <li>(optional/bonus 5 marks) Compare the performance of this method (neural networks) and the nearest neighbour methods.</li>

  </ol></li>

</ul>

<h2>Part 3: Genetic Programming for Symbolic Regression [30 marks]</h2>

In this part, you are required to use genetic programming to evolve a mathematical function (which is represented as an individual program in the population) for a simple symbolic regression task. In real world applications, a test set of data is needed in many situations but not needed in other scenarios, depending on the nature of the problems to be solved. In this assignment, to make the question simple, it is not required to have a test set — you are just required to evolve a mathematical model to reveal the relationship between the output variable and the input variable(s) from a (training) set of instances.

<h3>Problem Description</h3>

The task involves mapping a single input variable <em>x </em>to the (single) output variable <em>y</em>. In a 2D (twodimensional) space (x-y coordinates), there are 20 points (x-y pairs). The task is to find a mathematical model to describe the relationship between the output variable <em>y </em>and input variable <em>x</em>. The 20 points are as follows. They are also saved in the file regression in plain text format.

<table width="481">

 <tbody>

  <tr>

   <td width="24">x</td>

   <td width="48">-4.4</td>

   <td width="46">-4.2</td>

   <td width="46">-3.3</td>

   <td width="40">-3.0</td>

   <td width="53">-2.2</td>

   <td width="46">-2.4</td>

   <td width="46">-1.2</td>

   <td width="46">-1.6</td>

   <td width="46">-1.0</td>

   <td width="40">-0.5</td>

  </tr>

  <tr>

   <td width="24">y</td>

   <td width="48">5.721</td>

   <td width="46">4.882</td>

   <td width="46">1.685</td>

   <td width="40">1.0</td>

   <td width="53">0.04</td>

   <td width="46">0.119</td>

   <td width="46">0.64</td>

   <td width="46">0.16</td>

   <td width="46">0.956</td>

   <td width="40">2.25</td>

  </tr>

  <tr>

   <td width="24">x</td>

   <td width="48">0.3</td>

   <td width="46">0.6</td>

   <td width="46">1.7</td>

   <td width="40">2.0</td>

   <td width="53">2.4</td>

   <td width="46">2.9</td>

   <td width="46">3.9</td>

   <td width="46">3.6</td>

   <td width="46">4.4</td>

   <td width="40">5.0</td>

  </tr>

  <tr>

   <td width="24">y</td>

   <td width="48">5.27</td>

   <td width="46">6.76</td>

   <td width="46">13.69</td>

   <td width="40">16.0</td>

   <td width="53">19.391</td>

   <td width="46">24.01</td>

   <td width="46">34.81</td>

   <td width="46">31.36</td>

   <td width="46">40.96</td>

   <td width="40">49.0</td>

  </tr>

 </tbody>

</table>

<h3>Requirements</h3>

It is very time consuming to write your own GP package from scratch. As many GP packages are available, it is actually not necessary to write GP from scratch, but you can use the existing GP packages.. In this assignment, we recommend the following GP packages for the GP questions. They are JGAP (a Java GP library), ECJ (in Java), and DEAP ( in Python). More information/instructions for using these packages could be found in the course assignment page.

Your job is to use any of the genetic programming packages with necessary changes of the terminal set, function set, fitness function, parameters and termination criteria to solve the task described above. Please describe your choice in your report.

You should submit the following files electronically.

<ul>

 <li>Program code written by yourself (both the source code and the executable program running on ECS School machines),</li>

 <li>txt describing how to run your program, and • A report in PDF, text or DOC format. The report should:

  <ol>

   <li>Determine a good terminal set for this task.</li>

   <li>Determine a good function set for this task.</li>

   <li>Construct a good fitness function and describe it using plain language, and mathematical formula(or any other format that can describe the fitness function as accurately as mathematical formula, such as pseudo code).</li>

   <li>Describe the relevant parameter values and the stopping criteria you used.</li>

   <li>Report the mean squared error for each of 10 independent runs with different random seeds, andtheir average value.</li>

   <li>List three different best programs and their fitness values.</li>

   <li>(optional, bonus, 5 marks) Analyse one of the best programs and explain why it can solve the problem in the task.</li>

  </ol></li>

</ul>

<h2>Part 4: Genetic Programming for Classification [40 marks]</h2>

In this part, you are required to use GP to classify the Statlog (Landsat Satellite) data set instances into two classes. This data set was obtained from the <em>UCI machine learning repository </em>(http://archive.ics.uci.edu/ml/datasets.php).

<h3>Problem Description</h3>

The original data set was modified for this assignment. The new version of this data set has 195 instances of anomaly classification. This data set has 75 anomaly instances and 120 normal instances, where the task is to classify these instances into the <em>anomaly </em>and <em>normal </em>classes. Each instances has 36 attributes/features that are extracted from the satellite images. The file satellite contains all the 195 instances.

The 36 attributes are integer valued between 25 and 175. The attributes are denoted as V1, V2, …, V36 in the file. The final column of the file shows the class label (“target”) of each instance. The file satellite gives detailed description of the data.

<h3>Requirements</h3>

Your job is to use any of the genetic programming packages with necessary changes of the terminal set, function set, fitness function, parameters and termination criteria to solve the simple task described above. You should submit the following files electronically.

<ul>

 <li>Program code written by yourself (both the source code and the executable program running on ECS School machines),</li>

 <li>txt and test.txt with appropriate formats,</li>

 <li>txt describing how to run your program, and • A report in PDF, text or DOC format. The report should:

  <ol>

   <li>Determine a good terminal set for this task.</li>

   <li>Determine a good function set for this task.</li>

   <li>Construct a good fitness function and describe it using plain language, and mathematical formula(or any other format that can describe the fitness function as accurately as mathematical formula, such as pseudo code).</li>

   <li>Describe the relevant parameter values and the stopping criteria you used.</li>

   <li>Describe your main considerations in splitting the original data set into a training set txt and a test set test.txt.</li>

   <li>Report the classification accuracy (average accuracy over 10 independent experiment runs withdifferent random seeds) on both the training set and the test set.</li>

   <li>List three best programs evolved by GP and the fitness value of them.</li>

   <li>(optional, bonus, 5 marks) Analyse one of best programs to identify patterns you can find in the evolved/learned program and why it can solve the problem well (or badly).</li>

  </ol></li>

</ul>

<h2>Part 5: Genetic Programming for Classification/Regression [30 marks]</h2>

(This part is only for COMP420 students. COMP307 students do not need to do this part. )

In this part, you are required to use GP to perform classification or regression on the data set (same as Part 1). The data set has eight instances with three features and a target ourput value/a class label (target value:

0 or 1). This problem can be solved as a regression task or a classification task.

<table width="423">

 <tbody>

  <tr>

   <td width="105">Instance No.</td>

   <td width="78">Feature 1</td>

   <td width="78">Feature 2</td>

   <td width="78">Feature 3</td>

   <td width="83">Class/Target</td>

  </tr>

  <tr>

   <td width="105">1</td>

   <td width="78">0</td>

   <td width="78">0</td>

   <td width="78">1</td>

   <td width="83">0</td>

  </tr>

  <tr>

   <td width="105">2</td>

   <td width="78">0</td>

   <td width="78">1</td>

   <td width="78">0</td>

   <td width="83">1</td>

  </tr>

  <tr>

   <td width="105">3</td>

   <td width="78">1</td>

   <td width="78">0</td>

   <td width="78">1</td>

   <td width="83">1</td>

  </tr>

  <tr>

   <td width="105">4</td>

   <td width="78">1</td>

   <td width="78">1</td>

   <td width="78">0</td>

   <td width="83">0</td>

  </tr>

  <tr>

   <td width="105">5</td>

   <td width="78">1</td>

   <td width="78">1</td>

   <td width="78">1</td>

   <td width="83">0</td>

  </tr>

  <tr>

   <td width="105">6</td>

   <td width="78">1</td>

   <td width="78">0</td>

   <td width="78">0</td>

   <td width="83">1</td>

  </tr>

  <tr>

   <td width="105">7</td>

   <td width="78">0</td>

   <td width="78">1</td>

   <td width="78">1</td>

   <td width="83">1</td>

  </tr>

  <tr>

   <td width="105">8</td>

   <td width="78">0</td>

   <td width="78">0</td>

   <td width="78">0</td>

   <td width="83">0</td>

  </tr>

 </tbody>

</table>

<h3>Requirements</h3>

Your job is to use any of the genetic programming packages with necessary changes of the terminal set, function set, fitness function, parameters and termination criteria to solve the simple task described above. You should submit the following files electronically.

<ul>

 <li>Program code written by yourself (both the source code and the executable program running on ECS School machines),</li>

 <li>txt describing how to run your program, and</li>

 <li>A report in PDF, text or DOC format. The report should:

  <ol>

   <li>List the function set (only arithmetic operators, no logic), the terminal set, and the fitness functionof GP to solve this problem.</li>

   <li>Run the experiment five times and report the averaged results (either mean squared error orclassification accuracy).</li>

   <li>Report three best (different) programs/trees evolved by GP from the five runs.</li>

   <li>Analyse the results and programs. Make your conclusions.</li>

   <li>Compare the performance of GP in this part and that of Perceptron that you obtained in Part 1 and make your own discussions.</li>

  </ol></li>

</ul>

<h1>3          Relevant Data Files and Program Files</h1>

The relevant data files, information files about the data sets, and some utility programs files can be found from the following directory:

/vol/comp307/assignment2/

Under this directory, there are three/four subdirectories part1, part2, part3, part4, and part5 (COMP420 students only) corresponding to the four/five parts of the assignment, respectively.

The data files can also be downloaded from the course website as a ZIP file.

<h1>4      Notes</h1>

As an assignment in a 300 level course, you can make your own assumptions if necessary.

During the time between the assignment handout and submission, the tutor(s) will run a number of helpdesks to provide assistance.


