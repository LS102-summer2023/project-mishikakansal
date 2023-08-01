# LS 102 - Computer Science Research Paper

## Name

Mishika Kansal

# Title
Bridging the Knowledge Gap: Practical Applications of NLP in Cybersecurity 
---
### Introduction

A fast growing discipline called "natural language processing" (NLP) combines computer science, linguistics, and machine learning to give computers the ability to comprehend and interpret spoken or written language. NLP's fundamental goal is to enable computers to understand, interpret, and produce natural language in a manner that is comparable to that of humans. NLP attempts to create intelligent systems capable of understanding, analyzing, and deriving meaning from text by studying the grammar and structure of language.

Many different areas and industries use NLP in diverse ways. It is utilized in many different applications, including speech recognition, sentiment analysis, and translation. NLP approaches are used in the field of cybersecurity to improve breach detection, analysis, and protection. Cybersecurity is more important than ever due to the rise in people, devices, and software in modern businesses as well as the volume of sensitive and private data. By limiting illegal access to data centers and electronic systems, NLP plays a vital part in protecting against cybercrime, cyberattacks, and cyberterrorism.

It is impossible to overestimate the significance of cybersecurity in the online world. The risk of cybercrime rises as our reliance on internet activities like banking, talking, and shopping grows. Our systems and data are safeguarded by cybersecurity against unauthorized access, use, disclosure, interception, and destruction. NLP has a lot of potential to help the field of cybersecurity and solve the changing cybersecurity threats as a result of its breakthroughs.

NLP is growing beyond the common use cases of machine-human communication to machines that can comprehend both human and non-human language as more businesses use it. Organizations now have an exciting chance to stay ahead of changing cybersecurity threats. In cybersecurity workflows, NLP can be used to help with breach detection, identification, and size and scope analysis. For instance, phishing attempts can be detected or bot or spam behavior can be studied using NLP techniques to analyze and comprehend the content of emails. NLP may also be used to automatically monitor the dark web and examine interactions between threat players in cyber threat intelligence.

As the number and market for NLP applications continue to increase, the application of NLP in cybersecurity is gaining ground.There are numerous cybersecurity applications that can make use of the abundance of research and algorithms that are published every day. NLP has the ability to transform the methods used by cybersecurity experts to identify and stop online threats, strengthen breach defenses, and improve risk and compliance procedures.(5),(6),(7)


#### Current State of the Art

With numerous recent developments and ongoing research in the area, the state of the art in cybersecurity for natural language processing ( NLP) is rapidly changing. The provided search results highlight a few important points:

1. Machine learning (ML): Many fields already make use of machine learning (ML) capabilities, which is a crucial technology for both current and future information systems. However, ML deployment in cybersecurity is still in its infancy, showing that practice and research are very different from one another. As it can help with breach protection, identification, and scale and scope analysis, machine learning( ML) is becoming more and more a part of cybersecurity workflows.


2. Natural Language Processing (NLP): It is an AI-based deep learning branch that deals with how people and computers interact using common language. Threat feeds and overlaps in standards, frameworks, and data from an organization's tech stack can be found using NLP for risk and compliance.

3. Framework crosswalking and making security telemetry actionable from a risk and compliance perspective are two examples of processes that NLP is being used to automate.

4. A machine posing as a human can use NLP to analyze bot or spam behavior in email text. In order to identify spammer patterns and the kinds of messages they send, it can also be used to comprehend the email's internal structure.

5. The development of new NLP-based systems for digital forensics and cybersecurity is one of the ongoing research projects in the field.

#### Goals of the Project


1. To identify the most effective NLP techniques for detecting and preventing cyberattacks.

2. To integrate NLP into existing cyber workflows to help improve breaches and protection.

3. Provide valuable insights and practical applications of NLP for cybersecurity professionals.

4. Discuss ethical considerations.

### Related work
The field of NLP has acquired a meaningful amount of consideration in the realm of cybersecurity. While most of the research accompanying everything devotes effort to something hypothetical , there are a few studies that have focused on the experienced use:

