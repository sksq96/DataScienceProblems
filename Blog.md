## A Data Science Assistance writing code in Jupyter Notebook


In the past few years, using machine learning to intelligently autofill and generate text has taken quite a leap. It started with a single word auto-compete on mobile keywords, to entire phrase completion on GMail's smart compose, to writing an entire narrative fiction using GPT3 these days. 


A similar trend has been in effect, in the genre of developer productivity tools. It started with a single code token auto-compete using IntelliSense in VSCode, to entire phrase completion using Line Completion, to writing an entire method body from natural language description using powerful models like PyMT5 and Codex.

Another area in Natural Language Processing, which has seen enormous progress is transfer learning and pre-training strategies. Using an abundant corpus of textual data available on the internet, and training transformer models with different pretraining objectives, has led to huge progress in language understanding. Be it decoder models like GPT predicting the next word, or encoder models like BERT filling in the missing word or sequence-to-sequence models like BART and T5 solving the span masking problem. 

Building upon the shoulders of these giants, we introduce JuPyT5, a model trained for data science code-generation, using a new pretraining objective of code infilling. The code infilling objective is fill in the blanks, but applied to a document level instead of word level. Instead of masking out a single word in the corpus, code infilling masks out an entire code block, say a function, and the objective is to predict the missing function given the entire code context. In the example below, the code cell is masked and given the context of data loading, problem statement, and assert statements, JuPyT5 is expected to generate the missing code to replace the string the dataframe column. 

Another challenge with language models preforming code generation is, how do we evaluate these models? Historically generated text from a language model have been evaluated using lexical word overlap using BLEU, ROUGE score. However, it would naive to assume that any form of token overlap metric might be able to successfully evaluate code generation. 

We explore the area of pedagogical learning and how we can assist students and developers alike, solving data science problems. Problems such as manipulating pandas dataframe, translating complex latex equations to code or training a machine learning model. 

