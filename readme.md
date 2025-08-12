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

- but did u see that we put all in ```<td>``` and got same result 
-   even our heading looks same as our content in the table (items,price,colour,benefits)
- also looks same but to make it like as heading put```<th>``` instead of ```<td>```
- only put headings in ```<th>``` eg.
```
  <table>
            <tr>
                <th>item</th>
                <th>price</th>
                <th>colour</th>
                <th>benefits</th>
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
    
    
</body>
</html>
```
- her we got this in result...
**item**	       **price**	**colour**	 **benefits**
black chocolate	$2.12	     black	      instant energy
cold cofee	      $1.34	     grey	       keep mind focus
green tea	      $0.98	     transparent	 reduces cholestrol

- did u see we got heading in bold letters due to ```<th>``` so from now on when we have to make heading rows in table we use ```<th>``` and for normal rows we use ```<td>```

- also put table heading in ```<thead>``` just like we put ```<head>``` in simple html code
- it cant do anything but just to easy to understand the code to coder and made code stylish and to style in css and perfect code structure eg.  
```
<table>
 <thead>
            <tr>
                <th>item</th>
                <th>price</th>
                <th>colour</th>
                <th>benefits</th>
            </tr>
            </thead>
```
- and thead should be placed inside table

- and put table body i mean(table rows) inside ```<tbody>```this also cant do anything but easy for coders to understand and for perfect code structure eg. 
```
</tbody>
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
            </tbody>
        </table>
```
## semantic markup
** semantic elements all work like ```<div>``` but give meaning to the code eg this part of code is what part of code **

- semantic elements cant do anything new but provide meaning to our code(content)
- eg. we can put div but if we put main in place of div coder can understand eassily that this is the main part of the body also screen reader can know this is the main part of the body like i will give u example.
```
 <div>
            <p>Lorem, ipsum dolor sit amet consectetur adipisicing elit. Et delectus voluptatem labore commodi. Aliquam, aliquid similique. Non libero minus, nostrum labore explicabo dolore quod vero beatae, facilis, fugit mollitia earum!</p>
        </div>
```
- lets assume this is our main body in the code.
- we write code here with div and div make it seperate and when we have a very big code 
- and we fill it div coder and screen reader(inspect) got confuse what part is this
- like in the below pic

   ![example of ```<main>``` tag](images/main.png)

   - but if we write this same code with ```<main>``` tag
   - nothing gonna change main did same as div (seperates it) but 
   - when any other coder or screen reader(inspect) checks it
   - he says ohhh this is main body of the page.. eg..
```   
 <main>
            <p>Lorem, ipsum dolor sit amet consectetur adipisicing elit. Et delectus voluptatem labore commodi. Aliquam, aliquid similique. Non libero minus, nostrum labore explicabo dolore quod vero beatae, facilis, fugit mollitia earum!</p>
 </main>
```
 ![main_final_result_example](images/main_final_result.png)


- same as ```<header>``` cant do anything same as ```<div>``` but told screen reader this is the heading
```
<h1>lorem episum</h1>
        <header>lorem episum story</header>

```
- same as ```<footer>``` can do anything same as div but told the screen reader this is footer ( in footer we wrote mainly the contact detalis and other thing like feedback etc etc)
- hey we can write anything in this but mainly foot of the webpage to ease the coder that this is foot of the page. 
```
 <footer>copyright no one 2025</footer>
```
- same as ```<nav>``` do nothing same as div but tell us this part is navigation part
- navigation(means this part contains links to another page) easy for coder or screen reader(inspect) eg. 
```
<nav>
            <ul>
                <li><a href="https://google.com">google</a></li>
                <li><a href="https://facebook.com">facebook</a></li>
            </ul>
        </nav>
```
- dont do anything here just tell this part is navigation part(contain links to another page).

- same as ```<aside>``` aside (means something thats tells coder or screen reader little bit about main content of the page) works same as div we know that .

- same as ```<time>``` tells coder or screen reader that in this part we put info. about time releated. eg.
![time_concept](images/time.png)

- same as ```<summary>``` tells coder or screen reader that part contains summary

* in short sematic elements tells coder or screen reader wha this part contains *


## chapter 6 basic css

# inline style
- basically in inline style we can style only one thing it can be anything paragraph div etc etc mens in that line we put that style (in the line we put attributioj style and then we can style that one particular thing) eg.

