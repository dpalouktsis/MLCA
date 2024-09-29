# Machine Learning & Content Analytics

How to Run the Project

Prerequisites:
1. Python 3.7+ 
2. Jupyter Notebook
3. Flask
4. Pandas
5. Scikit-learn
6. NLTK (with stopwords)
7. Joblib
8. WordCloud

Steps:
1. Install the dependencies:
   Run the following command to install the necessary libraries:
   ```
   pip install flask pandas scikit-learn nltk joblib
   ```

2. Download the Data:
   Open the `Gutenberg_Downloads.ipynb` notebook and execute it to download and preprocess the book data.

3. Create the CSV File:
   Run the `Creation_of_the_csv_file.ipynb` to generate the necessary CSV file (`BOOKS_DATA_updated.csv`) that will be used in the Flask application.

4. Train the Topic Model:
   Open the `MLCA_Topic_Modelling_final.ipynb` and execute the cells to train the NMF topic model and save the results (`nmf_model.pkl`, `tfidf_vectorizer.pkl`, `nmf_topics.pkl`).

5. Run the Flask App:
   In the terminal, navigate to the directory containing `app.py` and run the following command:
   ```
   python app.py
   ```
   The app will be accessible at `http://127.0.0.1:5000/`.

Usage:
- Visit the web interface and input a query about books (e.g., "recommend books about science fiction").
- The system will return a list of book recommendations based on topic similarity.


Authors: Antonios Dimoglou, Sotirios Margonis, Dimitrios Palouktsis, Anastasios Parlanis
