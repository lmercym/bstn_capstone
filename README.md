# What makes a book a bestseller? Predicting a book's popularity using supervised machine learning and NLP
## Overview

In 2021, the books publishing industry represented $109.3bn globally, with more that 2.2 million books published every year. However, growth has been stagnating and even declining between 2016-2020, although it rebounded in 2021 due to the pandemic effect. According to [this report](https://www.ibisworld.com/global/market-size/global-book-publishing/), the global books publishing industry is declining faster than the economy overall. 

**Considering the considerable market size and the competitive marketplace, can we use machine learning to predict a book popularity based on its attributes, so that publishers can adopt a successfull book release strategy and authors can boost their book's success?**

To attempt to answer this question, the Best Books Ever dataset was collected from this [GitHub repository](https://github.com/scostap/goodreads_bbe_dataset) found through Kaggle. The dataset was put together by students in a Master’s Degree in Data Science as part of a project, with data scrapped from GoodReads' Best Book Ever list. It was prepared in November 2020.

Our work for this project will focus on 4 areas, each in a separate Jupyter notebook:

1. Data cleaning and EDA
2. Machine Learning models on a book's features, excluding title and description
3. Machine Learning models on a book's features, including vectorized title and description using Bag of Words and TF-IDF
4. Machine Learning models on a book's features, including vectorized title and description using Word2Vec and GloVe

## Contents

/books_1.Best_Books_Ever.csv : Original dataset collected from this [GitHub repository](https://github.com/scostap/goodreads_bbe_dataset)

/books_df_clean.csv : Dataset after EDA and cleanup, used for running the machine learning models in notebooks 2,3 and 4

/lexvec.enwiki+newscrawl.300d.W.pos.vectors : 

/glove.6B.300d.txt: 

## Dataset information

