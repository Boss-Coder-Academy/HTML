# Assignment: HTML 

## HTML

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

+ #### Comments

Comments are used to add notes or descriptions within the code that are not visible to users when the page is rendered in a web browser.
We can pass comments in an HTML document in the following way :

```bash
<!-- It is a Comment  -->
```


### 5. Assignment

**Task 1**: Create a search bar, along with the placeholder given inside. 

Follow the Given steps to create the following in HTML:

**Step 1: Set Up the HTML File**
             
+ Open Visual Studio Code (VS Code).
+ Create a new HTML file:
     + Go to File -> New File or press Ctrl + N.
     + Save the file with an appropriate name and the .html extension (e.g., index.html).
     + Start with the basic structure: <!DOCTYPE html>, <html>, <head>, and <body> tags

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

+ Inside the <head> tag, include a <meta> tag to define the character encoding: <meta charset="UTF-8">.
+ Set the title of the page using the <title> tag: <title>Search Bar </title>.

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

+ Inside the <body> tag, create a <div> element to contain the search bar.
+ Inside the <div>, add an <svg> element for the search icon
+ Use the viewBox attribute to set the coordinate system: viewBox="0 0 24 24".
+ Include a <path> element within the <svg> to define the shape of the search icon using the d attribute.

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

+ Within the <div>, add an <input> element:
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




**After all these steps the following output will be obtained:**

![Alt text](https://i.postimg.cc/MZ0wfTsr/asv.jpg)


 
                 


**Task 2**: Create a navbar

This task can be done with the help of lists and links and by following the same structure as in task 1. 

**Task 3**: Create a dropdown for the avatar on the right corner of the navbar

This task can also be done with the help of <select> and <option> tags or lists and links and by following the same structure as in task 1. 


