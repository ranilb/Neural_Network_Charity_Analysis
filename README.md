# Neural Network Charity Analysis

In this work, we will implement neural networks algorithms to determine where to support with funding using the TensorFlow platform in Python. This is due to the misuse of fundings from some organizations over the past years.

### Data 
For the analysis, [data](https://github.com/ranilb/Neural_Network_Charity_Analysis/blob/main/charity_data.csv) that ontains more than 34,000 organizations that have received funding from a funding agency over the years. The data set consists of following columns:

* EIN and NAME—Identification columns
* APPLICATION_TYPE—Alphabet Soup application type
* AFFILIATION—Affiliated sector of industry
* CLASSIFICATION—Government organization classification
* USE_CASE—Use case for funding
* ORGANIZATION—Organization type
* STATUS—Active status
* INCOME_AMT—Income classification
* SPECIAL_CONSIDERATIONS—Special consideration for application
* ASK_AMT—Funding amount requested
* IS_SUCCESSFUL—Was the money used effectively

## Results
first, a nueral network algorithm was implemented to determine where to support with fundings using the data listed in the above section.


### Data Preprocessing

* Both identification columns: "EIN" and "Name" were removed so that only relavent information for the goal is extracted. 
* The variable "IS_SUCCESSFUL" that explains was the money used effectively was selected as the target variable. 
* Hence all the other remaining variables were consided as features. 

### Compiling, Training, and Evaluating the Model
* Two hiddenn layers were included in the algorithm with the "relu" activation function. 
* 80 nuerons were included in first hidden layer and the 30 nuerons were included in the second hidden layer. This id due to the numner of imputs is 43. It is reccomended to use 2-3 times nuerons of number of imputs.
* The activation function of the output layer was selected as "sigmoid". Both hidden and output layers have "relu" and "sigmoid" activation fuctions as it can not expect a linear relationship here. 
* With all the above specifications, the model was ran for 50 epochs and the accuracy was 72,6% as shown in the following figure.

    <img width="639" alt="Screen Shot 2023-02-02 at 2 47 21 PM" src="https://user-images.githubusercontent.com/112113327/216434931-f263f7b2-2fcb-453b-b814-c164dc96494a.png">


