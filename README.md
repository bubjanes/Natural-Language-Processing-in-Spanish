# Natural Language Processing in Spanish
These notebooks demonstrate the capabilities and challenges to natural language processing (NLP) with Spanish language. The purpose of this project is to use machine learning to achieve word clustering using natural language data from a real insurance company's customer service department. 

At the beginning of our NLP pipeline we start with raw text. In our case, What'sApp chat messages made by customers writing into an Argentine insurance company for various reasons, such as requesting a tow truck, renewing a policy, or canceling a policy.

The first layer of abstraction:
From raw text we transform the data, each word and sentence, into 'token' objects, which contain useful pieces of data, such as part of speech, entity recognition, ngrams, srank, inverse document frequency, textrank, etc. We will use some of these in our next transformation to a vector object. 

The second layer of abstraction:
With our tokens we can apply a vectorizer() in a process called "embedding." In this step, our numerical representations of words are passed through complex statistical and probablistic formulas to create a vector object. Using the fit_transform() function, we create our most complex object yet, the matrix, which is exists in n-dimensions (this could be more than one hundred dimensions).

Out the pipe:
With the matrix object, we can now extract intelligence about our data set in various forms. The process applied in this project is called "clustering," which groups the words into categories or statistical clusters by the similarities between the attributes of the words. This information could be useful for the insurance company to analyze what people are asking about when they write the company for customer service.
