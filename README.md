# HTML 

### Agenda

1. **Introduction**
2. **Extensions**
3. **Basics of HTML**:
      + Basic HTML Structure
4. **Essential HTML elements**:
      + Headings
      + Paragraphs
      + Links
      + Images
      + Teams
      + Forms
      + Tables
5. **Assignment**

---


### 1. Introduction

HTML stands for HyperText Markup Language. It's the standard markup language used to create and structure content on the web. HTML is the backbone of web pages and provides the structure for the content that appears on a website.

HTML documents are text-based and consist of a series of elements that organize and define the structure of a web page. Elements are represented by tags enclosed in angle brackets, like <tagname>. Each element can contain content and additional attributes that provide information about the element.

### 2. Extension

For this course, we are going to use “Live Server” Extension. The "Live Server" extension for Visual Studio Code is a popular tool that allows you to create a local development server and instantly see changes to your HTML, CSS, and JavaScript code in a web browser without manually refreshing the page.


![Alt text](https://i.postimg.cc/gJP5GyPc/hryj.jpg)



### 3. Basics of HTML

HTML documents are composed of:

+ Elements: Building blocks of HTML pages.
+ Tags: Define different parts of the content.
+ Attributes: Provide additional information about elements.
+ Comments Comments are used to add notes or descriptions within the code that are not visible to users when the page is rendered in a web browser.
We can pass comments in an HTML document in the following way :

```bash
<!-- It is a Comment  -->
```


Basic Structure of an HTML document:

```bash
<!DOCTYPE html>
<html>
<head>
<title>Page Title</title>
</head>
<body>
<!-- Content goes here -->
</body>
</html>

```



### 4. Essential HTML elements
                      
+ #### Headings
                              
HTML provides six levels of headings from `<h1>` to `<h6>`.

``` bash
<h1>This is a Heading 1</h1>
<h2>This is a Heading 2</h2>
<!-- ... -->
<h6>This is a Heading 6</h6>

```

+ #### Paragraphs

To create paragraphs:
``` bash
<p>This is a paragraph.</p>
<p>This is another paragraph.</p>
```


+ #### Links

Creating links using `<a>` tag:
```bash
<a href="https://example.com">Visit Example</a>
```

+ #### Images
Inserting images using `<img>` tag:
```bash
<img src="image.jpg" alt="Description of the image">
```


+ #### Lists
                           
Creating ordered and unordered lists:

```bash
<ul>
    <li>Item 1</li>
    <li>Item 2</li>
</ul>

<ol>
    <li>Item 1</li>
    <li>Item 2</li>
</ol>
```

+ #### Forms
                
Basic form structure using `<form>`, `<input>`, and `<button>`:
```bash
<form>
    <input type="text" placeholder="Enter your name">
    <button type="submit">Submit</button>
</form>
```

+ #### Tables

Creating tables with `<table>`, `<tr>`, `<td>`, and `<th>`:

```bash
<table>
    <tr>
        <th>Name</th>
        <th>Age</th>
    </tr>
    <tr>
        <td>John</td>
        <td>25</td>
    </tr>
</table>
```



### 5. Assignment

**Task 1**: Create a search bar, along with the placeholder given inside. 

Follow the Given steps to create the following in HTML:

**Step 1: Set Up the HTML File**
             
+ Open Visual Studio Code (VS Code).
+ Create a new HTML file:
     + Go to File -> New File or press Ctrl + N.
     + Save the file with an appropriate name and the .html extension (e.g., index.html).
     + Start with the basic structure: `<!DOCTYPE html>`, `<html>`, `<head>`, and `<body>` tags

```bash
<!DOCTYPE html>
<html>
<head>
<title>Page Title</title>
</head>
<body>
<!-- Content goes here -->
</body>
</html>

```







**Step 2: Add Meta Information**

+ Inside the `<head>` tag, include a `<meta>` tag to define the character encoding: `<meta charset="UTF-8">`.
+ Set the title of the page using the `<title>` tag: `<title>`Search Bar`</title>`.

```bash
<!DOCTYPE html>
<html>
<head>
<meta charset="UTF-8">
<title>Search Bar</title>
</head>
<body>
<!-- Content goes here -->
</body>
</html>

```



**Step 3: Create the Input Bar Structure and add SVG**

+ Inside the `<body>` tag, create a `<div>` element to contain the search bar.
+ Inside the `<div>`, add an <svg> element for the search icon
+ Use the viewBox attribute to set the coordinate system: viewBox="0 0 24 24".
+ Include a `<path>` element within the `<svg>` to define the shape of the search icon using the d attribute.

```bash
<!DOCTYPE html>
<html>
<head>
<meta charset="UTF-8">
<title>Search Bar</title>
</head>
<body>
  <div >
    <!-- SVG search icon -->
    <svg class="search-icon" width="20" height="20" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg">
      <path d="M15.5 14h-.79l-.28-.27a6.5 6.5 0 0 0 1.48-5.34c-.47-2.78-2.79-5-5.59-5.34a6.505 6.505 
      0 0 0-7.27 7.27c.34 2.8 2.56 5.12 5.34 5.59a6.5 6.5 0 0 0 5.34-1.48l.27.28v.79l4.25 4.25c.41.41
      1.08.41 1.49 0 .41-.41.41-1.08 0-1.49L15.5 14zm-6 0C7.01 14 5 11.99 5 9.5S7.01 5 9.5 5 14 7.01
      14 9.5 11.99 14 9.5 14z"/>
    </svg>
  </div>
</body>
</html>

```

  



**Step 4: Add the Input Field**

+ Within the `<div>`, add an `<input>` element:
    + Set the type to "text":type="text".
    + Include a placeholder attribute to display text in the input field when it's empty: placeholder="Search...".

```bash
<!DOCTYPE html>
<html>
<head>
<meta charset="UTF-8">
<title>Search Bar</title>
</head>
<body>
  <div >
    <!-- SVG search icon -->
    <svg class="search-icon" width="20" height="20" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg">
      <path d="M15.5 14h-.79l-.28-.27a6.5 6.5 0 0 0 1.48-5.34c-.47-2.78-2.79-5-5.59-5.34a6.505 6.505 
      0 0 0-7.27 7.27c.34 2.8 2.56 5.12 5.34 5.59a6.5 6.5 0 0 0 5.34-1.48l.27.28v.79l4.25 4.25c.41.41
      1.08.41 1.49 0 .41-.41.41-1.08 0-1.49L15.5 14zm-6 0C7.01 14 5 11.99 5 9.5S7.01 5 9.5 5 14 7.01
      14 9.5 11.99 14 9.5 14z"/>
    </svg>

    <!-- Input field -->
    <input type="text" placeholder="Search...">
  </div>
</body>
</html>

```
         


**Step 5: Run the Live Server**

+ Right-click anywhere in the HTML file.
+ Select "Open with Live Server" from the context menu.
+ Or click on “Go Live” in the right bottom corner of the VS code window.

![Alt text](https://i.postimg.cc/RFBHGhwb/arg.jpg)



**After all these steps the following output will be obtained:**

![Alt text](https://i.postimg.cc/MZ0wfTsr/asv.jpg)


 
                 


**Task 2**: Create a navbar

This task can be done with the help of lists and links and by following the same structure as in task 1. And the output would look like this:

![Alt text](https://i.postimg.cc/0yXBWFBZ/17.jpg)

**Task 3**: Create a dropdown for the avatar on the right corner of the navbar

This task can also be done with the help of `<select>` and `<option>` tags or lists and links and by following the same structure as in task 1.And the output would look like this: 

![Alt text](https://i.postimg.cc/vT87dH1n/18.jpg)


**Task 4**: Create a Registration form that takes input Name, Email, Gender, Country, and address and has a submit and a reset button

This task can also be done with the help of `<radio>`, `<select>`, `<option>`, and other related tags. 


## **Code Shared in class**


```html
<!-- Agenda:

- Basics Structure of HTML
- Anchor tag and image tag
- Lists
- Tables in HTML
- HTML5 tags -- Audio, Video Tags
- Semantic HTML
- Forms
- HTML5 API's -- Geolocation API, Canvas API
- Logical vs Physical Tags
- HTML entities
- Meta Tags
- DOM (Introduction) -->


<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Basic HTML Page</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    
<!-- Specificity -->

    <!-- <h1 class="demo">Hello, World!</h1>
    <p>This is a basic HTML page.</p>
    <div>
        <p>This is 2nd p tag.</p>
        <p id="p-tag">This is 3rd p tag.</p>
        
        <div>
            <p class="tag" id="tag">This is 3rd p tag.</p>
        </div>
        
    </div> -->

<!---------------------------------------------------------------->


<!-- Box Model -->

    <!-- <div id="demo2">
        <h1>Hello World</h1>
    </div>
     -->

<!---------------------------------------------------------------->

<!-- CSS Varaibles  -->

<!-- <div id="somediv">
    <h1>Hello World</h1>
</div> -->


<!---------------------------------------------------------------->

<!-- Calc -->
<!-- <div>
    <h2>This is calc representation</h2>
</div> -->

<!---------------------------------------------------------------->


<!-- Pseudo Selectors --><!-- Pseudo Elements --> <!-- Attr -->

<!-- <div>
    <h1>About Me</h1>
    <p>My name is <b>Yashswi Singh</b> and I am a developer</p>
    <input type="text">
    <div id="banner" my-data="wow">I am visible</div>

    <p>My favourite languages:
    
        <ul>
            <li>HTML</li>
            <li>CSS</li>
            <li>JavaScript</li>
            <li>React</li>
        </ul>
    </p>
    
</div> -->

<!---------------------------------------------------------------->




<!-- <h1>Heading 1</h1>
<p>This is a paragraph.</p>
<a href="https://www.youtube.com">This is a link</a>
<img src="image.jpg" alt="Description of image"> -->

<!---------------------------------------------------------------->


<!-- <ul>
    <li>Unordered List Item 1</li>
    <li>Unordered List Item 2</li>
</ul>

<ol>
    <li>Ordered List Item 1</li>
    <li>Ordered List Item 2</li>
</ol> -->

<!---------------------------------------------------------------->


<!-- <table>
    <tr>
        <th>Header 1</th>
        <th>Header 2</th>
    </tr>
    <tr>
        <td>Data 1</td>
        <td>Data 2</td>
    </tr>
</table> -->

<!---------------------------------------------------------------->


<!-- <form action="/submit" method="post">
    <label for="name">Name:</label>
    <input type="text" id="name" name="name"><br>
    
    <label for="email">Email:</label>
    <input type="email" id="email" name="email"><br>
    
    <input type="submit" value="Submit">
</form> -->

<!---------------------------------------------------------------->


<!-- <audio controls>
    <source src="path/to/audio.mp3" type="audio/mpeg">
    Your browser does not support the audio element.
</audio> -->

<!---------------------------------------------------------------->


<!-- <video width="320" height="240" controls>
    <source src="path/to/video.mp4" type="video/mp4">
    Your browser does not support the video tag.
</video> -->

<!---------------------------------------------------------------->


<!-- <header>
    <h1>Website Title</h1>
</header>
<nav>
    <ul>
        <li><a href="#home">Home</a></li>
        <li><a href="#about">About</a></li>
    </ul>
</nav>
<main>
    <article>
        <h2>Article Title</h2>
        <p>Article content...</p>
    </article>
</main>
<footer>
    <p>&copy; 2024 My Website</p>
</footer> -->

<!---------------------------------------------------------------->

<!-- <form action="/submit" method="post">
    <fieldset>
        <legend>Personal Information</legend>
        <label for="name">Name:</label>
        <input type="text" id="name" name="name"><br>
        
        <label for="email">Email:</label>
        <input type="email" id="email" name="email"><br>
        
        <label>Gender:</label>
        <input type="radio" id="male" name="gender" value="male">
        <label for="male">Male</label>
        <input type="radio" id="female" name="gender" value="female">
        <label for="female">Female</label><br>
        
        <label for="country">Country:</label>
        <select id="country" name="country">
            <option value="us">United States</option>
            <option value="ca">Canada</option>
        </select><br>
        
        <label for="message">Message:</label><br>
        <textarea id="message" name="message"></textarea><br>
        
        <input type="submit" value="Submit">
    </fieldset>
</form> -->


<!---------------------------------------------------------------->


<button onclick="getLocation()">Get Location</button>
<p id="location"></p>

<script>
function getLocation() {
    if (navigator.geolocation) {
        navigator.geolocation.getCurrentPosition(showPosition());
    } else {
        document.getElementById("location").innerHTML = "Geolocation is not supported by this browser.";
    }
}

function showPosition(position) {
    document.getElementById("location").innerHTML = "Latitude: " + position.coords.latitude +
    "<br>Longitude: " + position.coords.longitude;
}
</script>


<!---------------------------------------------------------------->


<!-- <canvas id="myCanvas" width="200" height="100" style="border:1px solid #000000;"></canvas>

<script>
var c = document.getElementById("myCanvas");
var ctx = c.getContext("2d");
ctx.fillStyle = "#FF0000";
ctx.fillRect(0, 0, 150, 75);
</script> -->

<!---------------------------------------------------------------->

<!-- <head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="A brief description of the page">
    <meta name="keywords" content="HTML, CSS, JavaScript">
    <meta name="author" content="John Doe">
    <meta http-equiv="refresh" content="30">
    <title>Meta Tags Example</title>
</head> -->


<!---------------------------------------------------------------->


<!-- <em>This text is emphasized</em>
<strong>This text is strong</strong>
<cite>This text is a citation</cite>
<abbr title="World Health Organization">WHO</abbr>



<i>This text is italic</i>
<b>This text is bold</b>
<u>This text is underlined</u>
<small>This text is smaller</small> -->


<!---------------------------------------------------------------->


<!-- <p>Less than: &lt;</p>
<p>Greater than: &gt;</p>
<p>Ampersand: &amp;</p>
<p>Quotation mark: &quot;</p>
<p>Apostrophe: &apos;</p>
<p>Non-breaking space: &nbsp;</p> -->


<!---------------------------------------------------------------->


<!-- <form action="/submit" method="post">
    <label for="name">Name:</label>
    <input type="text" id="name" name="name"><br>

    <label for="email">Email:</label>
    <input type="email" id="email" name="email"><br>

    <label for="password">Password:</label>
    <input type="password" id="password" name="password"><br>

    <label for="dob">Date of Birth:</label>
    <input type="date" id="dob" name="dob"><br>

    <label for="color">Favorite Color:</label>
    <input type="color" id="color" name="color"><br>

    <label for="file">Upload File:</label>
    <input type="file" id="file" name="file"><br>

    <label for="website">Website:</label>
    <input type="url" id="website" name="website"><br>

    <label for="quantity">Quantity:</label>
    <input type="number" id="quantity" name="quantity" min="1" max="10"><br>

    <label for="range">Range:</label>
    <input type="range" id="range" name="range" min="0" max="100"><br>

    <label for="gender">Gender:</label>
    <input type="radio" id="male" name="gender" value="male">
    <label for="male">Male</label>
    <input type="radio" id="female" name="gender" value="female">
    <label for="female">Female</label><br>

    <label for="hobbies">Hobbies:</label>
    <input type="checkbox" id="reading" name="hobbies" value="reading">
    <label for="reading">Reading</label>
    <input type="checkbox" id="traveling" name="hobbies" value="traveling">
    <label for="traveling">Traveling</label><br>

    <label for="country">Country:</label>
    <select id="country" name="country">
        <option value="us">United States</option>
        <option value="ca">Canada</option>
    </select><br>

    <label for="comments">Comments:</label><br>
    <textarea id="comments" name="comments"></textarea><br>

    <input type="submit" value="Submit">
</form>
 -->

<!---------------------------------------------------------------->

<!-- <iframe src="https://yashswisingh.vercel.app/" width="800" height="600" title="Iframe Example"></iframe> -->



</body>
</html>


```
