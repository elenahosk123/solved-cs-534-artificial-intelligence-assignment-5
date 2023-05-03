Download Link: https://assignmentchef.com/product/solved-cs-534-artificial-intelligence-assignment-5
<br>



In this assignment you are required to build a Naïve Bayes email spam filter.




<h1>Data Description</h1>

The data can be downloaded from <a href="https://canvas.wpi.edu/files/1605424/download?download_frd=1">here</a><a href="https://canvas.wpi.edu/files/1605424/download?download_frd=1">.</a>

This dataset was created from 64 emails collected from the DBWorld mailing list. Please note, the actual emails are not given to you, and the emails have already been processed using NLP.

There are two datasets, <strong>dbworld_bodies_stemmed</strong> and <strong>dbworld_subjects_stemmed</strong> corresponding to the email body and email subject respectively

The data is currently represented as a <em>binary</em> <em>stemmed</em> bag-of-words and <u>requires no</u> <u>additional NLP</u>.

<ul>

 <li>Each dataset is in a table form with 64 rows and <em>n</em></li>

 <li>The <em>1<sup>st</sup></em> column is “id” and has values from 1 to 64, corresponding to each of the 64 emails (this column can be removed).</li>

 <li>The <em>2</em> to <em>n-1</em> columns are unique words found in all the emails, they have binary values i.e. 0 means that the word did not appear in the email and 1 means that the word appeared.</li>

 <li>The <em>n<sup>th</sup></em> column is CLASS, 0 means discard email and 1 means keep email.</li>

</ul>







<h1>Naïve Bayes Classifier</h1>

<ol>

 <li>You should implement <u>from scratch</u> a Naïve Bayes classifier (using the spam filter example discussed in class).</li>

</ol>

Also implement Laplacian smoothing to handle words not in the dictionary. (<strong>40 points</strong>)







<ol>

 <li>Using the implemented algorithm, train and test the model for each dataset.</li>

</ol>

Use 80% of each class data to train your classifier and the remaining 20% to test it.  Which dataset provides better classification i.e. email body or email subject? (<strong>20 points</strong>)




<em>f -measure</em>= 2<em>Pre</em><em>Rec Pre</em>+ <em>Rec</em>

<em>TP                      TP          </em>

where <em>Pre</em>= ;            <em>Rec</em>=    ; <em>TP</em>+ <em>FP         TP </em>+ <em>FN</em>




and <em>TP</em> is the number of true positives (class 1 members predicted as class 1),  <em>TN</em> is the number of true negatives (class 2 members predicted as class 2),  <em>FP</em> is the number of false positives (class 2 members predicted as class 1),  and <em>FN</em> is the number of false negatives (class 1 members predicted as class 2).




<ol>

 <li>Compare your     classifier          with     the       scikit-learn      implementation</li>

</ol>

<a href="https://scikit-learn.org/stable/modules/generated/sklearn.naive_bayes.MultinomialNB.html">(</a><a href="https://scikit-learn.org/stable/modules/generated/sklearn.naive_bayes.MultinomialNB.html">sklearn.naive_bayes.MultinomialNB</a><a href="https://scikit-learn.org/stable/modules/generated/sklearn.naive_bayes.MultinomialNB.html">)</a>.

Repeat the analysis from (b).  (<strong>20 points</strong>)


