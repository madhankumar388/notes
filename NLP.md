<h5>Python Library - TextBlob</h5>

from testblob import TextBlob

# Text Correction
  incorrect_line = "Heello,  i lobe nathural langueague perocesing"
  corrected_line = TextBlob(incorrect_line).correct()
  print(corrected_line)

# Noun Extraction
  sentence = "India is a country located in the Asian continent"
  for noun in TextBlob(sentence).noun_phrases:
      print(noun)

# Sentiment Analysis
  from textblob.sentiments import NaiveBayesAnalyzer
  text1 = TextBlob("The movie was excellent.", analyzer=NaiveBayesAnalyzer())
  text2 = TextBlob("The movie story pinch me a lot.", analyzer=NaiveBayesAnalyzer())
  print(text1.sentiment)
  print(text2.sentiment)
  
https://textblob.readthedocs.io/en/dev/quickstart.html
