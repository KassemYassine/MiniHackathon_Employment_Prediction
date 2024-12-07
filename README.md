# MiniHackathon_Employment_Prediction


## Project Overview
This project was developed as part of a mini-hackathon quiz at my university, where the dataset was provided to us. Participants were tasked with framing a problem and applying a machine learning algorithm to address it. The goal of this project is to predict employment status using a logistic regression model that incorporates polynomial feature transformations to better capture the complexities in the dataset.

### Framing the Problem
For our mini-hackathon project, we tackled the problem of predicting employment status by framing it as a binary classification task using the diverse attributes provided in the dataset. The dataset offered a rich blend of variables, including demographic details like age and education, behavioral aspects such as smoking habits, and personality traits like being extraverted or anxious. Each of these features potentially impacts employability. For example, 'Sector' indicates the industry of employment, while 'How old are you?' and 'What is the highest level of education you have attained?' are critical in determining professional opportunities available to an individual. Personality traits such as being 'dependable, self-disciplined' or 'anxious, easily upset' could also influence one's job performance and stability, thereby affecting employment status. Additionally, smoking habits could provide insights into stress management and health, factors that could indirectly affect one's employment status, especially in roles requiring high physical and mental endurance. Using these insights, we preprocessed the data by generating polynomial features to explore non-linear relationships that a simple logistic regression might miss. This approach allowed us to uncover complex interactions, such as how the combination of age, educational level, and smoking habits could predict employment status more accurately.

## Dataset
The dataset includes a variety of attributes that influence employment status, such as 'Sector', 'Age', 'Educational Level', 'Smoking Habits', and 'Personality Traits' (e.g., extraverted, anxious). These attributes provide a comprehensive view of potential employability influences, allowing for detailed analysis and modeling.

## Methodology
1. **Data Preparation**: We split the data into training, validation, and testing sets to manage overfitting and to evaluate the model's performance on unseen data effectively. Additionally, we preprocessed the data by handling missing values and removing unnecessary columns that did not contribute to the predictive model, ensuring clean and relevant input data for training.
   
2. **Feature Engineering**: Polynomial features of degree 2 are generated to allow the logistic regression model to capture not only linear relationships but also interactions between different features.

3. **Model Training and Validation**: The logistic regression model is trained on the training set, and the validation set is used to tune model parameters, ensuring the model is not biased towards the test data.

4. **Model Evaluation**: The final model is evaluated on the test set with metrics such as accuracy to assess its effectiveness in predicting employment status.

## Results
The model achieved an accuracy of approximately 96.1% on the test set, demonstrating high proficiency in predicting employment status based on the provided features.

## Technologies Used
- Python
- Scikit-Learn for machine learning
- Jupyter Notebook for interactive development

## How to Run
1. Clone the repository.
2. Ensure that Python and the necessary packages (pandas, scikit-learn) are installed.
3. Run the Jupyter Notebook `Employmentprediction.ipynb` to view the workflow and results.

## Conclusion
This project highlights the capability of logistic regression, enhanced with polynomial feature engineering, to effectively predict employment status as part of a university mini-hackathon. Future work could explore more complex models, additional feature engineering, and advanced machine learning techniques to further improve the accuracy.

