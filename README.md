# Predicting-User-Behavior-for-Marketing-Campaign

Machine Learning Individual Project by Patrick Guillano La Rosa - November 23, 2021. The code, analysis, and the full report are included in the [Technical Report](https://github.com/pgplarosa/Predicting-User-Behavior-for-Marketing-Campaign/blob/main/md/FinalReport_LaRosaPatrick.md). If you have any questions regarding this study, please send me a message via  [LinkedIn](https://www.linkedin.com/in/patricklarosa/).


<img src="./img/banner.png" width=100% />

## Executive Summary 

<p align="justify">Shopee is the leading e-commerce in southeast Asia and continuously growing amidst the pandemic. They started their operation in Singapore in 2015. They could expand to 10 more countries in just six years, namely the Philippines, Malaysia, Thailand, Taiwan, Indonesia, Vietnam, Brazil, Mexico, Chile, and Colombia. One of the secrets to its success is its sophisticated business model that uses Artificial Intelligence to gather insights from the users.</p>

<p align="justify">In this study, I explored one of the applications of AI in marketing: Predicting when a user would open an email sent by Shopee. I started by performing exploratory data analysis on the distribution, correlation, and correction of our data and finding useful patterns that can be used for our analysis. I saw that most of the users do not open/login/checkout within two months, but those who open an email recently are most likely to open it again. I then see that age slightly plays a factor in the opening of emails by Shopee. As it turns out, older people tend to read an email compared to the younger generation. On a side note, by performing exploratory data analysis, I also saw that our dataset is not that clean where I got an age that is negative and too high of a number that is older than that of the oldest person in the world. It seems that at the time they created the dataset, there was a problem in the app of Shoppee, where a user can enter any birthdate.</p>

<p align="justify">I proceeded by performing data processing to prepare our data for our machine learning model. I used some techniques for imputing null values and feature engineering to help our model better understand the data. I then trained eight different models using a stratified train test split on ten trials with a 25% test size and found that the best-performing model in terms of prediction is Catboost. To improve the accuracy, I then performed resampling methods such as SMOTE, ADASYN, and SMOTENC, which further boosted the accuracy by 1%</p>

<p align="justify">I then used model interpretability and saw how the features affect the target variable in the summary plot. I noticed that a high open count of users tends to open an email again. I also noticed that subject line length and age play an important role in the model's decision. I then inspected features using the Accumulated Local Effects (ALE) Plot that I think are relevant to the study and further verified the results. I then used the RuleFit model to create rule-based decisions and saw that some countries do not prefer email as a platform.</p>

<p align="justify">Some of my recommendation to Shopee drawn from the models is that they can: Understand existing users who recently opened their email because they are likely to open it again, There is an optimal subject line length of 40 to 50 characters, and Consider targeting older people as they are more likely to read mails, and be aware on the country of the user because some countries may not prefer email as a medium at all.</p>
