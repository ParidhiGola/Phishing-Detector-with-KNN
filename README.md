# KNN-Classifier-to-detect-phishing-website
Build a model to find out if a website is Legitimate/Suspicious/Malicious using  K Nearest Neighbor

The input data is a In the Pre processing of the Data the attributes are coded into following format for application of KNN Classifier 

 	SFH's type is nominal, range is ('1', '-1', '0')
 	popUpWidnow's type is nominal, range is ('-1', '0', '1')
 	SSLfinal_State's type is nominal, range is ('1', '-1', '0')
 	Request_URL's type is nominal, range is ('-1', '0', '1')
 	URL_of_Anchor's type is nominal, range is ('-1', '0', '1')
 	web_traffic's type is nominal, range is ('1', '0', '-1')
 	URL_Length's type is nominal, range is ('1', '-1', '0')
 	age_of_domain's type is nominal, range is ('1', '-1')
 	having_IP_Address's type is nominal, range is ('0', '1')
 	Result's type is nominal, range is ('0', '1', '-1'))
    
    The  data coding is as follows:
    "1"  - Legitimate Website
    "0"  - Suspicious
    "-1" - Malicious Website
    
   
   **Approach for Building the model**
   
   Left attribute (having_IP_Address's type) as there is n't much variation in the data while creating predictors.
   Applied GridsearchCV to find out Best K (number of neighbors) and used weights as 'distance' with cv = 5 for KNN Classifier
   
   By using the above parameters in KNN Classifier, we achieved 88.67% accuracy.   

