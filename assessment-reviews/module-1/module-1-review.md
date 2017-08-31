# Module 1 Review Questions and Exercises

## Instructions

1. Click "edit" at the top of the page.
2. Fill in your answers below each question.
3. Save your changes and send a link to your mentor!

## HTML

### Questions

1. What is HTML and what is it used for?
  - Stands for HyperText Markup Language and is used to create documents that become web pages
  
2. What is the difference between an ID and a class?
  - An ID is an attribute that can be attached to only one HTML element. A class can be used on an infinite amount of      elements.
  
3. What does it mean to write "semantic" HTML?
  - Creating a meaning behind certain HTML tags

### Exercises

1. Write a paragraph tag with a class of "highlight" and content "Watch out!".
  
  ```html
  <p class="highlight">Watch out!</p>
  ```

2. Write an HTML image tag to show an image called `profile-picture.jpg`.
  
  ```html
  <img src="profile-picture.jpg>
  ```
  
3. Write a link tag that links to http://google.com.
  
  ```html
  <a href="http://google.com></a>
  ```
  
5. Write an complete standard HTML document outline (including a DOCTYPE, and `<html>`, `<head>`, and `<body>` tags).
  
  ```html
    <!DOCTYPE html>
    <html>
      <head>
        (7) <link href="main.css" rel="stylesheet" type="text/css">
      </head>
      <body>
        (6) <script src="main.js" type="text/javascript"></script>
      </body>
    </html>
  ```

6. Inside of the code for the previous exercise, write the appropriate tag to link to a script file called `main.js`.
7. Inside of the code for the previous exercise, write the appropriate tag to link to a stylesheet file called `main.css`.
8. Write a numbered list in HTML and list three of your favorite books.
  -
  ```html
    <ul>
      <li>Ready Player One - Ernest Cline</li>
      <li>Mistborn: The Well of Ascension - Brandon Sanderson</li>
      <li>Timeline - Michael Crichton</li>
    </ul>
  ```

9. Fix the indentation of the following HTML sample:

  ```html
  <div>
    <ul>
      <li>Item 1</li>
      <li>Item 2</li>
      <li>Item 3</li>
    </ul>
  </div>
  ```

## CSS

### Questions

1. What is CSS and what is it used for?
  - Stands for Cascading Style Sheets, used to add styling to HTML elements

2. What is the CSS box model?
  - A box that wraps around every HTML element includes padding, border and margin
  
3. What's the difference between margin and padding?
  - Margin will add space outside of the element, padding will add space inside

### Exercises

1. Write a CSS rule to make the text of all `h1` tags red.
  - h1 {
      color: red; }

2. Write a CSS rule to make the background color of the link with `class="btn"` blue:

  ```html
  <a href="#" class="btn">Learn more</a>
  ```
  .btn {
    background-color: blue; }

3. Write a CSS rule to give the first paragraph in the following HTML a font size of `20px`, but not the second paragraph.

  ```html
  <header class="jumbotron">
    <p>Hello, World!</p>
  </header>

  <p>Welcome to this awesome website!</p>
  ```
  .jumbotron p {
    font-size: 20px; }

## JavaScript

### Questions

1. What is a function? What are they used for?
  - a set of statements that performs a task and used to make a site interactive

2. What is the difference between `==` and `===`?
  - With "---" type and value must be the same to be true, "==" can be true without having both values be of the same type (string and number)
  
3. What is the difference between global and local scope variables?
  - global variables can be used throughout the entire JS document, local scope variables can only be used within the function in which they are called
  
4. What is a boolean value?
  - a true or false value
  
5. What is an array?
  - arrays hold multiple values in a single variable (store a list of items/values)

### Exercises

1. Write a line that declares a variable called `myName` and set its value to your name.
  - var myName = "Michael Fraino";
  
2. Write a loop that logs the numbers 1 through 10 to the console.
  
  ```javascript
  for(var i = 1; i <= 10; i++){
      console.log(i);
  }
  ```
    
3. Translate the following pseudocode into JavaScript: if `score` is greater than `3` and `lives` is greater than `0`, alert "You win!".
 
 ```javascript
 if(score > 3 && lives > 0) {
      alert("Your win!"); 
 }
 ```
    
4. Write a function `sayHello` that takes one argument, a name, and logs "Hello, <name>!" to the console. Then, call the function below the function definition and pass in your name as the argument.
 
 ```javascript
 function sayHello(name){
      console.log("Hello, " + name + "!");
 }
    
 sayHello(Michael);
 ```


5. What would the following script log to the console?

  ```javascript
  var currentSong = "Call Me Maybe";

  function setSong(song) {
    currentSong = song;
  }

  setSong("Friday, Friday");

  console.log(currentSong);
  ```
  
  answer: Friday, Friday

6. What would the following script log to the console?

  ```javascript
  var add = function(a, b) {
    return a + b;
  }

  var result = add(3, 7);

  console.log(result);
  ```
  answer: 10

7. What would the following script log to the console?

  ```javascript
  var helloGoodbye = function(name) {
    return sayHello(name) + " " + sayGoodbye(name);
  }

  var sayHello = function(name) {
    return "Hello " + name " !";
  }

  var sayGoodbye = function(name) {
    return "Goodbye " + name " !";
  }

  console.log(helloGoodbye("Sarah"));
  ```
  answer: Hello Sarah ! Goodbye Sarah !

8. Write a function `findLongestWord()` that takes an array of words and returns the length of the longest one.
  
  ```javascript
  function findLongestWord(words){
    var longest = 0;
    
  }
  ```

9. Define a function `sum()` that sums all the numbers in an array of numbers. For example, `sum([1,2,3,4])` should return 10.

```javascript
function sum(numbers) {
  var total = 0;
	for (var i = 0; i < numbers.length; i++) {
		total += numbers[i];
	}
	return total;
}
```

10. Write a function that takes a character (i.e. a string of length 1) and returns true if it is a vowel, false otherwise.

```javascript
function isVowel(x){
  if(x = "a" || x = "e" || x = "i" || x = "o" || x = "u"){
    return true;
  } else {
      return false;
    }
}
```

11. Write the correct line to make `"Woof!"` show up in the console based on this script:

  ```javascript
  var pet = {
    name: "Charles",
    goodDog: true,
    speak: function() {
      console.log("Woof!");
    }
  };
  ```
  answer: pet.speak()

12. Using the same script as above, write the correct line to log the dog's name to the console.
  - console.log(pet.name)

## Command Line

### Questions

1. What is the command line and what is it used for?
- A way to interact with a computer and programs by sending commands through text in the console

2. What does the command `ls` do?
- lists files in the current working directory

3. What does the command `pwd` do?
- print working directory, shows the directory you're currently working with

4. What does the following command do: `cd my-cool-project`
- it will take you to the directory "my-cool-project"

### Exercises

1. Write the command to make a new directory called "my-cool-project".
- mkdir my-cool-project

2. Write the command to create a file called "index.html".
- touch index.html

3. Write the command to delete a file called "main.css".
- rm main.css

## Git

### Questions

1. What is Git and what is it used for?
- a distributed version control system that allows you to record changes to your files and allows others to access via remote repositories 

2. What's the difference between a local repository and a remote repository?
- local is stored on the computer you are working on, a remote is elsewhere (GitHub, some other server)

### Exercises

1. Write the command that you would use to create a new local Git repository.
- git init

2. Write the command to stage a file called `index.html` to be committed.
- git add index.html

3. Write the command to view the current status of the git repository.
- git status
