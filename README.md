### 100 Days of Machine Learning - Day 8

# Text Preprocessing Pipeline

This repository contains a basic text preprocessing pipeline, which includes tokenization, stemming, and stopword removal. These steps are essential in many natural language processing tasks, and my goal is to provide a simple, easy-to-use tool for these purposes.

### Getting Started

Define the preprocess function, which takes in a string of text and returns the preprocessed text as a list of stemmed tokens with stopwords removed:

    def preprocess(text):
        # Convert the text to lowercase
        text = text.lower()

        # Tokenize the text into individual words
        words = word_tokenize(text)

        # Remove the stopwords
        words = [word for word in words if word not in stopwords.words('english')]

        # Apply stemming to the words
        stemmer = PorterStemmer()
        words = [stemmer.stem(word) for word in words]

        return words

### Usage

To use the text preprocessing pipeline in your Colab notebook, simply call the preprocess function and pass in your text as a string:

    text = "I love machine learning and natural language processing!"
    processed_text = preprocess(text)
    print(processed_text)

This will output the preprocessed text as a list of stemmed tokens with stopwords removed:

    ['love', 'machin', 'learn', 'natur', 'languag', 'process']

### Contributing

Feel free to contribute to this project and improve the pipeline by adding more features or enhancing the existing ones. To contribute, simply fork this repository, make your changes, and submit a pull request. Happy coding!
