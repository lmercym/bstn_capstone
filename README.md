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

- /books_1.Best_Books_Ever.csv : Original dataset collected from this [GitHub repository](https://github.com/scostap/goodreads_bbe_dataset)

- /books_df_clean.csv : Dataset after EDA and cleanup, used for running the machine learning models in notebooks 2,3 and 4

- /lexvec.enwiki+newscrawl.300d.W.pos.vectors : Pre-trained vectors used for Word2Vec embedding

- /glove.6B.300d.txt: Pre-trained vectors used for Glove embedding

## Clean Dataset information

- title: Book title
- description: Book description
- pages: Number of pages
- word_count_title: Number of words in title
- is_series: Indicates whether or not the book is part of a series	
- book_count_by_author: Number of books the author has listed on the Goodreads' Best Book Ever list
- word_count_description: Number of words in description
- genre_Adult: Indicates the book's genre ( a book can be multiple genres)
- genre_Adventure: Indicates whether the book belongs to this genre ( a book can be multiple genres)
- genre_Biography: Indicates whether the book belongs to this genre ( a book can be multiple genres)
- genre_Childrens: Indicates whether the book belongs to this genre ( a book can be multiple genres)
- genre_Classics: Indicates whether the book belongs to this genre ( a book can be multiple genres)
- genre_Contemporary: Indicates whether the book belongs to this genre ( a book can be multiple genres)
- genre_Fantasy: Indicates whether the book belongs to this genre ( a book can be multiple genres)
- genre_Fiction: Indicates whether the book belongs to this genre ( a book can be multiple genres)
- genre_Historical: Indicates whether the book belongs to this genre ( a book can be multiple genres)
- genre_Historical Fiction: Indicates whether the book belongs to this genre ( a book can be multiple genres)
- genre_History: Indicates whether the book belongs to this genre ( a book can be multiple genres)
- genre_Horror: Indicates whether the book belongs to this genre ( a book can be multiple genres)
- genre_Islam: Indicates whether the book belongs to this genre ( a book can be multiple genres)
- genre_Literature: Indicates whether the book belongs to this genre ( a book can be multiple genres)
- genre_Magic: Indicates whether the book belongs to this genre ( a book can be multiple genres)
- genre_Mystery: Indicates whether the book belongs to this genre ( a book can be multiple genres)
- genre_Nonfiction: Indicates whether the book belongs to this genre ( a book can be multiple genres)
- genre_Novels: Indicates whether the book belongs to this genre ( a book can be multiple genres)
- genre_Paranormal: Indicates whether the book belongs to this genre ( a book can be multiple genres)
- genre_Poetry: Indicates whether the book belongs to this genre ( a book can be multiple genres)
- genre_Romance: Indicates whether the book belongs to this genre ( a book can be multiple genres)
- genre_Science Fiction: Indicates whether the book belongs to this genre ( a book can be multiple genres)
- genre_Thriller: Indicates whether the book belongs to this genre ( a book can be multiple genres)
- genre_Urban: Indicates whether the book belongs to this genre ( a book can be multiple genres)
- genre_Young Adult: Indicates whether the book belongs to this genre ( a book can be multiple genres)
- genre_Other: Indicates whether the book belongs to this genre ( a book can be multiple genres)
- format_Audiobook: Book's format
- format_Hardcover: Book's format
- format_Mass Market Paperback: Book's format
- format_Paperback: Book's format
- format_ebook: Book's format
- has_awards: Indicates whether the book has received awards or not
- publish_year: Year the edition has been published
- is_popular: Indicates whether or not a book is popular (1 if rating >4.0, 0 if not)