```
    <h1 style="color: brown;">THE LEGENDARY AK-47</h1>
    <p style="color:gold;">
        The <a href="https://www.istockphoto.com/photos/ak-47">AK-47</a>, officially known as the Avtomat Kalashnikova, is one of the most iconic and widely used assault rifles in the world. It was developed in the <a href="https://en.wikipedia.org/wiki/Soviet_Union">Soviet Union</a> by  <a href="https://www.gettyimages.in/photos/mikhail-kalashnikov">Mikhail Kalashnikov</a> and officially adopted by the Red Army in 1949. Renowned for its durability, simplicity, and low production cost, the AK-47 has become a symbol of both military power and revolutionary struggle. Its gas-operated, 7.62×39mm cartridge system allows it to function reliably in harsh conditions, including mud, sand, and extreme temperatures.The rifle can be operated with minimal training, which has made it especially popular among irregular forces and guerrilla fighters. Over 100 million units of the AK-47 and its variants have been produced, making it the most widely manufactured assault rifle in history. Its influence extends beyond military use; it appears on flags, national emblems, and even currency in some countries. Despite being over 75 years old, it continues to see active service in conflicts across the globe. Critics argue that its widespread availability has fueled violence and instability in many regions. Nonetheless, its reputation for reliability and ruggedness is unmatched. Several countries have produced their own licensed or unlicensed versions. The AK-47 has inspired countless other firearms, influencing modern weapon design. Its distinct curved magazine and rugged construction make it instantly recognizable. It’s not just a weapon but a part of global history. Whether viewed as a tool of liberation or destruction, the AK-47 remains one of the most influential firearms ever made.
    </p>
      <b> TONY STARK THE LEGEND</b>
    <div style="color: orange;">
        <a href="https://en.wikipedia.org/wiki/Tony_Stark_(Marvel_Cinematic_Universe)">Tony Stark</a>, also known as Iron Man, is a genius billionaire, inventor, and superhero from the Marvel Universe. He is the owner of Stark Industries, a powerful tech company known for its advanced weaponry and innovations. After being captured and injured, he builds the first Iron Man suit to escape, which sparks his journey as a hero. Stark is known for his intelligence, charm, and sarcastic wit. Despite his flaws, he often puts others before himself and fights to protect the world. He is a founding member of the Avengers, playing a key role in many battles. Over time, Tony grows from a selfish playboy into a selfless hero. His ultimate sacrifice in  <a style="color: black;" href="https://en.wikipedia.org/wiki/Avengers:_Endgame">"Avengers: Endgame"</a> saved the universe, solidifying his legacy.
    </div>
    <main style="color: green;">
        Tony Stark's relationship with the AK-47 is indirect but significant in the story of his transformation into Iron Man. In the <a style="color: chocolate;" href="https://en.wikipedia.org/wiki/Iron_Man_(2008_film)">2008 Iron Man film</a>, Stark is captured by a terrorist group called the Ten Rings, who are armed with various weapons — including AK-47 assault rifles. These weapons, along with other advanced arms, were surprisingly traced back to Stark Industries. This shocking discovery makes Tony realize that his inventions are being used for destruction instead of protection. The AK-47, a symbol of global conflict and terrorism, becomes a powerful reminder for Tony of the damage caused by irresponsible weapons distribution. This experience deeply affects him and marks a turning point in his life. After escaping captivity, he shuts down Stark Industries' weapons division. Instead, he focuses on building technologies to protect people, like the Iron Man suits. The presence of the AK-47 and similar weapons serves as a catalyst for his moral awakening. It ultimately drives his transformation from a weapons dealer to a superhero.
    </main>
    <footer style="color: darkolivegreen;">so that was the story of relation of ak 47 with tony Stark</footer>
```
result ![inline_result](images/inlinestyle.png)
- i put style attribution everywhere in links in paragraphs and in main in div in footler we can put it in everywhere (style attribute) how to put it put style like a attribute and in two commas write what u want border, width, font, color, eg. we put color her i show u how to put color with colon and then ehat type of colour u want put that in semicolon  (color:gree;)  style="color:"

