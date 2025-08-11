# Fresh Pasta Exercise

This is a simple HTML project that demonstrates a recipe page for making fresh pasta.  
It is created as part of a beginner HTML learning exercise, with no CSS styling applied.

## Project Structure

- **index.html** – The main HTML page containing the recipe content.
- **images/** – Folder containing images used in the recipe.

## Features

- Basic HTML tags (headings, paragraphs, lists, images).
- Recipe instructions for making fresh pasta.
- Semantic HTML structure for better readability.

## How to Open

1. Download the project files.
2. Open `index.html` in any web browser.

## Purpose

This project is made for learning HTML only — **no CSS** is used so that the focus remains on HTML elements and structure.

# Chapter 4 – Working With Forms

This chapter has 7 topics and 1 exercise.

## Topic 1 – Creating Text Input & Buttons

1. This is simple using HTML tags. For example, if I have to create a text input:

```<input type="text"> ```
REMEMBER: The input tag does not have a closing tag.

This code makes a simple rectangle where we can put text.

And then I learned about making buttons using the <button> tag:

text
```<button>Press Me</button>```
This makes a button named Press Me.

AND SIR GAVE US THIS TAG FOR BUTTONS:

text
```<button type="button">Press Me</button>```
But lastly, he told us we don’t need to write the (type) attribute in the button tag — it’s not important.

Topic 2 – The Form Element
We learned about the form element. The form element sends our data somewhere.
Example:

text
```<form>```
   ```<input type="text">```
   ```<button>Send</button>```
```</form>```
Here, it makes an input text box and a button inside the form element, meaning when we press the button, the form element sends our data (which we put in the input text box).

BUT WHERE DOES IT SEND OUR DATA?

We read about one attribute of the form element called (action):

text
```<form action="login">```
   ```<input type="text">```
   ```<button>Send</button>```
```</form>```
Here, the action attribute in the form element tells the form where to send data. For example, if we have a login page in the backend, we can set the action to "login", and the form will send data to the login page.

We can put anything in the action attribute, e.g.:

text
```<form action="https://google.com">```
   ```<input type="text">```
   ```<button>Search</button>```
```</form>```
Here, the action tells the form element to send data to Google.com.

And sir told us about method="get" which specifies how to send data — but he said we would learn it later.

## Topic 3 – Name and Placeholder Attributes

In the input tag, putting the name attribute gives a name to the value you enter:

text
```<form action="https://google.com">```
   ```<input name="username">```
   ```<button>Send</button>```
```</form>```
When the user puts data in the text input and presses the button, the browser will redirect to Google with the query parameter like:
google.com/?username=(what you typed)

Placeholder Attribute

It’s like a visual hint inside the input box. When you start typing, it disappears.

text
```<input placeholder="First Name">```
Here, “First Name” is shown until you type something.

Note: Attributes like (type), (name), (placeholder) should be written in the input element.

Topic 4 – Label
The ```<label>``` tag is used to give a label to a text input box.

text
```<label>Type Name</label>```
```<input type="text">```
This shows a text input box with the label Type Name, but clicking the label does nothing.

To make the label clickable:

text
```<label for="name">Type Name</label>```
```<input id="name" type="text">```
Now, when you click the label, the cursor automatically goes to the text box with the matching id.

## Topic 5 – Different Types of Inputs
There are many types of inputs:

type="number" (only numbers)

type="password" (hides characters)

type="color" (color picker)

type="date" (date picker)

type="email" (requires a valid email format)

required forces the field to be filled before submission — added directly to ```<input>```.

Topic 6 – Checkbox, Textareas, and Range Inputs
Textarea – Multi-line text box.

text
```<textarea></textarea>```
Range – A slider.

text
```<input type="range" min="0" max="10" step="1">```
min, max, and step control slider limits.

Checkbox

text
```<input type="checkbox" id="check">```
```<label for="check">Check Me</label>```
Clicking the label toggles the checkbox.

Topic 7 – Select and Radio Button
Select Dropdown

text
```<select name="options">```
   ```<option value="opt1">Option 1</option>```
   ```<option value="opt2">Option 2</option>```
   ```<option value="opt3">Option 3</option>```
```</select>```
The value in each ```<option>``` is what gets sent when the form is submitted.

Radio Buttons

text
```<input type="radio" name="choice" value="A">```
```<input type="radio" name="choice" value="B"> ```
Radio buttons allow selecting only one option per name group.

## chapter 5 other elements

## topic one ```<spans>```
- spans are generic inline elements. they have no special
- meaning but can be use later in styling in css.
- like i give u example
``` <p>hey i love my <span>cats </span> and i love my cars</p>```
    - here i put cats in between span and if u run the code nothing 
    - is gonna happen but when we enter in css we can change colour, style ,etc etc 
    - of the thing which is between in span.

## topic 2 ```<div>```
- A div can be used to group some things together, e.g.,
```<div>```
```<p>Hey, I love my <span>cats</span> and I love my cars</p>```
```<h1>Come learn HTML and CSS with us</h1>```
```<h2>Let's start with elements</h2>```
```<p>Hello, we are all going to read about elements now in HTML, and```
```after that, we will also learn CSS.</p>```
```</div>```

** Here, we wrote a heading and a paragraph and closed all of them inside a div element. When we run the code, we see the headings and paragraphs, but when we learn CSS, we can style that part alone. For example, we can put the code in a div and then style this part separately in CSS. We can style this entire section of code all at once. **

## topic 3 ```<table>```
- table is the element use use to make the tables
in table element we have to put ```<tr>``` element which tells table element that i am making rows in table now
- then to make rows we have to put ```<td>``` element eg.
```
        <table>
            <tr>
                <td>item</td>
                <td>price</td>
                <td>colour</td>
                <td>benefits</td>
            </tr>
            <tr>
                <td>black chocolate</td>
                <td>$2.12</td>
                <td>black</td>
                <td>instant energy</td>
            </tr>
            <tr>
                <td>cold cofee</td>
                <td>$1.34</td>
                <td>grey</td>
                <td>keep mind focus</td>
            </tr>
            <tr>
                <td>green tea</td>
                <td>$0.98</td>
                <td>transparent</td>
                <td>reduces cholestrol</td>
            </tr>
        </table>
```
- we get this result....
        item	   price	 colour	     benefits
black chocolate  $2.12   black	      instant energy
cold cofee	    $1.34 	 grey	        keep mind focus
green tea	     $0.98	 transparent	reduces cholestrol

## 
        
        