# Project 1 Generative Text

Kasidech Tantipanichaphan, ktantipa@ucsd.edu

(Your teammate's contact info, if appropriate)

![alt text](https://github.com/ucsd-ml-arts/generative-text-ktantipa/tree/master/Images/it-chapter-two.png)

## Abstract

Include your abstract here. This should be one paragraph clearly describing your concept, method, and results. This should tell us what architecture/approach you used. Also describe your creative goals, and whether you were successful in achieving them. Also could describe future directions.

As Halloween event is approaching, I decided to rewrite a new horror film by using a script from my favorite movies, IT chapter one and two. The purpose for this project is that I wanted to create a ‘bonus’ chapter for this movie, even though the storyline is already finished. For visualization, I decided to pick several scenes from the movie in order to complement the generated text. The scene makes sense for that generated text. For building the model, I set the embedding dimension to 1024. In the neural network model, I decided to use the LSTM layer instead. I decided to add two more LSTM layers and dropouts, because... I trained with 50 epochs with the temperature value around 0.5. Based on the experiment, the higher temperature would cause nonsense wording. On the other hand, temperature close to zero would cause a repetition of words. In the context of the script, some of the sentences seems to make sense and some didn’t.  


## Model/Data

Briefly describe the files that are included with your repository:
- trained models
- training data (or link to training data). what is your corpus?

## Code

Your code for generating your project:
- training_code.py or training_code.ipynb - your training code
- generative_code.py or generative_code.ipynb - your generation code

## Results

- Documentation of your generative text in an effective form. A file with your generated text (.pdf, .doc, .txt). 

## Technical Notes

Any implementation details or notes we need to repeat your work. 
- Does this code require other pip packages, software, etc?
- Does it run on some other (non-datahub) platform? (CoLab, etc.)

## Reference

References to any papers, techniques, repositories you used:
- Papers
  - [This is a paper](this_is_the_link.pdf)
- Repositories
- Blog posts