Primary Resources:
1. The paper "Natural Language Processing Model for Automatic Analysis of Cybersecurity-Related Documents" by Tiberiu-Marian Georgescu describes the development of an NLP model for automatic analysis of cybersecurity-related documents. (1) 

2. "Cyber Security Vulnerability Detection Using Natural Language Processing" This paper expands a scheme targeting spreadsheet exposure discovery as an NLP question. (2)

3. The SAMHSA Publications and Digital Products primer, "Communicating in a Crisis," offers advice on how to communicate effectively and make decisions. The primer emphasizes the value of concise, accurate, and clear communication during a crisis and offers advice on how to communicate effectively, such as by sending out regular updates and using simple messages. The primer offers insights into the significance of effective communication during a crisis, which may be pertinent to the development of NLP models for detecting and responding to cybersecurity threats. (3)


Secondary Resources:
1. A research paper examining the available literature and open data sources related to cybersecurity and cyber risk is titled "Cyber risk and cybersecurity: a systematic review of data availability." The paper, which offers insights into the accessibility of cybersecurity and cyber risk data, is accessible on the NCBI website. About 150 articles, business and government reports, academic papers, and historical cost data or derived cost estimates for losses make up the paper. As it offers insights into the available literature and data sources related to cybersecurity and cyber risk. (4)


2. The IEEE Xplore paper, "Review of NLP-based Systems in Digital Forensics and Cybersecurity," reviews the literature on these systems in cybersecurity and digital forensics, outlining their functions, uses, difficulties, and potential future directions. It sheds light on how NLP-based systems are used in cybersecurity and digital forensics. The paper identifies challenges and potential research directions in this field as well as the potential of NLP-based systems for detecting and responding to cybersecurity threats. (5)


