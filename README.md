# Project 1 Generative Text

Kasidech Tantipanichaphan, ktantipa@ucsd.edu

(Your teammate's contact info, if appropriate)

## Abstract

<sup>*Side Note: My original idea was to generate the movie 'IT' screenplay, however I decided to change to Goosebumps: Welcome to the Dead House text since the storyline is a lot more interesting and at the same time easier to understand for the audience. (Still, I kept the same halloween concept)</sup>


As the Halloween event is approaching, I decided to remake the horror story based on one of the first R.L. Stine masterpiece that makes him live up to his title: ‘Goosebumps: Welcome to Dead House’,  by using a text generator. The goal of this project is that I wanted to create a “remake’’ for this book by using rnn. In order to see how the text generator could describe the story in its own ways. For visualization, I decided to draw out the scene in order to complement the generated text. The drawing process takes some time to finish, and the scene makes sense for that generated text. As a brief storyline, this is the story of the Benson family and their new home in Dark Falls. Come to find out, everyone in their new town is a zombie, and that every year they require new blood. That fresh blood comes from tricking families into moving into the so-called "dead house" and then murdering them. According to Glamour blog, this Goosebumps tale was our first prep for a zombie apocalypse, long before The Walking Dead. 

There are minor differences using a text generator. In the generated story, it turns out that everyone died at the end. However, in the original story everyone in the Benson family survived at the end, by escaping from the zombies town. Another difference is that Mr. Dawes, the real-estate agent turns out to be a zombie. When the original story, everyone that lives in that neighborhood is the zombie. Lastly, one of the characters is missing in the text, such as Karen. Otherwise, most of the generated text seems to conform to the original story.

## Model/Data

The data that I fetched is from this website: 

https://archive.org/stream/GoosebumpsDeadHouse/GoosebumpsDeadHouse_djvu.txt

As described in the Abstract section, I decided to use a beautiful soup to extract the text from the book. Basically, I perform a web scraping and do data cleaning in order to remove the stuff that is irrelevant to the text, such as page numbers or appendix.  

This first part here is going to be the data cleaning process by using beautiful soup.

First I retrieve the contents on a page and examine them a bit.

I make a variable called `link`, that stores the following URL (as a string):
'https://archive.org/stream/GoosebumpsDeadHouse/GoosebumpsDeadHouse_djvu.txt' 

Now, to open the URL, use `requests.get()` and I provide `link` as its input. Store this in a variable called `page`.

After that, make a variable called `soup` to parse the HTML using `BeautifulSoup`.

This is what the content looks like originally:

![Alt text](https://github.com/ucsd-ml-arts/generative-text-ktantipa/blob/master/Images/web_scraping.png)

Then I extract the text from the page and save it in a variable. I extract it as a string.

To do so, I have to use the soup object created in the above cell. 

The next step is to remove the ‘\n’ by using the replace command. The page numbers were also removed, by using isdigit().

After the steps above, the following becomes the new result of the content:

![Alt text](https://github.com/ucsd-ml-arts/generative-text-ktantipa/blob/master/Images/Screen%20Shot%202019-10-17%20at%204.04.05%20PM.png)

## Code

All the code files are in this github

## Results

The final result of the generated story can be found in this github, the file is called 'Goosebumps_generated_text_(Final_remake).pdf'

## Technical Notes


## Reference

https://archive.org/stream/GoosebumpsDeadHouse/GoosebumpsDeadHouse_djvu.txt - Goosebump Text
