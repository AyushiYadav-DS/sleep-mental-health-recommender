# sleep-mental-health-recommender

<b> Objective </b>
The objective is to analyze the impact of sleep disorders on mental health and build a predictive model to classify sleep disorders based on demographic, lifestyle, and health-related factors.It uses machine learning to predict sleep issues like insomnia or sleep apnea and this project also includes a Gradio-based UI to allow users to check their sleep disorder status and receive personalized recommendations(dietary).

<b>  Data collection & preprocessing </b> 
 Dataset: The dataset contains information on sleep patterns, mental health indicators, demographics, and lifestyle factors.

Preprocessing steps:
1) Handling missing values
2) Encoding categorical variables

<b> Exploratory data analysis (EDA) </b>
 EDA insights:
1)  Understanding gender distribution in sleep disorders
2)  Average sleep duration by occupation (jobs associated with better/worse sleep)
3)  Impact of physical activity on sleep
4)  Variation of insomnia & sleep apnea across demographics
>> Sleep disorders are more prevalent in individuals with high stress and low physical activity.

<b> Model training & evaluation </b>
Pipeline approach:
1)  Built a pipeline with XGBoost as the default model
2)  Compared results with Logistic regression, Decision tree, and KNN

   

<b> Model deployment with Gradio & Comet </b>
1) User Interface with Gradio:
> Users input sleep patterns, lifestyle habits, and mental health status <br>
> Model predicts sleep disorder category <br>
> UI provides sleep disorder & dietary recommendations <br>

>> The XGBoost model is the best choice due to its balance of precision and recall.
The Gradio UI successfully allows users to input their details and get personalized recommendations.


<b> Conclusion </b>
1) The XGBoost model achieved the highest accuracy of 89%, followed closely by the Decision tree (89%) and Logistic regression (88%), while KNN lagged at 84%.
> Key insights from Model comparison
1) XGBoost & Decision tree performed best, indicating tree-based models capture complex patterns in sleep disorders well.
2) Logistic regression performed well but had slightly lower recall for certain classes.
3)  KNN underperformed, suggesting that distance-based models might not be well-suited for this dataset.









