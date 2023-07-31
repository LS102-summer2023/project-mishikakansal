# LS 102 - Computer Science Research Paper

## Name

Mishika Kansal

# Title
Bridging the Knowledge Gap: Practical Applications of NLP in Cybersecurity 
---
### Introduction

The ability of a computer program to understand and interpret human language as they are spoken or written is known as Natural Language Processing(NLP).NLP's main objective is to make it possible for computers to comprehend, interpret, and produce natural language in a manner similar to that of humans.NLP entails a number of steps that, when combined, produce the desired result. It is employed for the analysis, comprehension, and production of natural language text and speech.In order to study the rules and structure of language and develop intelligent systems capable of comprehending, analysing, and extracting meaning from text, linguistics and computer science are combined in NLP.


NLP is used in many ways across a variety of fields and industries.Translation, sentiment analysis, and speech recognition are a few examples. NLP techniques are utilized in speech recognition systems to translate spoken language into written text as well as in search engines to extract pertinent information from vast amounts of text.NLP is regarded as a challenging field in computer science since human language is rarely precise or plainly articulated. Knowing human language requires knowing not only the words but also the thoughts and connections that underlie them. In the following years, there could be a lot of advancement, especially in cybersecurity.


Because there are more users, devices, and software in the modern company, along with a flood of private and sensitive data, cybersecurity is becoming more and more crucial. The issue is made worse by the increase in the number, level of skill, and number of cyberattackers. Cybersecurity is essential for defending against a range of online risks, such as cybercrime, cyberattacks, and cyberterrorism. People and businesses use it to prevent illegal access to data centers and other digital systems.


The importance of cybersecurity in the online world cannot be overstated. As we rely more and more on online activities like banking, chatting, and shopping, the risk of cybercrime increases. Our systems and data are protected by cybersecurity from unauthorized access, use, disclosure, interception, and data deletion.(5),(6),(7)


#### Current State of the Art

With numerous recent developments and ongoing research in the area, the state of the art in cybersecurity for natural language processing( NLP) is rapidly changing. The provided search results highlight a few important points.:

1.Machine learning (ML): Many fields already make use of machine learning( ML) capabilities, which is a crucial technology for both current and future information systems. However, ML deployment in cybersecurity is still in its infancy, showing that practice and research are very different from one another. As it can help with breach protection, identification, and scale and scope analysis, machine learning( ML) is becoming more and more a part of cybersecurity workflows.


2.Natural Language Processing(NLP): It is an AI-based deep learning branch that deals with how people and computers interact using common language. Threat feeds and overlaps in standards, frameworks, and data from an organization's tech stack can be found using NLP for risk and compliance.

3.Framework crosswalking and making security telemetry actionable from a risk and compliance perspective are two examples of processes that NLP is being used to automate.

4. A machine posing as a human can use NLP to analyze bot or spam behavior in email text. In order to identify spammer patterns and the kinds of messages they send, it can also be used to comprehend the email's internal structure.

5.The development of new NLP-based systems for digital forensics and cybersecurity is one of the ongoing research projects in the field.

#### Goals of the Project


1.To identify the most effective NLP techniques for detecting and preventing cyber attacks.

2.To integrate NLP into existing cyber workflows to help improve breaches and protection.

3.Provide valuable insights and pratical applications of NLP for cybersecurity professionals.

4. Discuss ethical onsiderations.

### Related work
The field of NLP has acquire a meaningful amount of consideration in the rule of cybersecurity. While most of the research accompanying everything devote effort to something the hypothetical facet present are few studies that have fixated on the experienced use:

Primary Resources:
1.The paper "Natural Language Processing Model for Automatic Analysis of Cybersecurity-Related Documents" by Tiberiu-Marian Georgescu describes the development of an NLP model for automatic analysis of cybersecurity-related documents.(1) 

2."Cyber Security Vulnerability Detection Using Natural Language Processing" This paper expands a scheme targetting spreadsheet exposure discovery as a NLP question. (2)

3.The SAMHSA Publications and Digital Products primer, "Communicating in a Crisis," offers advice on how to communicate effectively and make decisions. The primer emphasizes the value of concise, accurate, and clear communication during a crisis and offers advice on how to communicate effectively, such as by sending out regular updates and using simple messages. The primer offers insights into the significance of effective communication during a crisis, which may be pertinent to the development of NLP models for detecting and responding to cybersecurity threats.(3)


