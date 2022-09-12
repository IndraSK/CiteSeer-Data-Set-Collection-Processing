{
 "cells": [
  {
   "cell_type": "markdown",
   "id": "cc7bf411",
   "metadata": {},
   "source": [
    "# CiteSeer Data Set Collection Processing (CS582: Information Retrieval)\n",
    "\n",
    "This project is part of a homework assignment for CS582: Information Retrieval course at the University of Illinois at Chicago.\n",
    "\n",
    "----\n",
    "\n",
    "The CiteSeer UMD collection is a standard text document collection, consisting of abstracts of research articles from Computer Science, which are sampled from the CiteSeer digital library. \n",
    "\n",
    "---\n",
    "\n",
    "**Tasks**\n",
    "\n",
    "1. Write a program that preprocesses the collection. This preprocessing stage should specif- ically include a function that tokenizes the text. In doing so, tokenize on whitespace and remove punctuation.\n",
    "2. Determine the frequency of occurrence for all the words in the collection. Answer the following questions:\n",
    "    * What is the total number of words in the collection?\n",
    "    * What is the vocabulary size? (i.e., number of unique terms).\n",
    "    * What are the top 20 words in the ranking? (i.e., the words with the highest frequencies).\n",
    "    * From these top 20 words, which ones are stop-words?\n",
    "    * What is the minimum number of unique words accounting for 15% of the total number of words in the collection?\n",
    "3. Integrate a stemmer and a stopword eliminator into your code. Answer again questions from the previous point.\n",
    "\n",
    "---\n",
    "\n",
    "**Instructions**\n",
    "\n",
    "Check out the [Jupyter Notebook](citeseer.ipynb) to see the python implementation of the tasks.\n",
    "\n",
    "Check out the [article](https://www.codecademy.com/article/how-to-use-jupyter-notebooks) to implement code in Jupyter Notebook.\n",
    "\n",
    "Please run ```pip install -U gensim``` command in-order to import the gensim library which is used for removing the stopwords.\n",
    "\n",
    "----\n",
    "\n",
    "**Results**\n",
    "\n",
    "Task 2:\n",
    "\n",
    "* Total number of words in the collection : 476203\n",
    "* Vocabulary size (number of unique words) : 19890\n",
    "* Top 20 words in the ranking and their frequencies :\n",
    "  'the': 25662, 'of': 18638, 'and': 14131, 'a': 13345, 'to': 11536, 'in': 10067, 'for': 7379, 'is': 6577, 'we': 5138, 'that': 4820, 'this': 4446, 'are': 3737, 'on': 3656, 'an': 3281, 'with': 3200, 'as': 3057, 'by': 2765, 'data': 2691, 'be': 2500, 'information': 2322\n",
    "* Stop-words out of the top 20 words :\n",
    "  'the','of','and','a','to','in','for','is','we','that','this','are','on','an','with','as','by','be'\n",
    "* Minimum no. of unique words accounting for 15% of the total number of words in the collection : 6\n",
    "\n",
    "  \n",
    "Task 3:\n",
    "\n",
    "* Total number of words in the collection : 284504\n",
    "* Vocabulary size (number of unique words) : 17029\n",
    "* Top 20 words in the ranking :\n",
    "  'data': 2763, 'based': 2534, 'information': 2359, 'paper': 2211, 'systems': 1830, '1': 1783, 'agent': 1688, 'agents': 1565, 'web': 1556, 'learning': 1499, 'user': 1306, 'model': 1241, 'approach': 1169, 'query': 1168, 'search': 1032, 'problem': 1023, 'new': 977, 'use': 959, 'introduction': 952, 'time': 930\n",
    "* Stop-words out of the top 20 words : None (All the stop words have been removed)\n",
    "* Minimum no. of unique words accounting for 15% of the total number of words: 36"
   ]
  }
 ],
 "metadata": {
  "kernelspec": {
   "display_name": "Python 3",
   "language": "python",
   "name": "python3"
  },
  "language_info": {
   "codemirror_mode": {
    "name": "ipython",
    "version": 3
   },
   "file_extension": ".py",
   "mimetype": "text/x-python",
   "name": "python",
   "nbconvert_exporter": "python",
   "pygments_lexer": "ipython3",
   "version": "3.8.8"
  }
 },
 "nbformat": 4,
 "nbformat_minor": 5
}