![Spam-detection-block-diagram](https://github.com/LS102-summer2023/project-mishikakansal/assets/136472000/ccad79c2-a95c-4d4b-91e8-2c966861e295)        (23)


### Prototype
The Naive Bayes algorithm is used in the prototype to implement a spam message classifier. The implementation is described below:

1. Importing Libraries: The code starts by importing the required libraries, such as CountVectorizer for text feature extraction, MultinomialNB for the Naive Bayes classifier, and various Sklearn metrics. metrics for assessing the effectiveness of the classifier.

2. Loading the dataset: Using the requests library, the code loads the dataset from a specified URL. The CSV file is loaded into a Pandas DataFrame if the response status code is 200, indicating that the request was successful. Otherwise, a printed error message appears.

3. Checking Column Names: To confirm the dataset's structure, the code prints the column names in the DataFrame.

4. Data preparation: The text and label columns are divided into X- and Y-variables, respectively.
Using the train _ test _ split function from sklearn, the dataset is divided into training and testing sets. selection of models. A random state of 42 is used for reproducibility, and the testing set size is set at 20% of the total data.

5. Feature Extraction: To transform text data into numerical features, a CountVectorizer object is created. The training data is fitted to the vectorizer and transformed into a matrix of token counts using the fit _ transform method.

6. Training the Classifier: A MultinomialNB classifier is instantiated, and the fit method is used to train it using the training data that has been transformed.

7. Transforming the Testing Data:The feature matrix is created by transforming the testing data using the same vectorizer.

8. Making Predictions: Using the transformed testing data, predictions are made using the predict method.

9. Performance Evaluation: Using the actual labels ( y _ test) and the predicted labels, the metrics for accuracy, precision, recall, and F1 score are calculated.

10. Printing Evaluation Metrics: To evaluate the spam classifier's effectiveness, the evaluation metrics (accuracy, precision, recall, and F1 score) are printed.

Data loading, preprocessing, feature extraction, model training, prediction, and evaluation are all part of the prototype's standard machine learning pipeline. The CountVectorizer is used to transform text data into numerical features, and the classification algorithm is the Naive Bayes algorithm. Various metrics are used to assess the classifier's performance.

 <img width="848" alt="Screenshot 2023-08-01 at 2 33 04 AM" src="https://github.com/LS102-summer2023/project-mishikakansal/assets/136472000/1c59b27e-3c4c-4139-be64-dbf60e594f93">   (21)

### Experiments
The spam message classifier's experimental design is as follows:

1. Dataset: From the provided URL, a dataset is obtained that will be used to train and test the spam message classifier. The labeled messages in the dataset are represented by the "v1" column, which stands for labels( spam or non-spamm), and the 'v2' column for text messages.

2. Data loading and processing: The requests library is used to load the dataset into a Pandas DataFrame. To make sure the dataset is loaded correctly, the column names are checked.

3. Data splitting: Using the Sklearn's train _ test _ split function, the dataset is divided into training and testing sets. module for model selection. A random state of 42 is used for reproducibility, and the testing set size is set at 20% of the total data.

4. The CountVectorizer from sklearn is a feature extraction. extraction of features. The text data is transformed into numerical features using the text module. The training and testing data are both transformed using the vectorizer, which is compatible with the training data.

5. Model training: The sklearn's MultinomialNB classifier. The transformed training data is used to train the naive _ bayes module. Due to its efficiency in text classification tasks, this classifier was chosen.

6. Performance evaluation: Using the trained classifier, the testing data are predicted. The sklearn's corresponding functions are used to calculate the accuracy, precision, recall, and F1 score, moduleS for metrics. These metrics reflect the classifier's ability to accurately classify spam and non-spam messages as well as its overall performance.

The evaluation of the spam message classifier using the provided code yielded the following results:

Accuracy: 0.9838565022421525

recision: 0.9852941176470589

Recall: 0.8933333333333333

F1 score: 0.9370629370629371

These metrics show that the classifier effectively categorizes both spam and non-spam messages. The classifier's high accuracy, precision, recall, and F1 score values imply that it can tell spam messages apart from non-spam messages.
It's crucial to remember that the type of dataset used and the characteristics of the messages can have an impact on how well the classifier performs. To evaluate the classifier's effectiveness on various datasets and look into potential enhancements or optimizations, additional experimentation and evaluation are possible.

![Screenshot 2023-07-27 at 1 04 46 PM 2](https://github.com/LS102-summer2023/project-mishikakansal/assets/136472000/0f2a9615-9003-4de4-b777-15ae3530bcd6)     (22)


#### Evaluation

The search results offer information on the most recent developments in natural language processing( NLP) and cybersecurity. The following are highlighted by the results:

1. As it can assist with breach protection, identification, and scale and scope analysis, machine learning (ML) is integrating into cybersecurity workflows more and more.

2. NLP, an AI-based deep learning branch that focuses on how people and computers interact using common language, offers a wealth of capabilities to enhance human ability. NLP is used to find threats and overlaps in data, standards, and frameworks in an organization's tech stack.

3. NLP is being used to automate processes like framework crosswalking and make security telemetry actionable from a risk and compliance standpoint.

4. NLP can be used to understand the internal structure of an email, spot spammer patterns, and analyze bot or spam behavior in text.

5. The creation of new NLP-based systems for cybersecurity and digital forensics is one of the ongoing research projects in the field.

High accuracy, precision, recall, and F1 score values were obtained in the prototype Naive Bayes algorithm spam message classifier implementation, demonstrating its ability to effectively classify both spam and non-spam messages. The performance of the classifier, however, can be influenced by the kind of dataset used and the messages' characteristics. It is possible to conduct additional experiments and evaluate the classifier's performance on various datasets in order to identify any potential improvements.

The project's objectives include identifying the most efficient NLP methods for spotting and preventing cyberattacks, incorporating them into current cyber workflows to help reduce breaches and protect users, offering cybersecurity professionals useful insights and real-world applications, and breaking them down into manageable steps.
Overall, the search findings and prototype implementation show NLP's potential in cybersecurity and emphasize the need for additional field research and development.

#### Threats to Validity
The following are potential threats to its validity :

1. Bias: Depending on the search terms and criteria used, certain sources or perspectives may be the subject of biased search results.

2. Incomplete coverage: Because the search terms and criteria might not have collected all pertinent data, the results may not contain all relevant sources.

3. Information that is out of date: Given how quickly the field of NLP in cybersecurity is developing, some of the sources might be out of date.

4. Limited scope: Only a small portion of the potential uses and difficulties of NLP in cybersecurity are covered by the search results, so their scope may be constrained.

#### Summary of Results
For cybersecurity professionals looking to continuously enhance their compliance procedures, NLP, a subset of machine learning (ML), has excellent applications. Cybersecurity workflows can use NLP to help with scale and scope analysis, breach identification, and protection. Systems based on NLP are being created for cybersecurity and digital forensics. The prototype implements a spam message classifier that efficiently classifies both spam and non-spam messages using the Naive Bayes algorithm. According to the evaluation metrics, the classifier can distinguish between spam messages and non-spam messages because of its high accuracy, precision, recall, and F1 score values. Future research will focus on identifying the most efficient NLP methods for spotting and preventing cyberattacks, incorporating them into pre-existing cyber workflows, and giving cybersecurity professionals useful insights and real-world uses.

#### Future Work

Future work could include:

1. Additional Spam Detection Research: The provided code uses the Naive Bayes algorithm to implement a spam message classifier. Machine learning models that can precisely identify and filter spam while minimizing false positives may be the subject of additional research and development in the future. Additionally, more intelligent filters that can adapt to various spam attacks could be developed.

2. Experimentation for Responsible Design: A resource that suggests an innovative, experiment-based approach to fairness and inclusiveness was found in the search results. Experimentation may be used in the future to evaluate responsible design's inherent qualities and find areas for improvement.

3. A resource on natural language processing fundamentals is included in the search results. Future research and development of NLP models and methods for text classification tasks, such as spam detection, may be involved.

#### Ethical Implications and Recommendations

There are several ethical issues raised by the application of NLP techniques in cybersecurity that need to be taken into account. The possibility of bias in the NLP algorithms is one of the main ethical ramifications. The NLP algorithms should be created to be as impartial as possible to reduce this. The potential for privacy invasion is another ethical implication. The NLP techniques should be created to only gather and analyze data that is pertinent to cybersecurity in order to lessen this risk.

#### Conclusions

In conclusion, the role of natural language processing (NLP) in cybersecurity is rapidly evolving, and ongoing research and development will continue to propel the industry forward. NLP has a wide range of applications in cybersecurity, including threat detection and prediction, improving breach protection, risk and compliance, dark web monitoring, digital forensics, and securing code. To automate processes like threat feeds and overlaps in standards, frameworks, and data from an organization's tech stack for risk and compliance, machine learning and NLP are being used. NLP is also used to understand machine-level headers and human languages, as well as to analyze bot or spam behavior in email text. The project's objectives are to determine which NLP techniques are most useful for detecting and thwarting cyberattacks, integrate NLP into current cyber workflows to help improve breaches and protection, and offer insightful information and useful NLP applications for cybersecurity professionals. It is important to consider the ethical implications of NLP in cybersecurity and make recommendations to ensure responsible use of the technology. As more enterprises adopt NLP, the sub-field is developing beyond those popular use cases of machine-human communication to include machines interpreting both human and non-human language. This creates an exciting opportunity for organizations to stay ahead of evolving cybersecurity threats. In the future, NLP has the potential to completely change the cybersecurity industry. As the number and market of NLP applications continue to grow, the role of NLP in cybersecurity will also increase. The plethora of research and algorithms released every day may therefore be used for a suite of cybersecurity applications. In summary, NLP has the potential to significantly impact the cybersecurity industry. Ongoing research and development will continue to drive advancements in this field, offering new ways to detect and prevent cyber threats. As cybersecurity professionals continue to integrate NLP into their workflows, they will be better equipped to protect their organizations from evolving threats. However, it is important to use this technology responsibly and consider the ethical implications of its use.

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









