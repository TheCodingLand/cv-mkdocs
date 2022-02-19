# Artificial Intelligence

*Below are some examples of my machine learning projects.*



## Auto Helpdesk (company : CTG)

!!! quote "*Automated IT incident classification using deep learning and large language models/transformers. (implemented at 2 different companies)*"


???- Note "Details"

    === "Main Tools"
        - Jupyter

    === "Main ML Libraries"
        - Huggingface transformers
        - Tensorflow (custom ensemble of several deep learning models)
        

## Alfred (Company: CTG):

!!! quote "*Automated incident prevention for IT servers / cloud architectures using deep learning, boosting, and time series forecasting, from monitoring data and sensors, to automatically detect valid threshold for metric combinations*"


???- Note "Details"
    === "Abstract"
        Working with monitoring tools, sometimes, it is very difficult to predict if an alert is valid or not, only based on metrics threshold.<BR/>
        Fast moving environment like cloud and orchestrated containers, make it even more challenging to define thresholds for all individual metrics.<BR/>
        Using a deep learning approach, boosting, and time series forecasting, I was able to implement a model capable of detecting potential issues in advance of alerts, removing hard coded thresold from all our monitoring solutions.<BR/>
        The solution is able to detect anomalies in variable levels, extrapolating from their normal inter-dependence, and normal platform usage cycles (with Prophet to flatten recurrent "seasonal" variations)
        
    === "Main Tools"
        - Jupyter
        - Zabbix
        - Nagios / Icinga

    === "Main ML Libraries"
        - XgBoost
        - pytorch
        - FBprophet
        
## Resume Parser (Company: CTG):


!!! quote "*Automated data extraction for CVs, and web backend to help query the results using django*"

???- Note "Details"

    === "Main Tools"
        - Jupyter
    
    === "Main ML Libraries"
        - django
        - scipy
        - spacy
        - transformers


