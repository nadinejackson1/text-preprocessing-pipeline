# Text Preprocessing Pipeline

This repository contains a basic text preprocessing pipeline, which includes tokenization, stemming, and stopword removal. These steps are essential in many natural language processing tasks, and my goal is to provide a simple, easy-to-use tool for these purposes.

### Getting Started

To use this pipeline, follow these steps:

1. Clone the repository:
              
              
         git clone https://github.com/nadinejackson1/text-preprocessing-pipeline.git

2. Navigate to the project directory:
              
              
         cd text-preprocessing-pipeline

3. Install the required dependencies:
              
              
         pip install -r requirements.txt

### Usage

To use the text preprocessing pipeline, simply import the preprocess function from the pipeline module and pass in your text as an argument:

    from pipeline import preprocess

    text = "I love machine learning and natural language processing!"
    processed_text = preprocess(text)

    print(processed_text)

This will return the preprocessed text as a list of stemmed tokens with stopwords removed, like so:

    ['love', 'machin', 'learn', 'natur', 'languag', 'process']

Feel free to contribute to this project and improve the pipeline by adding more features or enhancing the existing ones. Happy coding!
