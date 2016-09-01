##eyeHeard
June 26, 2016 

*by Jostine Ho*

[badlip](https://www.youtube.com/watch?v=ufGlBv8Z3NU)

**eyeHeard** is a visual speech recognition AI that reads lips. Along with sign language, lip reading is traditionally used in the hearing impaired community. However, visual recognition of speech is a difficult task. Study shows that even an experienced lip reader can only achieve 50% accuracy. This is because speech contains around 50 distinct units of sound, but the mouth forms only roughly 15 different shapes when speaking. There is a significant amount of information loss during visual speech recognition, as a result, the translation often does not make much sense (click on the picture above, you'll know what I mean). 

The goal of eyeHeard is to minimize information loss and retrieve real textual meanings. The preliminary visual-only speech processing (short video clips) can be transcribed through a trained recurrent neural network (RNN). Though the translation accuracy after RNN might not be very high, the misinformation can be corrected using natural language processing (NLP) techniques. NLP serves to understand the main idea of the text output, evaluate the probability of word sequences and choose the correct words to replace those that are most likely wrong.  

###Data Collection

* [LiLiR Twotalk Corpus](http://www.ee.surrey.ac.uk/Projects/LILiR/datasets.html)
* Youtube clips with close caption

###Approach

* Build a recurrent neural network (RNN) using TensorFlow
* Long short-term memory (LSTM) (if nesscessary)
* Use AWS for fast computing
* Use Python NLTK package
* Perform N-grams sentence parser

###Expectations

* improve lip reading accuracy above 50%
* make a web application that uses webcam for demo
* if possible, apply to real-time lip reading
* if possible, make it into an app

###Applications

* serves as a convenient tool for the hearing impaired
* eavesdropping for creepy curious minds
* improve the accuracy of existing audio speech recognition
* serve as a backup system for malfunctioning audio system

###References

[The Challenges and Threats of Automated Lip Reading](https://www.technologyreview.com/s/530641/the-challenges-and-threats-of-automated-lip-reading/)

[Artificial Intelligence Learns to Improve Lip Reading Accuracy](http://blogs.voanews.com/techtonics/2016/04/22/artificial-intelligence-learns-to-improve-lip-reading-accuracy/)

[Interesting Facts about Lip Reading](https://www.lipreading.org/beginners-guide-to-lipreading)

[A noob’s guide to implementing RNN-LSTM using Tensorflow](https://medium.com/@monikkinom/a-noobs-guide-to-implementing-rnn-lstm-using-tensorflow-1907a5bbb1fa#.habobr5xh)

[Lip-reading computers could spell the end of badly dubbed films](http://www.sciencefocus.com/news/lip-reading-computers-could-spell-end-badly-dubbed-films)
