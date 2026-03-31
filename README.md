# Personal Librarian

## Background
Ensuring that educational materials are appropriately matched to a reader’s ability is a central challenge in education and literacy development. Readability assessment plays a critical role in this process by estimating how difficult a given text is to understand. Accurate readability measures help educators select suitable learning materials and promote equitable access to knowledge. When texts are too complex, learners may struggle with comprehension and disengage, and when they are too simple, opportunities for cognitive growth may be limited. As such, improving the accuracy of readability prediction is an important problem with direct implications for educational outcomes.

Traditional readability formulas, such as the Flesch-Kincaid Grade Level, rely primarily on shallow linguistic features like sentence length, word length, and syllable counts. While these metrics are easy to compute and widely used, they fail to capture deeper aspects of language, such as semantic complexity and contextual meaning. For example, two sentences with similar lengths and word structures may differ significantly in conceptual difficulty depending on their content.

Recent advances in natural language processing (NLP), particularly the development of transformer-based language models such as BERT, have enabled more sophisticated representations of text. These models generate contextual embeddings that capture semantic meaning, syntactic structure, and relationships between words in a way that traditional metrics cannot. As a result, machine learning approaches using these embeddings have shown promise in tasks such as text classification and sentiment analysis.

Prior work has combined feature engineering and regression modelling to determine readability prediction. A comparative analysis using different vectorizers (count vectorizer, TF-IDF vectorizer, Word2Vec) and regression models (deep neural networks, linear regression, k-nearest neighbors, decision tree, gradient boosting) shows that TF-IDF Word2Vec vectorizer resulted in the most significant reduction in mean absolute error and mean squared error, respectively, and gradient boosted decision trees and deep neural networks performed the best in terms of the mean absolute and mean squared error of predicting the difficulty of texts (Maddali 2023).

In this project, we propose to expand on the existing literature by fine-tuning and evaluating a BERT-based model for predicting text readability. Our approach integrates semantic embeddings with regression techniques to estimate reading difficulty and compares the results against traditional baselines such as the Flesch-Kincaid Grade Level. Through this comparison, we aim to demonstrate that deep learning models can provide more accurate and meaningful assessments of readability, ultimately contributing to the development of more accessible educational materials.

## Dataset
The CommonLit Ease of Readability (CLEAR) dataset provides a valuable resource for advancing this line of research. It contains thousands of text excerpts annotated with readability scores. By combining this dataset with transformer-based embeddings, it is possible to build models that better reflect the true cognitive demands of reading.

## Methods


## Results


## References
Maddali 2023, https://github.com/suhasmaddali/Predicting-Readability-of-Texts-Using-Machine-Learning