- and what we do if we have a 100's of paragraphs,divs,mains,etc etc and want all style at once for that we use
```<style>
p{color:red;}     (in place of p we can write anything like div, main,h1, h2, heading,footler etc etc) like i write in code down below  (div) 
</style>
```
- that means in style tag we use "p" means paragraph that tells browser style all paragraphs. 
```
<h1 style="color: brown;">THE LEGENDARY AK-47</h1>
    <style>
        div{
            color: rosybrown;
        }
    </style>
    <div>
        The <a href="https://www.istockphoto.com/photos/ak-47">AK-47</a>, officially known as the Avtomat Kalashnikova, is one of the most iconic and widely used assault rifles in the world. It was developed in the <a href="https://en.wikipedia.org/wiki/Soviet_Union">Soviet Union</a> by  <a href="https://www.gettyimages.in/photos/mikhail-kalashnikov">Mikhail Kalashnikov</a> and officially adopted by the Red Army in 1949. Renowned for its durability, simplicity, and low production cost, the AK-47 has become a symbol of both military power and revolutionary struggle. Its gas-operated, 7.62×39mm cartridge system allows it to function reliably in harsh conditions, including mud, sand, and extreme temperatures.The rifle can be operated with minimal training, which has made it especially popular among irregular forces and guerrilla fighters. Over 100 million units of the AK-47 and its variants have been produced, making it the most widely manufactured assault rifle in history. Its influence extends beyond military use; it appears on flags, national emblems, and even currency in some countries. Despite being over 75 years old, it continues to see active service in conflicts across the globe. Critics argue that its widespread availability has fueled violence and instability in many regions. Nonetheless, its reputation for reliability and ruggedness is unmatched. Several countries have produced their own licensed or unlicensed versions. The AK-47 has inspired countless other firearms, influencing modern weapon design. Its distinct curved magazine and rugged construction make it instantly recognizable. It’s not just a weapon but a part of global history. Whether viewed as a tool of liberation or destruction, the AK-47 remains one of the most influential firearms ever made.
        </div>
    </p>
      <b> TONY STARK THE LEGEND</b>
    <div>
        <a href="https://en.wikipedia.org/wiki/Tony_Stark_(Marvel_Cinematic_Universe)">Tony Stark</a>, also known as Iron Man, is a genius billionaire, inventor, and superhero from the Marvel Universe. He is the owner of Stark Industries, a powerful tech company known for its advanced weaponry and innovations. After being captured and injured, he builds the first Iron Man suit to escape, which sparks his journey as a hero. Stark is known for his intelligence, charm, and sarcastic wit. Despite his flaws, he often puts others before himself and fights to protect the world. He is a founding member of the Avengers, playing a key role in many battles. Over time, Tony grows from a selfish playboy into a selfless hero. His ultimate sacrifice in  <a style="color: black;" href="https://en.wikipedia.org/wiki/Avengers:_Endgame">"Avengers: Endgame"</a> saved the universe, solidifying his legacy.
    </div>
    <main style="color: green;">
        Tony Stark's relationship with the AK-47 is indirect but significant in the story of his transformation into Iron Man. In the <a style="color: chocolate;" href="https://en.wikipedia.org/wiki/Iron_Man_(2008_film)">2008 Iron Man film</a>, Stark is captured by a terrorist group called the Ten Rings, who are armed with various weapons — including AK-47 assault rifles. These weapons, along with other advanced arms, were surprisingly traced back to Stark Industries. This shocking discovery makes Tony realize that his inventions are being used for destruction instead of protection. The AK-47, a symbol of global conflict and terrorism, becomes a powerful reminder for Tony of the damage caused by irresponsible weapons distribution. This experience deeply affects him and marks a turning point in his life. After escaping captivity, he shuts down Stark Industries' weapons division. Instead, he focuses on building technologies to protect people, like the Iron Man suits. The presence of the AK-47 and similar weapons serves as a catalyst for his moral awakening. It ultimately drives his transformation from a weapons dealer to a superhero.
    </main>
    <footer style="color: darkolivegreen;">so that was the story of relation of ak 47 with tony Stark</footer>
    <div>
        Wanda Maximoff, also known as Scarlet Witch, is a powerful member of the Avengers.
She possesses extraordinary abilities, including telekinesis, telepathy, and reality manipulation.
Originally introduced as a reluctant ally, Wanda later became a trusted hero.
Her powers are fueled by strong emotions, making her one of the most formidable Avengers.
She shares a deep bond with Vision, which shapes many of her choices.
Wanda’s journey is filled with loss, sacrifice, and personal growth.
Despite her struggles, she continues to fight for what she believes is right.
    </div>
    <div>
        Captain America, whose real name is Steve Rogers, is one of the most respected Avengers.
Originally a frail young man, he became a super-soldier through the Super Soldier Serum.
He is known for his unshakable sense of justice, courage, and leadership.
Armed with his iconic vibranium shield, he defends the world against evil.
Steve always puts the safety of others before his own life.
His moral compass makes him a symbol of hope and integrity.
Even when times are dark, Captain America inspires people to stand strong.
    </div>
```

# external styles
 - external styles means write css in another file and then link it with html we can link that css with thousand of html files at once through link tag (link is self closing tag ```<link   />```) self closing.
 ```<link />
 eg. we wrote css in chapter6.css file eg.
 ``` div {
    color: green;
    font-size:30px;
 }
 ```
 - then i can link this css file with unlimited html file take here our own file 
 in html file i wrote ```<link href="chapter6.css" rel="stylesheet"/>``` if css file is in another folder then we have to metion that here we make in same folder so only write direct name of css file and to join two file u need to put one more attribution in link tag called (rel) write style sheet with rel ....

## anatomy of css
- ist we select something put curly braces{}
and put property in curly braceswith colon and which property in semicolon eg.
```
p{
    color:black;
    font-size: 30px;
    diaplay:flex;  (etc etc,,,,)
}
```
## css selesctors
- selesctors are what we select to style eg.
```
P{
    color:red;
}
```
here selector is p means paragraph
  # element selector
  ** 
  element selctors are simple selectors in css like their name eg
  p, div, h1,h2,main,footler,body,a,like we litreally have to write their names 
  to select that thing to style 
  **
  *
  those simple selectors where we only have to write their name to select for style are called element selectors eg. below 
  *
  ```
p{
    color: greenyellow;
    font-size:20px;
}
a{
    color:grey;
    font-size:25px;
}
div{
    font-size: x-large;
    color: coral;
}
h1{
    font-size: xx-large;
    color: black;
}
h2{
    font-size: 30px;
    color: aqua;
}

  ```
  ## the world of css

  # the background-color
  - when we have to change the background color of anything like body,h1,h2,p,
  - div,main,a, etc etc... we just write in them eg in div
  ```
  div{
    background-color: olive;
  }
```



