Data Science Capstone: Predicting the Next Word
========================================================
author: Amyas Walji
date:  November, 2019
autosize: true
transition: rotate
transition-speed: slow
incremental: true
font-import: http://fonts.googleapis.com/css?family=Helvetica
font-family: 'Helvetica'

<div>
<img src="coursera.png" style="width:15%"
</div>

Overview
========================================================

<small>The recent advances in mobile technology have enabled people to stay connected on the go. However, to communicate by text swiftly without error on a smartphone keyboard is rather challenging without any language prediction.</small> 

<small>In this backdrop, the purpose of the Data Science Capstone project was to develop a data product which uses natural language processing to predict the next word a user may want to type. A shiny application serves as the final product for this project.</small>

<small>The application is available at the following link:
<a href="http://45.55.48.122/" target="_blank">Shiny App</a>.</small>

Model and algorithm
========================================================

<small>The prediction algorithm developed is based on an N-Gram Language Model. This model uses a Markov Assumption in which each word depends only on the previous N words in a given string of text. For this project a series of four N-gram models have been constructed:</small><small>
* Unigram: previous words do not matter
* Bigram: only the previous word matters
* Trigram: only the previous two words matter
* Quadgram: only the previous three words matter.</small>

<small>Given this dictionary of N-grams, the algorithm chooses candidates observed in the input text and through Maximum-Likelihood Estimation combined with Good Turing Smoothing returns the probabilities for possible next words. The implementation of returning a fitting response is built using a Backoff Model.</small>   

The Application
========================================================
incremental: false
<small>
The Shiny application offers an intuitive and simple graphical user interface that can easily be adapted for educational and commercial uses. The dashboard presents the user with a text input box, which when filled out with a word or short phrase returns a prediction along with a dynamic table suggesting possible next words and a word cloud visualizing the top predictions.</small> </small>
<div>
<img src="CapstoneApp.png" style="width:75%"
</div>




Thanks!
========================================================
incremental: false

<small>
Shiny App    
<a href="http://45.55.48.122/" target="_blank">Link</a>.

Shiny App Source Code on Github    
<a href="https://github.com/wowkazmir/Data-Science-Capstone" target="_blank">Link</a>.

Data Science Capstone on Coursera    
<a href="https://www.coursera.org/learn/data-science-project" target="_blank">Link</a>.
