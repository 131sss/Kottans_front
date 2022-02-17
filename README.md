# frontend
[Study Plan](https://github.com/kottans/frontend/blob/master/contents.md#stage-0-self-study)


**Completed tasks:**

General
- [x] [0. Git Basics](#0-Git-Basics)
- [x] [1. Linux CLI, and HTTP](#1-Linux-CLI-and-HTTP)
- [x] [2. Git Collaboration](#2-Git-Collaboration)

Front-End Basics
- [x] [3. Intro to HTML and CSS](#3-Intro-to-HTML-and-CSS)
- [x] [4. Responsive Web Design](#4-Responsive-Web-Design)
- [x] [5. HTML and CSS practice Hooli-style Popup](#5-HTML-and-CSS-practice-Hooli-style-Popup) (practice)
- [x] [6. JavaScript Basics](#6-JavaScript-Basics)
- [ ] [7. Document Object Model](#7-Document-Object-Model)
- [ ] [7. Document Object Model Practice](#7-Document-Object-Model-Practice)

Advanced Topics
- [ ] [8. Building a Tiny JS World](#8-Building-a-Tiny-JS-World)
- [ ] [9. Object oriented JS](#9-Object-oriented-JS)
- [ ] [10. OOP exercise](#10-JS-post-OOP)
- [ ] [11. Offline Web Applications](#11-Offline-Web-Applications)
- [ ] [12. Memory pair game](#12-Memory-pair-game)
- [ ] [13. Website Performance Optimization](#13-Website-Performance-Optimization)
- [ ] [14. Friends App](#14-Friends-App)


## General

### 0. Git Basics 

It was good to refresh the knowledge about git and different git commands.
git rebase definitely helps to keep git history clearer.


### 1. Linux CLI and HTTP

I liked site about Linux because you can read theory and practice after that.
It has a good explanation about base commands, permissions, etc.
I would recommend this site to everyone who wants to learn Linux.

ALso information about HTTP was useful. But I would add a simple article about
REST API, to better understand where and how statuses and methods are used.

**Screenshots**

- [Linux-Tutorial-Quiz-1](task_linux_cli/Linux-Tutorial-Quiz-1-Linux-Survival.png?raw=true)
- [Linux-Tutorial-Quiz-2](task_linux_cli/Linux-Tutorial-Quiz-2-Linux-Survival.png?raw=true)
- [Linux-Tutorial-Quiz-3](task_linux_cli/Linux-Tutorial-Quiz-3-Linux-Survival.png?raw=true)
- [Linux-Tutorial-Quiz-4](task_linux_cli/Linux-Tutorial-Quiz-4-Linux-Survival.png?raw=true)


### 2. Git Collaboration

**what was new:** working with forked repository
```commandline
git remote add upstream https://github.com/udacity/course-collaboration-travel-plans.git
git fetch upstream master
# merge in Lam's changes
git merge upstream/master
# send Lam's changes to *my* remote
git push origin master
```
**what was surprised:** -
**what intend to use in future:** squashing the commits
```commandline
git rebase -i HEAD~3
```
use p or pick – to keep the commit as is  
use r or reword – to keep the commit's content but alter the commit message  
use s or squash – to combine this commit's changes into the previous commit (the commit above it in the list)

**Screenshots**

- [GitHub-Collaboration-Udacity](task_git_collaboration/GitHub-Collaboration-Udacity.png?raw=true)
- [Learn-Git-Branching](task_git_collaboration/Learn-Git-Branching.png?raw=true)


## Front-End Basics


### 3. Intro to HTML and CSS

**what was new:** 
* some new tags from HTML5 
    * `<nav>`
    * `<header>`
    * `<main>`
    * `<footer>`
    * `<section>`
    * `<article>`
    * `<figure>`
    * `<figcaption>`
    * `<small>`
* `<datalist>` input
* `grid` and `flex` CSS

**what was surprised:** 
* CSS transitions 
  
**what intend to use in future:** 
* developer tools
* new tags and CSS

**Screenshots**
- [Intro-to-HTML-and-CSS-Udacity](task_html_css_intro/Intro-to-HTML-and-CSS-Udacity.png?raw=true)
- [Learn-HTML-Codecademy](task_html_css_intro/Learn-HTML-Codecademy.png?raw=true)
- [Learn-CSS-Codecademy](task_html_css_intro/Learn-CSS-Codecademy.png?raw=true)


**Useful links:**
* [HTML Cheat Sheet](https://www.codecademy.com/learn/learn-html/modules/learn-html-elements/cheatsheet)
* [CSS Cheat Sheet](https://www.codecademy.com/learn/learn-css/modules/learn-css-selectors-visual-rules/cheatsheet)


### 4. Responsive Web Design

**what was new:** 
* viewport
* media-queries
* breakpoints


**what was surprised:** 
  
  
**what intend to use in future:** 
* flex and media-queries


**Screenshots**
- [Responsive-Web-Design-Fundamentals-Udacity](task_responsive_web_design/Responsive-Web-Design-Fundamentals-Udacity.png?raw=true)
- [Flexbox-Froggy](task_responsive_web_design/Flexbox-Froggy-Игра-для-изучения-CSS-Flexbox.png.png?raw=true)



**Tips**
* Width 100% is always relative and therefore responsive.
```css
img, embed, video {
  max-width: 100%;
}
```
* max-width actually overrides the width
* 125 pixels is pretty much smaller than any device, 
so logo 125 px will actually work well and be responsive.
* Tap targets should be bigger than the average finger. 
So, to ensure that all of your elements are at least that size, 
add min-height: 48px; and min-width: 48px; to every tappable element.  
height and width alone can be a little dangerous because 
it won't allow the element to resize 
if the content inside of it is bigger than the container.
* 2 breakpoints for different width
* 65 characters per line - optimal length


### 5. HTML and CSS practice Hooli-style Popup

**Demo:**  
https://tavor118sn.github.io/kottans-html-css-popup/

**Repo:**  
https://github.com/tavor118sn/kottans-html-css-popup


**Tips**
* Input can be placed in `<label>`
```html
<label class="check">
  <input class="check__input" type="checkbox">
</label>
```
* Visually hidden:
```css
.visually-hidden {
  position: absolute;
  width: 1px;
  height: 1px;
  margin: -1px;
  padding: 0;
  overflow: hidden;
  border: 0;
  clip: rect(0 0 0 0)
}
```


**Useful links:**
* [Custom Checkbox - Vadim Makeev](https://www.youtube.com/watch?v=E6kLaaQFctU&ab_channel=VadimMakeev)
* [How to hide - htmlacademy](https://htmlacademy.ru/blog/boost/frontend/short-12)
* [You Need to Stop Targeting Tags in CSS](https://frontstuff.io/you-need-to-stop-targeting-tags-in-css)


### 6. JavaScript Basics

**what was new:** 
* Anonymous Function expression, Named function expressions  
(when a function is assigned to a variable),  
and Function declaration.
* A function that is passed into another function is called a callback.
* for loop, forEach() and map() to loop through an array

**Tips**
* JavaScript provides eight different data types which are 
undefined, null, boolean, string, symbol, bigint, number, and object.
* `contacts.hasOwnProperty(prop)` => `prop in contacts`
* ES6
    * Arrow Functions 
    ```javascript
    const myFunc = () => "value";
    const doubler = (item) => item * 2;
    const multiplier = item => item * 2;
    ```
    * Rest Parameter `function howMany(...args)`
    
    * Spread Operator to Evaluate Arrays In-Place
    ```javascript
    const maximus = Math.max(...arr);
    let thatArray = ['basil', 'cilantro', ...thisArray, 'coriander'];
    ```
    
    * Destructuring Assignment to Extract Values from Objects and Arrays
    ```javascript
    const user = { name: 'John Doe', age: 34 };
    const { name, age } = user;
    const { name: userName, age: userAge } = user;  
    
    const [a, b,,, c] = [1, 2, 3, 4, 5, 6];
    const [a, b, ...arr] = [1, 2, 3, 4, 5, 7];
  
    const ratings = watchList.map(({ Title: title, imdbRating: rating }) => ({title, rating}));
    ```
    
    * Destructuring Assignment to Pass an Object as a Function's Parameters
    ```javascript
    const profileUpdate = ({ name, age, nationality, location }) => {
      /* do something with these fields */
    }
    ```
    
    * Create Strings using Template Literals
    ```javascript
    const greeting = `Hello, my name is ${person.name}!
    I am ${person.age} years old.`;
    ```
    
    * Object Literal Declarations Using Object Property Shorthand
    ```javascript
    const getMousePosition = (x, y) => ({ x, y });
    ```
    
    * Declarative Functions
    ```javascript
    const person = {
      name: "Taylor",
      sayHello() {
        return `Hello! My name is ${this.name}.`;
      }
    };
    ```
    
    * Constructor Function
    ```javascript
    class SpaceShuttle {
      constructor(targetPlanet) {
        this.targetPlanet = targetPlanet;
      }
    }
    const zeus = new SpaceShuttle('Jupiter');
    ```
    
    * getters and setters to Control Access to an Object
    ```javascript
    class Book {
      constructor(author) {
        this._author = author;
      }
      // getter
      get writer() {
        return this._author;
      }
      // setter
      set writer(updatedAuthor) {
        this._author = updatedAuthor;
      }
    }
    const novel = new Book('anonymous');
    console.log(novel.writer);  // anonymous
    novel.writer = 'newAuthor';
    console.log(novel.writer);  // newAuthor
    ```
    
* Array functions
    * `every`
    ```javascript
    function isEveryoneHere(obj) {
      return ["Alan", "Ryan"].every(name => obj.hasOwnProperty(name));
    }
    ```
    
    * some
    ```javascript
    arr.some(elem => elem > 0);
    ```
    
    * `filter`
    ```javascript
    const millionPlusCities = cities.filter(function (e) {
      return e.population > 1000000;
    });
    var millionPlusCities = cities.filter(e => e.population > 1000000);
  
    const divisibleByThrreeES6 = array.filter(v => v % 3 === 0);

    Array.prototype.forEach(element => (callback(element) && newArray.push(element)));
    ```
    
    * reduce
     ```javascript
    const users = [
      { name: 'John', age: 34 },
      { name: 'Amy', age: 20 },
      { name: 'camperCat', age: 10 }
    ];
    
    const sumOfAges = users.reduce((sum, user) => sum + user.age, 0);
    console.log(sumOfAges); // 64
    ```   
    
    * includes
    ```javascript
    const array1 = [1, 2, 3];
    console.log(array1.includes(2));
  
    const destroyer = (arr, ...valsToRemove) => arr.filter(elem => !valsToRemove.includes(elem));
    ``` 
    
    * sort numeric array
    ```javascript
    numArray.sort((a, b) => a - b); // For ascending sort
    numArray.sort((a, b) => b - a); // For descending sort  
    ```
    
    
* Objects
    * for ... in
    ```javascript
    let result = 0;
    for (let user in usersObj) {
    if (usersObj[user].online === true) {
      result++;
      }
    }
    ```
    
    * `Object.keys(obj)`
    * `hasOwnProperty`

* String
    * `string.repeat(count)`
    * `string.endsWith(searchvalue, length)`
    * `string.slice(start, end)`

    * Reverse string
    ```javascript
    function reverseString(str) {
      return str
        .split("")
        .reverse()
        .join("");
    }
    ```
    
    * Longest word
    ```javascript
    function findLongestWordLength(str) {
      return Math.max(...str.split(" ").map(word => word.length));
    }
    ```
    
    * To Uppercase
    ```javascript
    function titleCase(str) {
      var convertToArray = str.toLowerCase().split(" ");
      var result = convertToArray.map(function(val) {
        return val.replace(val.charAt(0), val.charAt(0).toUpperCase());
      });
      return result.join(" ");
    }    
    ```
**Screenshots**
- [Intro-to-JavaScript-Udacity](task_js_basics/Intro-to-JavaScript-Udacity.png?raw=true)
- [JavaScript-freeCodeCamp](task_js_basics/Learn-to-code-at-home-freeCodeCamp-org.png?raw=true)

### 7. Document Object Model

#### DOM

**Element content**

* `$0` to get selected Element
*The .innerHTML property sets or returns the HTML content 
inside the selected element (i.e. between the tags).

* `textContent` and  `innerHTML`:

    If you'd like to update an element, including its HTML, 
    then you need to use the .innerHTML property:
```javascript
// doesn't work as expected
myElement.textContent = 'The <strong>Greatest</strong> Ice Cream Flavors'; 

// works as expected
myElement.innerHTML = 'The <strong>Greatest</strong> Ice Cream Flavors';  
```

**Add New Page Content**

* Add element - `.createElement()`, `.appendChild()`
```javascript
// create a brand new <span> element
const newSpan = document.createElement('span');
// select the first (main) heading of the page
const mainHeading = document.querySelector('h1');
// add the <span> element as the last child element of the main heading
mainHeading.appendChild(newSpan);
```

* Add paragraph with text
```javascript
const myPara = document.createElement('p');
myPara.textContent = 'I am the text for the paragraph!';
document.body.appendChild(myPara);
```

* `.insertAdjacentHTML()`
```html
<!-- beforebegin -->
<p>
    <!-- afterbegin -->
    Existing text/HTML content
    <!-- beforeend -->
</p>
<!-- afterend -->
```
```javascript
const mainHeading = document.querySelector('#main-heading');
const htmlTextToAdd = '<h2>Skydiving is fun!</h2>';
mainHeading.insertAdjacentHTML('afterend', htmlTextToAdd);
```

* Remove Page Content  
    `.removeChild()` and `.remove()`  
    Helpful properties - `.firstChild`, `.firstElementChild`, `.parentElement`
```javascript
const mainHeading = document.querySelector('h1');
mainHeading.parentElement.removeChild(mainHeading);
mainHeading.remove();
```

**Style Page Content**
```javascript
const mainHeading = document.querySelector('h1');
mainHeading.style.color = 'red';
mainHeading.style.cssText = 'color: blue; font-size: 3.5em';
mainHeading.setAttribute('style', 'color: blue; background-color: orange; font-size: 3.5em;');

const mainHeading = document.querySelector('#main-heading');
// store the list of classes in a variable
const listOfClasses = mainHeading.className;
const arrayOfClasses = listOfClasses.split(' ');
// or
// store the list of classes in a variable
const listOfClasses = mainHeading.classList;
```
The `.classList` property has a number of properties of its own. Some of the most popularly used ones are:

`.add()` - to add a class to the list
`.remove()` - to remove a class from the list
`.toggle()` - to add the class if it doesn't exists or remove it from the list if it does already exist
`.contains()` - returns a boolean based on if the class exists in the list or not

**Events**

EventTarget methods:
* `.addEventListener()`
* `.removeEventListener()`
* `.dispatchEvent()`

```javascript
const mainHeading = document.querySelector('h1');
mainHeading.addEventListener('click', function (event) {
  console.log('The heading was clicked!');
});
```
There are three different phases during the lifecycle of an event. They are:
* the capturing phase
* the at target phase
* the bubbling phase

`.preventDefault()` and Event Delegation
```javascript
const links = document.querySelectorAll('a');
const thirdLink = links[2];

thirdLink.addEventListener('click', function (event) {
    event.preventDefault();
    console.log("Look, ma! We didn't navigate to a new page!");
    console.log('A paragraph was clicked: ' + event.target.textContent);
    
    if (evt.target.nodeName === 'SPAN') {  // ← verifies target is desired element
        console.log('A span was clicked with text ' + evt.target.textContent);
    }
});
```

* `DOMContentLoaded` Event
```javascript
document.addEventListener('DOMContentLoaded', function () {
  document.querySelector('footer').style.backgroundColor = 'purple';
});
```

* Permormance
```javascript
const fragment = document.createDocumentFragment();  // ← uses a DocumentFragment instead of a <div>

for (let i = 0; i < 200; i++) {
    const newElement = document.createElement('p');
    newElement.innerText = 'This is paragraph number ' + i;

    fragment.appendChild(newElement);
}

document.body.appendChild(fragment); // reflow and repaint here -- once!
```
* In general, if you have to make a group of changes, hide/change all/show 
is a great pattern to use if the changes are relatively contained.
```javascript
// hide #comments
document.getElementById("comments").style.display = "none";
// delete spam comments
// show #comments
document.getElementById("comments").style.display = "block";
```

**Screenshots**
- [JavaScript-and-the-DOM-Udacity](task_js_dom/JavaScript-and-the-DOM-Udacity.png?raw=true)
- [freeCodeCamp](task_js_dom/Learn-to-code-at-home-freeCodeCamp-org.png?raw=true)
