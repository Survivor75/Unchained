# Unchained
This repository contains nuggets on the following : 1. JavaScript 2. Python

##  JavaScript

### Particles
Creating particles using JavaScript

![alt text](https://github.com/Survivor75/Unchained/blob/master/JavaScript/partcles/img/particles.png?raw=true "particle.js")

### DrumKit
Drum Kit implementation in vanilla JavaScript


![alt text](https://github.com/Survivor75/Unchained/blob/master/JavaScript/Drum_Kit/img/drum_kit.PNG?raw=true "drum kit")

### D3IndiaNF
NowFloats Technologies 's customer data mapped across India  using D3.js.

Features :
1. Data Visible on Hover
2. Ripples Animation
3. Zoom-In Zoom-Out of States

![alt text](https://github.com/Survivor75/Unchained/blob/master/JavaScript/D3IndiaNF/img/india_nf.PNG?raw=true "")

### NF_MAP
Backend for D3IndiaNF implemented in Node.js Express and MongoDB

### Baz_Man
The game is roughly based on Dark Blue by Thomas Palef. I chose that game because it is both entertaining and minimalist. It looks like this (Level 1):

![alt text](https://github.com/Survivor75/Unchained/blob/master/JavaScript/Baz_Man/img/level_1.PNG?raw=true "")

The dark box represents the player, whose task is to collect the yellow boxes (coins) while avoiding the red stuff (lava). A level is completed when all coins have been collected.

The player can walk around with the left and right arrow keys and can jump with the up arrow. Jumping is a specialty of this game character. It can reach several times its own height and can change direction in midair. This may not be entirely realistic, but it helps give the player the feeling of being in direct control of the on-screen avatar.

As of now it has 3 levels
Level 2

![alt text](https://github.com/Survivor75/Unchained/blob/master/JavaScript/Baz_Man/img/level_2.PNG?raw=true "")

Level 3

![alt text](https://github.com/Survivor75/Unchained/blob/master/JavaScript/Baz_Man/img/level_3.PNG?raw=true "")


### Rock Paper Scissor

![alt text](https://github.com/Survivor75/Unchained/blob/master/JavaScript/rock_paper_scissor/img/rps.PNG?raw=true "")


### Speech Detection

![alt text](https://github.com/Survivor75/Unchained/blob/master/JavaScript/SpeechDetection/img/speech.PNG?raw=true "")


### Regular Language

"*The evaluator, which determines the meaning of expressions in a programming language, is just another program.*"
- Hal Abelson and Gerald Sussman, Structure and Interpretation of Computer Programs

Regular Language is my take on developing my own programming language using regular expressions.
Everything here is an expression. An expression can be the name of a binding, a number, a string, or an *application*. Applications are used for function calls but also for constructs such as ```if``` or ```while```.

To keep the parser simple, it does not support anything like backslash escapes. A string is simply a sequence of characters that are not double quotes, wrapped in double quotes. A number is a sequence of digits. Binding names can consist of any character that is not whitespace and that does not have a special meaning in the syntax.

Applications are written the way they are in JavaScript, by putting parentheses after an expression and having any number of arguments between those parentheses, separated by commas.

```do(define(x, 10),
   if(>(x, 5),
      print("large"),
      print("small")))
```
The uniformity of the language means that things that are operators in JavaScript (such as >) are normal bindings in this language, applied just like other functions. And since the syntax has no concept of a block, we need a do construct to represent doing multiple things in sequence.

The data structure that the parser will use to describe a program consists of expression objects, each of which has a type property indicating the kind of expression it is and other properties to describe its content.

Expressions of type "value" represent literal strings or numbers. Their value property contains the string or number value that they represent. Expressions of type "word" are used for identifiers (names). Such objects have a name property that holds the identifier’s name as a string. Finally, "apply" expressions represent applications. They have an operator property that refers to the expression that is being applied, as well as an args property that holds an array of argument expressions.

The >(x, 5) part of the previous program would be represented like this:
```
{
  type: "apply",
  operator: {type: "word", name: ">"},
  args: [
    {type: "word", name: "x"},
    {type: "value", value: 5}
  ]
}
```
Such a data structure is called a syntax tree.

## Python

### UnsplashScraper
Ingredients for a simple Image Scraper

1. Python (3.6.3 or newer)
2. Pycharm (Community edition is just fine)
3. pip install requests Pillow selenium
4. geckodriver 
5. Mozlla Firefox (as if you didn’t have it installed)
6. Working internet connection (obviously)
7. 30 minutes of your time (possibly less)
