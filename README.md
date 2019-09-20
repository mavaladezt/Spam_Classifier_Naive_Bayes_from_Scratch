### SMS and Email Spam Classifier using Naive Bayes (only numpy)

#### Naive Bayes
Naive Bayes is a very popular and powerful classifier. One of the reasons it is popular is because it is very efficient. The data processing of the classifier is linear to the number of features since it doesn't involve iterations.<br>

Naive Bayes operates under the assumption that all features are independent and that the data's distribution is known. The latter is not always true but there are ways to estimate the distribution (with the Maximum Likelihood Estimation or MLE).<br><br>
______ ______ ______ ______ ______ ______ ______ ______ ______ ______ ______<br>

__All the coding related to feature generation is the same I already made in my previous 'SMS and Email Classifier notebook' where I used Logistic Regression and Gradient Descent. The 'new' material regarding Naive Bayes starts in the section: Naive Bayes Implementation__<br>
______ ______ ______ ______ ______ ______ ______ ______ ______ ______ ______<br>

The data was obtained from:<br>
__Dua, D. and Graff, C. (2019). UCI Machine Learning Repository (https://archive.ics.uci.edu/ml/datasets/SMS+Spam+Collection). Irvine, CA: University of California, School of Information and Computer Science.__<br>

Abstract: The SMS Spam Collection is a public set of SMS labeled messages that have been collected for mobile phone spam research.<br>

Examples:<br>
__ham__ What you doing?how are you?<br>
__ham__ Ok lar... Joking wif u oni...<br>
__ham__ dun say so early hor... U c already then say...<br>
__ham__ MY NO. IN LUTON 0125698789 RING ME IF UR AROUND! H*<br>
__ham__ Siva is in hostel aha:-.<br>
__ham__ Cos i was out shopping wif darren jus now n i called him 2 ask wat present he wan lor. Then he started guessing who i was wif n he finally guessed darren lor.<br>
__spam__ FreeMsg: Txt: CALL to No: 86888 & claim your reward of 3 hours talk time to use from your phone now! ubscribe6GBP/ mnth inc 3hrs 16 stop?txtStop<br>
__spam__ Sunshine Quiz! Win a super Sony DVD recorder if you canname the capital of Australia? Text MQUIZ to 82277. B<br>
__spam__ URGENT! Your Mobile No 07808726822 was awarded a L2,000 Bonus Caller Prize on 02/09/03! This is our 2nd attempt to contact YOU! Call 0871-872-9758 BOX95QU<br>
