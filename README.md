# TYPING PRACTICE
#### Website Link: <https://evernew998.github.io/typingPractice_website/>
#### Video Demo: <https://youtu.be/eSyUkDvDXcE>
## Description:

Typing Practice is a website developed using Python, Flask, Javascript, HTML, and CSS. Its purpose is to allow people to practice their typing skills by typing a set number of random words. This website will then calculate their typing speed and accuracy. Currently, Typing Practice only supports two languages, English and Bahasa Malaysia. Also, it only supports the QWERTY keyboard layout. It requires the user to have a keyboard to work. So, it usually only works on desktops and laptops. I chose this project because I wanted to practice using Javascript. 

## Usage

Here is the procedure for using Typing Practice:
1. Choose a language to practice typing in by clicking on the language option tab at the top right-hand corner.
2. Select the total number of words to type in a single practice session by clicking on a number in the total number of words section at the bottom middle of the screen.
3. Type the random words that you see above the typing area. If you spell a letter correctly, the corresponding letter will turn green. If you spell it incorrectly, then it will turn red.
4. After you finish typing all the words, Typing Practice will calculate your gross words per minute, typing accuracy, and adjusted typing speed. To know more about how we calculate these values, go to this link: https://www.typetolearn.app/knowledge-base/how-words-per-minute-and-accuracy-are-calculated/
5. To reset everything, click the reset button in the middle of the screen, or change the total number or the language of the random words. The reset button will only appear after you have finished typing all the random words.

## File content

There are five files in this project, excluding the README.md file. These are app.py, layout.html, index.html, styles.css, and requirements.txt. The app.py file contains code to create the most basic Flask application. The layout.html file is just a barebones HTML layout. It has one CSS attribute, font-size:clamp(2.5rem, 2.125rem + 1.875vw, 4.375rem), that is important in controlling the responsiveness of the font size. It allows font size to scale according to screen size, which makes the website look great on most devices. The index.html file contains all the Javascript code that controls the webpage features. These features manage:
1. The total number of random words.
2. The number of random words shown on the screen at a given time.
3. The letters' colour change.
4. The calculation of typing speed and accuracy.
5. The language of the random words.
6. The stopwatch.
7. The reset button.

The styles.css file contains the code that styles the content of the webpage. Generally, letters are in white, except for the first random word shown on the screen. The letters in those words can either be white, green or red. Words' font size scales depending on the screen size. They shrink to fit smaller screens and grow for larger screens. The overall style of the webpage is simple to avoid distractions during typing. It is also in "dark mode" for a better experience in dark environments. The requirements.txt file contains the Python packages needed to run this project smoothly. Those Python packages are Flask, Flask-sessions, and requests.

## Challenges

The biggest challenge I faced when developing this website was implementing the letter colour change feature. This feature changes the letter to green when the user types it correctly. Otherwise, it turns the letter red. Implementing this feature felt like I was trying to solve one of CS50's earlier problem sets. On the surface, the feature seemed simple. However, looking deeper, I discovered that there were more conditions that I needed to take into consideration. These conditions were:
1. If the user spells a letter correctly, it should turn green only if the previous letter is green or if it is the first letter. 
2. If the previous letter is red, the current letter should also turn red regardless if the user spelt it correctly.
3. When a user misspells a letter, the letter should turn red. A letter misspelling occurs when the key pressed by the user is unequal to the letter. However, the key has to produce a character on screen. So, keys like the "Shift" or "Enter" keys do not count as they do not create any character. Therefore, if the user presses any of these keys, the letter colour should not turn red.

My biggest mistake was going straight into coding when trying to solve the new problems that kept popping up. Instead, even before doing anything, I should have taken the time to figure out exactly how the feature would work.

## Potential features

In the future, if I decide to improve the project, I would like to add a couple of features. One is support for other keyboard layouts such as Dvorak and Colemak. Another is allowing users to make accounts to keep track of their progress. I also want to improve how the random words appear on the screen. Currently, the words' positions change depending on their length. Ideally, I want them to stay in the same place throughout the session so that users do not have to track their movement. Hopefully, it would make it less distracting and improve the typing experience.

## Acknowledgments

I want to thank David J. Malan, Carter Zenke, Doug Lloyd, Brian Yu, and the rest of the CS50 team for providing an incredible computer science course that has and will continue to inspire current and future programmers. Thanks to CS50, I was able to create and develop my very first website, Typing Practice, from scratch. Typing Practice takes a lot of inspiration from www.colemak.academy. I essentially wanted to make a copy of that website. It is where I got most of my ideas from. Below is a list of the resources I used in this project:
1. https://cs50.harvard.edu/x/2023/ 
2. https://www.colemak.academy/
3. https://www.w3schools.com/js/js_array_sort.asp
4. https://www.typetolearn.app/knowledge-base/how-words-per-minute-and-accuracy-are-calculated/
5. https://css-tricks.com/linearly-scale-font-size-with-css-clamp-based-on-the-viewport/
6. https://www.espressoenglish.net/100-most-common-english-verbs/
7. https://www.espressoenglish.net/100-common-nouns-in-english/
8. https://www.espressoenglish.net/100-common-english-adverbs/
9. https://www.espressoenglish.net/100-common-adjectives-in-english/
10. https://www.vocabulary.com/lists/133109
11. https://www.vocabulary.com/lists/151206
12. https://www.pinhok.com/kb/malay/230/100-basic-malay-vocabularies/
13. https://getbootstrap.com/
