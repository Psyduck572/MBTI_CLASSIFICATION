# MBTI_CLASSIFICATION

This project explores the concept of classification of personality types using the MBTI test, which is usually an introspective self-report questionnaire that shows people's different psychological preferences when perceiving the world and making decisions. It arises from four dimensions that consist of two categories each. Those dimensions are Extraversion (E) versus Introversion (I), Sensing (S) versus Intuition (N), Thinking (T) versus Feeling (F), and Judging (J) versus Perceiving (P).

The main focus of the project is constructing an immediate MBTI personality diagnosis through individuals’ responses to certain topics. To begin with, two precleaned datasets are adopted from Kaggle for model construction. Both datasets originate from dataset MBTI1, but with different cleaning standards. The first dataset extracts several features from the original posts such as average content length, and frequency of certain punctuations, while the other dataset is content only.

After doing literature reviews on papers under similar settings, three commonly used classification methods are selected: Naive Base, Linear SVM, and Random forest. The first dataset with features is selected in this section. Instead of applying direct multi-classification on sixteen personality types, this study carefully carries out four separate binary classifications according to four major dichotomies in the original MBTI test. Regardless of the four classifications, Random Forest seems to outstand others with the highest accuracy rate of 76.8%( E or I), 86.4% (N or S), 65.2% (T or F), and 59.1 % (J or P).

Later, Long short-term memory (LSTM)​ is used to accomplish a content-only classification, which is a typical machine learning model based on a bag of words model that considers the words in isolation but is a type of neural network that has hidden states and allows past outputs to be used as inputs​. To make the comparison, the study also applied three previous methods to the second content-only dataset. However, LSTM fails to show superior performance compared to others in both binary and multi-classification scenarios.

In later explorations with a larger dataset mbti500, the result shows LSTM personality predictive power increase and surpass the other three as data size increases. LSTM obtains an overall 72% accuracy rate in multi-classification while others only obtain around 20% accuracy.

For more detailed information, please follow the link: https://github.com/Octopusflower/STOR565_PROJECT_MBTI_CLASSIFICATION
