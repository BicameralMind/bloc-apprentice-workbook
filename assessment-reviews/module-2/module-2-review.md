# Module 2 Review Questions and Exercises

## Instructions

1. Click "edit" at the top of the page.
2. Fill in your answers below each question.
3. Save your changes and send a link to your mentor!

*Note: any topics from the first assessment should be reviewed in addition to the questions below!*

## CSS

### Questions

1. What is the box model?
- A box that wraps around every HTML element includes padding, border and margin

2. What is the difference between block and inline elements?
- block elements stack on top of each other on the page, however inline elements are grouped next to each other

3. What is responsive design?
- a design strategy where the webpage should be able to adapt to the users screen size

4. Which selector is more specific, a tag selector or class selector?
- class

5. What does `box-sizing` do?
- used to tell the browser what the sizing properties (width and height) should include

6. What's the difference between `relative` and `absolute` positioning?
- a relative positioned element is positioned relative to previous element, absolute positing allows you to place elements where you want them on a page

### Exercises

1. Write a CSS rule to turn the background color of the link with the `.btn` class blue on hover:

  ```html
  <a href="#" class="btn">Learn more</a>
  ```
  
  ```css
  a.btn:hover { 
    background-color: blue; }
  ```

2. Write a CSS rule to give the `.container` a maximum width of `980px` when the browser window is wider than `1200px`:

  ```html
  <div class="container">
    <h1>I'm a heading!</h1>
  </div>
  ```
  
  ```css
  @media (min-width: 1200px){ 
    .container { max-width: 980px;}
  }
  ```

3. Which text would be red in the following example?

  ```html
  <style>
    section p:last-child {
      color: red;
    }
  </style>

  <section>
    <p>First paragraph</p>
    <p>Second paragraph</p>
    <p>Third paragraph</p>
  </section>
  <section>
    <p>First paragraph</p>
    <p>Second paragraph</p>
    <p>Third paragraph</p>
  </section>
  ```
  - Third paragraph

4. Open this [JSBin](http://jsbin.com/qigiwuhepe/1/edit?html,css,output). Write a CSS rule using floats to make the HTML sample into a four column layout. Paste your udpated link below.

http://jsbin.com/nunebameta/edit?html,css,output

## JavaScript

### Questions

1. What is a callback?
- a function that is passed to another function as a parameter, and the callback function is called inside that function

### Exercises

1. Write a function `filterLongWords()` that takes an array of words and an integer `num` and returns the array of words that are longer than `num`.

```javascript
function filterLongWords(words, num){
  var longer = [];
  for(i = 0; i > words[i].length; i++){
    if(num.length < words[i].length)
    longer.push(words[i]);
  }
  return longer;
}
```

2. Write a function `charFreq()` that takes a string and builds a frequency listing of the characters contained in it. Represent the frequency listing as a Javascript object. Try it with something like `charFreq("abbabcbdbabdbdbabababcbcbab")`.

```javascript
function charFreq(string){
  
}
```

## DOM Scripting

### Questions

1. What does DOM stand for and what is it?
- document object model, an API that treats an HTML document as a tree structure where each node (element) is an object representing a part of the document.

### Exercises

1. Write a JavaScript statement that finds the element with the ID, `next`, and saves it to a variable called `nextButton`:

  ```html
  <a href="#" id="next" class="btn">Next</a>
  ```
  
  ```javascript
  var nextButton = document.getElementById('next');
  ```

2. Write another line that updates the text of `nextButton` to `"Next image"`.

```javascript
nextButton.textContent = "Next Image";
```

3. Write another line that adds a click event listener to `nextButton` so that when it's clicked the browser alerts `"Next image coming up."`.

```javascript
nextButton.addEventListener("click", alert("Next image coming up.");
```

## jQuery

### Questions

1. What is a JavaScript library and why do we use them?
- pre-written JavaScript which allows for easier development of JavaScript-based applications

2. What is jQuery for?
- a JavaScript library, simplifies more complicated JavaScript code, takes a lot of common tasks that require many lines of JavaScript code to accomplish, and wraps them into methods that you can call with a single line of code.

### Exercises

1. Write a statement to select all elements with the `.btn` class using a jQuery selector and save them to a variable called `buttons`:

  ```html
  <a href="#" id="next" class="btn">Next</a>
  <a href="#" id="beginning" class="btn">Beginning</a>
  <a href="#" id="previous" class="btn">Previous</a>
  ```
  
  ```javascript
  var buttons = $(".myClass");
  ```

2. Write another line that adds a click event to the buttons that logs `'click'` to the console when the button is clicked. Use the jQuery syntax.

```javascript
buttons.click(function() {
  console.log("Click");
});
```

## Angular

### Questions

1. How is a framework different than a library?
- frameworks gives you structure for your application, libraries are packages of code that typically get called by your application to perform a task

2. What is a controller?
- a JavsScript object that controls the data in the application

3. What is a view?
- the view that the user will see in their browser

4. What is a single page application?
- a web app that load a single HTML page and dynamically updates that page as the user interacts with the app

5. What is a directive in Angular?
- HTML attributes that can attach to elements to enhance funcationality

## Git

### Exercises

1. Write a command to create a new branch called `bug-fix`.
- $ git checkout -b bug-fix

2. If you're on the `master` branch, write a command to merge a branch called `bug-fix` into the `master` branch.
- $ git merge bug-fix
