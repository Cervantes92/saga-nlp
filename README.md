# The Icelandic Sagas: A Machine Learning Approach

## Abstract

The Iceladic sagas are a collection of narrative documents written between the 12th and 14th century. The Icelandic sagas typically take place in the 9th to 11th century through the settlement of Iceland by norse settlers. Together, these sagas weave a colorful history of feuds and families that expands out of Iceland from Constantinople to Newfoundland, often with blunt, terse prose that stands in stark contrast to modern literature, but does too good a job hiding complexity and subtext.

The goal of this project is to make the Icelandic sagas more approachable to the modern reader by using natural language processing techniques to perform topic extraction on both a chapter and paragraph basis. I also hope to train a tool to provide a contextualized thesaurus to aid both casual readers and accademics in decyphering the meaning of terms and phrases.

## Methodology

We will be using two methods for topic extraction. Term Frequency - Inverse Document Frequency (TF-IDF) and Latent Dirichlet Allocation (LDA). TF-IDF works by considering how often a term appears in a given document, and subtracts it by how frequently documents contain the word. This method is useful for automatically dismissing frequent but less important words (common stop words such as 'the', 'and' et al) and highlighting topics that are prominent within each document.

LDA is a generative statistical model that explains sets of observations to be explained by unobserved groups. For example, for each document within our corpus, our LDA model will take as observations what terms belong to what documents, and produce a set of topics that explain the presence of each word.