Secondary Resources:
1.A research paper examining the available literature and open data sources related to cybersecurity and cyber risk is titled "Cyber risk and cybersecurity: a systematic review of data availability." The paper, which offers insights into the accessibility of cybersecurity and cyber risk data, is accessible on the NCBI website. About 150 articles, business and government reports, academic papers, and historical cost data or derived cost estimates for losses make up the paper. As it offers insights into the available literature and data sources related to cybersecurity and cyber risk.(4)


2.The IEEE Xplore paper, "Review of NLP-based Systems in Digital Forensics and Cybersecurity," reviews the literature on these systems in cybersecurity and digital forensics, outlining their functions, uses, difficulties, and potential future directions. It sheds light on how NLP-based systems are used in cybersecurity and digital forensics. The paper identifies challenges and potential research directions in this field as well as the potential of NLP-based systems for detecting and responding to cybersecurity threats.(5)


![Spam-detection-block-diagram](https://github.com/LS102-summer2023/project-mishikakansal/assets/136472000/ccad79c2-a95c-4d4b-91e8-2c966861e295)        (23)


### Prototype
The Naive Bayes algorithm is used in the prototype to implement a spam message classifier. The implementation is described below:

1.Importing Libraries: The code starts by importing the required libraries, such as CountVectorizer for text feature extraction, MultinomialNB for the Naive Bayes classifier, and various sklearn metrics. metrics for assessing the effectiveness of the classifier.

2.Loading the dataset:Using the requests library, the code loads the dataset from a specified URL. The CSV file is loaded into a pandas DataFrame if the response status code is 200, indicating that the request was successful. Otherwise, a printed error message appears.

3.Checking Column Names: To confirm the dataset's structure, the code prints the column names in the DataFrame.

4.Data preparation: The text and label columns are divided into X- and Y-variables, respectively.
Using the train _ test _ split function from sklearn, the dataset is divided into training and testing sets. selection of models. A random state of 42 is used for reproducibility, and the testing set size is set at 20% of the total data.

5.Feature Extraction: To transform text data into numerical features, a CountVectorizer object is created. The training data is fitted to the vectorizer and transformed into a matrix of token counts using the fit _ transform method.

6.Training the Classifier: A MultinomialNB classifier is instantiated, and the fit method is used to train it using the training data that has been transformed.

7.Transforming the Testing Data:The feature matrix is created by transforming the testing data using the same vectorizer.

8.Making Predictions:Using the transformed testing data, predictions are made using the predict method.

9.Performance Evaluation: Using the actual labels( y _ test) and the predicted labels, the metrics for accuracy, precision, recall, and F1 score are calculated.

10.Printing Evaluation Metrics: To evaluate the spam classifier's effectiveness, the evaluation metrics( accuracy, precision, recall, and F1 score) are printed.

Data loading, preprocessing, feature extraction, model training, prediction, and evaluation are all part of the prototype's standard machine learning pipeline. The CountVectorizer is used to transform text data into numerical features, and the classification algorithm is the Naive Bayes algorithm. Various metrics are used to assess the classifier's performance.

 <img width="848" alt="Screenshot 2023-08-01 at 2 33 04 AM" src="https://github.com/LS102-summer2023/project-mishikakansal/assets/136472000/1c59b27e-3c4c-4139-be64-dbf60e594f93">   (21)

### Experiments
The spam message classifier's experimental design is as follows:

1.Dataset: From the provided URL, a dataset is obtained that will be used to train and test the spam message classifier. The labeled messages in the dataset are represented by the "v1" column, which stands in for labels( spam or non-spamm), and the'v2 'column for text messages.

2.Data loading and processing: The requests library is used to load the dataset into a pandas DataFrame. To make sure the dataset is loaded correctly, the column names are checked.

3.Data splitting: Using the sklearn's train _ test _ split function, the dataset is divided into training and testing sets. module for model selection. A random state of 42 is used for reproducibility, and the testing set size is set at 20% of the total data.

4.The CountVectorizer from the sklearn is a feature extraction. extraction of features. The text data is transformed into numerical features using the text module. The training and testing data are both transformed using the vectorizer, which is compatible with the training data.

5.Model training: The sklearn's MultinomialNB classifier. The transformed training data is used to train the naive _ bayes module. Due to its efficiency in text classification tasks, this classifier was chosen.

6.Performance evaluation: Using the trained classifier, the testing data are predicted. The sklearn's corresponding functions are used to calculate the accuracy, precision, recall, and F1 score. module for metrics. These metrics give the classifier's ability to accurately classify spam and non-spam messages as well as its overall performance.

The evaluation of the spam message classifier using the provided code yielded the following results:

Accuracy: 0.9838565022421525

recision: 0.9852941176470589

Recall: 0.8933333333333333

F1 score: 0.9370629370629371

These metrics show that the classifier effectively categorizes both spam and non-spam messages. The classifier's high accuracy, precision, recall, and F1 score values imply that it can tell spam messages apart from non-spam messages.
It's crucial to remember that the type of dataset used and the characteristics of the messages can have an impact on how well the classifier performs. To evaluate the classifier's effectiveness on various datasets and look into potential enhancements or optimizations, additional experimentation and evaluation are possible.

![Screenshot 2023-07-27 at 1 04 46 PM 2](https://github.com/LS102-summer2023/project-mishikakansal/assets/136472000/0f2a9615-9003-4de4-b777-15ae3530bcd6)     (22)


#### Evaluation

The search results offer information on the most recent developments in natural language processing( NLP) cybersecurity. The following are highlighted by the results:

1.As it can assist with breach protection, identification, and scale and scope analysis, machine learning( ML) is integrating into cybersecurity workflows more and more.

2.NLP, an AI-based deep learning branch that focuses on how people and computers interact using common language, offers a wealth of capabilities to enhance human ability. NLP is used to find threats and overlaps in data, standards, and frameworks from an organization's tech stack.

3.NLP is being used to automate processes like framework crosswalking and making security telemetry actionable from a risk and compliance standpoint.

4.NLP can be used to understand the internal structure of an email, spot spammer patterns, and analyze bot or spam behavior in text.

5.The creation of new NLP-based systems for cybersecurity and digital forensics is one of the ongoing research projects in the field.

High accuracy, precision, recall, and F1 score values were obtained in the prototype Naive Bayes algorithm spam message classifier implementation, demonstrating its ability to effectively classify both spam and non-spam messages. The performance of the classifier, however, can be influenced by the kind of dataset used and the messages' characteristics. It is possible to conduct additional experiments and evaluate the classifier's performance on various datasets in order to identify any potential improvements.

The project's objectives include identifying the most efficient NLP methods for spotting and preventing cyberattacks, incorporating it into current cyber workflows to help reduce breaches and protect users, offering cybersecurity professionals useful insights and real-world applications, and breaking it down into manageable steps.
Overall, the search findings and prototype implementation show NLP's potential in cybersecurity and emphasize the need for additional field research and development.

#### Threats to Validity
The following are potential threats to the validity :

1.Bias: Depending on the search terms and criteria used, certain sources or perspectives may be the subject of biased search results.

2.Incomplete coverage: Because the search terms and criteria might not have collected all pertinent data, the results may not contain all relevant sources.

3.Information that is out of date: Given how quickly the field of NLP in cybersecurity is developing, some of the sources might be.

4.Limited scope:Only a small portion of the potential uses and difficulties of NLP in cybersecurity are covered by the search results, so their scope may be constrained.

#### Summary of Results
For cybersecurity professionals looking to continuously enhance their compliance procedures, NLP, a subset of machine learning( ML), has excellent applications. Cybersecurity workflows can use NLP to help with scale and scope analysis, breach identification, and protection. Systems based on NLP are being created for cybersecurity and digital forensics. The prototype implements a spam message classifier that efficiently classifies both spam and non-spam messages using the Naive Bayes algorithm. According to the evaluation metrics, the classifier can distinguish between spam messages and non-spam messages because of its high accuracy, precision, recall, and F1 score values. Future research will focus on identifying the most efficient NLP methods for spotting and preventing cyberattacks, incorporating it into pre-existing cyber workflow, and giving cybersecurity professionals useful insights and real-world uses.

#### Future Work

Future work could include:

1.Additional Spam Detection Research: The provided code uses the Naive Bayes algorithm to implement a spam message classifier. Machine learning models that can precisely identify and filter spam while minimizing false positives may be the subject of additional research and development in the future. Additionally, more intelligent filters that can adapt to various spam attacks could be developed.

2.Experimentation for Responsible Design: A resource that suggests an innovative, experiment-based approach to fairness and inclusiveness was found in the search results. Experimentation may be used in the future to evaluate responsible design's inherent qualities and find areas for improvement.

3.A resource on Natural Language Processing Fundamentals is included in the search results. Future research and development of NLP models and methods for text classification tasks, such as spam detection, may be involved.

#### Ethical Implications and Recommendations

There are several ethical issues raised by the application of NLP techniques in cybersecurity that need to be taken into account. The possibility of bias in the NLP algorithms is one of the main ethical ramifications. The NLP algorithms should be created to be as impartial as possible to reduce this. The potential for privacy invasion is another ethical implication. The NLP techniques should be created to only gather and analyse data that is pertinent to cybersecurity in order to lessen this risk.

#### Conclusions

In conclusion, Natural Language Processing (NLP) is an area that is rapidly developing and has a wide range of applications, including cybersecurity. With ongoing research and development, the state-of-the-art in cybersecurity for NLP is rapidly evolving. To automate processes like threat feeds and overlaps in standards, frameworks, and data from an organization's tech stack for risk and compliance, machine learning and NLP are being used. NLP is also used to understand machine-level headers and human languages, as well as to analyse bot or spam behaviour in email text.The project's objectives are to determine which NLP techniques are most useful for detecting and thwarting cyberattacks, integrate NLP into current cyber workflows to help improve breaches and protection, and offer insightful information and useful NLP applications for cybersecurity professionals. In order to ensure that the technology is used responsibly, recommendations should be made that take into account the ethical implications of NLP in cybersecurity. In conclusion, NLP has the potential to completely change the cybersecurity industry, and ongoing research and development will continue to propel the industry forward.

#### References

[1]T.-M. Georgescu, “Natural language processing model for automatic analysis of cybersecurity-related documents,” Symmetry (Basel), vol. 12, no. 3, p. 354, 2020.

[2]K. Singh, S. S. Grover, and R. K. Kumar, “Cyber security vulnerability detection using natural language processing,” in 2022 IEEE World AI IoT Congress (AIIoT), 2022, pp. 174–178.

[3]	“> > > > > > > risk communication guidelines for public officials communicating in a crisis communicating in a crisis: Risk communication guidelines for public officials 2 NATIONAL LIBRARY OF MEDICINE CATALOGING IN PUBLICATION,” Samhsa.gov. [Online]. 


[4] F. Cremer et al., “Cyber risk and cybersecurity: a systematic review of data availability,” Geneva Pap. Risk Insur. Issues Pract., vol. 47, no. 3, pp. 698–736, 2022.

[5] Ukwen, D. O., & Karabatak, M. (2021). Review of NLP-based systems in digital forensics and cybersecurity. 2021 9th International Symposium on Digital Forensics and Security (ISDFS), 1–9.

[6]Richardson, B. (2022, October 19). Changing cybersecurity with natural language processing. NVIDIA Technical Blog. 

[7] Peacock, J. (n.d.). How NLP is transforming cyber risk and compliance. Cybersaint.Io. Retrieved July 31, 2023

[8] Ameri, K., Hempel, M., Sharif, H., Lopez, J., Jr, & Perumalla, K. (2021). CyBERT: Cybersecurity claim classification by fine-tuning the BERT language model. Journal of Cybersecurity and Privacy, 1(4), 615–637. 

[9]Abri, F., Gutierrez, L. F., Kulkarni, C. T., Namin, A. S., & Jones, K. S. (2021). Toward explainable users: Using NLP to enable AI to understand users’ perceptions of cyber attacks. In arXiv [cs.HC].

[10] Cybersecurity vulnerability classification utilizing natural language processing methods. (2021).

[11] Cyberthreat. (2023, February 28). NordVPN. 

[12] Digital collections: Using NLP to predict the severity of cyber sec. (n.d.). UC San Diego Library | Digital Collections. Retrieved July 31, 2023.

[13] Georgescu, T.-M. (2020). Natural language processing model for automatic analysis of cybersecurity-related documents. Symmetry, 12(3), 354. 

[14] Haynes, K., Shirazi, H., & Ray, I. (2021). Lightweight URL-based phishing detection using natural language processing transformers for mobile devices. Procedia Computer Science, 191, 127–134.

[15] Kaur, R., Gabrijelčič, D., & Klobučar, T. (2023). Artificial intelligence for cybersecurity: Literature review and future research directions. An International Journal on Information Fusion, 97(101804), 101804. 

[16] Role and applications of NLP in cybersecurity. (2020, January 22). Masernet. 

[17] Rouse, M. (2011, July 5). Cyberthreat. Techopedia. 

[18] What is cybersecurity? (2022, January 26). Michigan Technological University. 

[19] (N.d.). Perplexity.Ai. Retrieved July 31, 2023.

[20] Rewriter AI. (n.d.). Rewriter.Ai. Retrieved July 31, 2023

[21] Rusland, N. F., Wahid, N., Kasim, S., & Hafit, H. (2017). Analysis of naïve Bayes algorithm for email spam filtering across multiple datasets. IOP Conference Series. Materials Science and Engineering, 226, 012091.

[22] Graphic design software - create awesome designs online. (n.d.). Designcap.com. Retrieved July 31, 2023

[23] ResearchGate. (n.d.). ResearchGate. Retrieved July 31, 2023









