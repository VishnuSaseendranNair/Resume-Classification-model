# Resume-Classification-model
 ML Resume Classification Model
The main steps and functionalities of the code are as follows:

1. Import Libraries: The necessary libraries such as NumPy, Pandas, Matplotlib, Seaborn, NLTK, and scikit-learn are imported.

2. Read and Explore Data: The script reads a CSV file named 'UpdatedResumeDataSet.csv', which contains information about resumes, including the text content and the corresponding category. The data is explored to understand its structure and unique categories.

3. Data Cleaning: The script defines a function ("cleanResume") to clean the resume text by removing URLs, mentions, special characters, and extra whitespace. The cleaned text is stored in a new column called 'cleaned_resume'.

4. Exploratory Data Analysis (EDA): The script performs EDA to visualize the distribution of resume categories using bar plots and pie charts.

5. Word Cloud Generation: A word cloud is generated to visualize the most common words in the cleaned resume text.

6. Label Encoding: The 'Category' column, which contains categorical labels, is encoded using Label Encoding.

7. Text Vectorization: The script uses TF-IDF (Term Frequency-Inverse Document Frequency) vectorization to convert the cleaned resume text into numerical features. The data is split into training and testing sets.

8. Model Training: A K-Nearest Neighbors (KNN) classifier is trained using the One-vs-Rest strategy to handle multiclass classification.

9. Model Evaluation: The script evaluates the classifier's accuracy on both the training and testing sets and prints a classification report, including precision, recall, and F1-score.

10. Confusion Matrix Visualization: The confusion matrix is visualized using Seaborn's heatmap to show the performance of the classifier across different categories.

11. PDF Text Extraction: The script defines a function (`extract_text_from_pdf`) to extract text from a PDF file using the PyMuPDF library.

12. New Resume Classification: The script uses the trained classifier to predict the category of a new resume. A sample PDF file ('resume3.pdf') is provided as an example. The PDF text is extracted, preprocessed, vectorized, and then classified using the trained KNN classifier.

The code provides a comprehensive example of text classification for resumes, including data preprocessing, feature engineering, model training, evaluation, and application to new data (PDF resume).
