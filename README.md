# Text-Mining-on-500-MNT-News
In this project we predicted some surprised ratings for three raters on basis of many variables by using text mining techniques.

Text Mining is the process of deriving high-quality information from text. High-quality
information is typically derived through the devising of patterns and trends through means such
as statistical pattern learning.
In this project our main aim was to compute the average human rater’s surprise rating for the 500
and 1500 cases respectively with the use of text mining to turn the text into data for analysing
these conditions .So we took the 500MNT health corpus data to see if the text mining on these
articles would help us analyze on what basis the three human’s surprise raters rated these articles.
In the process of text mining , extracting the features from the articles and picking the
independent variables from the ground truth file helped us analyze what could be the reason for
which the raters were surprised by reading the health articles.The use of features extraction
greatly helped us understand how the raters rated the articles on the basis on their surprise level
.With these external entities ,we build predictive models and calculated the accuracy to see
which model is the best fit.


PART 1 :

We predicted the average surprise ratings by building and running the following models.
Here we have 500 cases of human ratings for each article with variables like surprise
ratings, like ratings, familiarity ratings, categories, title and article ids. As we have to find
the the average surprise ratings , we need to acquire average of few variables like ‘like’
ratings, ‘familiarity’ ratings.
Hence, we took average of the above specified variables and appended the average values
into a new column. We also used features like surprise words and word count in each article
as we thought semantic analysis can help us more in finding out the surprise element and by
this we can also find out the average surprise variable. The variables we finally considered
for building and running the model are as follows:
Article Id, Average familiarity rating, Avg. like rating, category variables.

After acquiring the variables we will be building models:
Logistic Regression
Random forest 
Naive Bayes

Result : 

Based on the above three models , we observed that the Logistic Regression model
gave us better accuracy in predicting the human’s average surprise rating for the three human
raters (r1,r2,r3). Even though logistic regression gave a better accuracy, as we can see from the
above screenshots, naive bayes model has done a better job at splitting the data and predicting it.
Therefore we can deduce that naive bayes is a better predictive model for the above case.

PART 2 :

We have constructed the following predictive models to address the below question -
Each individual human rater’s surprise rating for an article using whatever your proposed
features (1,500 cases in total)
In this case we had to build prediction models for the entire 1500 cases which consists of
R1, R2 and R3. So that variables we considered for this case are category 1, category 2, category
3, category 4, familiarity (c1 familiarity, c2 familiarity , c3 familiarity , c4 familiarity), like,
article.
Along with these independent variables from the ground truth file for this case we have
derived few semantic features from the corpus, that are surprise words, conditional words, ‘Wh’
words, believe words. We have used these features explicitly because semantic analysis will help
us find out the surprise elements and its effects in the rating.
‘Wh’ words - We took words such as ‘when’, ‘what’, ‘why’, ‘where’, etc
Conditional words - We took words like ‘even if’, ‘as soon as’, as a result of’, etc
Surprise words - We took words like ‘unannounced’, ‘awesome’, ‘awful’, etc
Believe words - We took words like ‘accept’, ‘appreciate’, ‘assume’, etc

After acquiring the independent variables and derived features we will apply them to the below
predictive models.
- Logistic regression
- Random forest
- Neural network

Result : 

Based on the above three models , we observed that the Neural network model gave us
better accuracy in predicting the human’s average surprise rating for the three human raters
(r1,r2,r3).
