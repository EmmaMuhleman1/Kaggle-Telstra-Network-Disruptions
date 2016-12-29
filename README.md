# Kaggle : Telstra Network Disruptions

Competition : [Kaggle](https://www.kaggle.com/c/telstra-recruiting-network)

Blog : [anshgandhi.wordpress.com](https://anshgandhi.wordpress.com/)


The time duration of this competition was quite over when I started working on this challenge.
As a part of the competition there were 5 files through the users were asked to predict the severity of faults based on given time and log data.
The solution I implemented involved running KModes on the merged data set into 3 clusters, the reason I dd this was because there were 3 fault severities. Next, I trained Neural Networks individually on those clusters. The configuration was, 2 hidden layers - Input -> 6 Neurons -> 3 Neurons -> Output.


<u>Results</u>:<br/>
The loss score of .74 using Neural Network after pre-processing using KMode. The best score for this competition is .395 with the benchmark set at 25.79. Trying various model, the current model worked best, as the competition aimed to minimize log loss function. Having access to some grouped Location data wuld have helped. The data could have been grouped by, for example - Geographical Region.