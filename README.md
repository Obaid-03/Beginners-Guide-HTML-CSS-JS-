# Beginners-Guide-HTML-CSS-JS-
Beginners Guide to HTML CSS and JavaScript to get started with web development

Introduction:

In today's digital age, having a basic understanding of web development has become essential. HTML, CSS, and JavaScript form the foundation of every website, allowing you to create and style web pages while adding interactive elements. This article aims to provide beginners with an overview of these three fundamental technologies and their roles in web development.

HTML: 

Building Blocks of a Web Page HTML (Hypertext Markup Language) is the backbone of every web page. It defines the structure and content of a webpage using various elements, such as headings, paragraphs, images, links, and lists. Here are some key points to understand:

Basic HTML structure: The essential elements like <html>, <head>, and <body>.

Tags and attributes: How to use tags like <h1>, <p>, <img>, and attributes like src, alt, and href.

Semantic elements: Introduction to semantic tags like <header>, <nav>, <section>, and their significance in structuring content.

Creating forms: Understanding form elements like <input>, <select>, <textarea>, and their attributes for user input.

CSS:

 Styling Your Web Pages CSS (Cascading Style Sheets) is responsible for the visual presentation and layout of web pages. It allows you to customize the colors, fonts, spacing, and positioning of HTML elements. Here's what beginners should know:

Selectors and declarations: How to target HTML elements using selectors and define styling properties in declarations.

Inline, internal, and external stylesheets: Different ways to include CSS styles in your web page.

Basic styling: Changing colors, fonts, backgrounds, margins, and padding of elements.

Layout and positioning: Introduction to CSS box model, float, flexbox, and grid for controlling the layout of web pages.

Responsive design: Designing websites that adapt to different screen sizes using media queries.

JavaScript:

 Adding Interactivity and Functionality JavaScript is a programming language that brings life to web pages by adding interactivity and dynamic functionality. Here are some essential concepts to grasp:

Basics of JavaScript: Variables, data types, operators, conditionals, loops, and functions.

DOM manipulation: How to access and modify HTML elements using JavaScript to create dynamic effects.

Event handling: Responding to user interactions like clicks, mouse movements, and form submissions.

Fetching data: Making AJAX requests to retrieve data from servers without refreshing the entire page.

Introduction to frameworks and libraries: Mentioning popular JavaScript frameworks like React, Angular, and libraries like jQuery.

In this article, we will focus on the basic concepts to get started.

Implementation 

Here are the simple steps to get started:

  Install VScode

Create a file named index.html in a new directory.

Open the file in VScode and write the boilerplate. I picked it from http://htmlshell.com/ or you can also type ! and enter to get an instant boilerplate.

Congratulations now you can start coding…

It will look like this. 

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Document</title>
</head>
<body>
  
</body>
</html>

I have added heading and paragraph tags, now we can see what happens to our webpage to do so we have double click on the HTML file it will open in browser.

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Document</title>
</head>
<body>
  
<h1>Welcome Beginners</h1>
<p>Click the button to toggle the visibility of the paragraph below:</p>

</body>
</html>

our webpage will look like this: 

Now to add some functionality we will use a couple of more tags and assign them id and class

<body>
  
  <h1>Welcome Beginners</h1>
  <p>Click the button to toggle the visibility of the paragraph below:</p>
  <button id="myButton">Toggle</button>
  <p id="myParagraph" class="hidden">This paragraph is initially hidden.</p>
  

</body>

The id and class inside tags are used as a selector to style and perform some functionality. We will use them in our next few steps.

Webpage looks like this:

 Putting code inside a div helps in various functions such as applying a background colour to all the elements inside a div .

 <div class="container">
    <h1>Welcome Beginners</h1>
    <p>Click the button to toggle the visibility of the paragraph below:</p>
    <button id="myButton">Toggle</button>
    <p id="myParagraph" class="hidden">This paragraph is initially hidden.</p>
    
  </div>

Now to make it look decent we will add some styles to do so firstly we will add the styles tag inside head tag.

<style>
    /* CSS styles */
    body {
      font-family: Arial, sans-serif;
      background-color: #f2f2f2;
      margin: 0;
      padding: 0;
    }

    .container {
      max-width: 800px;
      margin: 0 auto;
      padding: 20px;
      background-color: #fff;
      box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
    }

    h1 {
      color: #333;
      text-align: center;
    }

    p {
      color: #666;
    }

    #myButton {
      display: block;
      width: 120px;
      height: 40px;
      margin: 20px auto;
      background-color: #4CAF50;
      color: #fff;
      font-size: 16px;
      text-align: center;
      line-height: 40px;
      cursor: pointer;
      border-radius: 4px;
      text-decoration: none;
    }

    .hidden {
      display: none;
    }

   
  </style>

Here is the explanation: 

body: This selector targets the <body> element of the HTML document. The styles applied include setting the font family to Arial or a fallback sans-serif font, setting the background color to a light gray (#f2f2f2), and removing any default margin and padding on the body element.

.container: This selector targets an element with a class of "container". It is commonly used to wrap a section of content. The styles applied include setting a maximum width of 800 pixels, centring the container horizontally with  margin: 0 auto, adding some padding, setting a white background color, and applying a box shadow for a subtle shadow effect.

h1: This selector targets <h1> heading elements. The styles applied include setting the color to a dark gray (#333) and center-aligning the text.

p: This selector targets <p> paragraph elements. The styles applied include setting the color to a medium gray (#666).

#myButton: This selector targets an element with an id attribute of "myButton". It is typically used for styling a specific button element. The styles applied include setting the display to block (which makes it take up the full width available), setting a specific width and height, centering the button horizontally with margin: 20px auto, setting a background color of a green shade (#4CAF50), setting the text color to white, defining a font size, center-aligning the text vertically and horizontally with line-height and text-align, setting the cursor to a pointer when hovering over the button, applying a border radius to give rounded corners, and removing the default text decoration (underlining).

.hidden: This selector targets elements with a class of "hidden". It is typically used to hide elements from being displayed on the webpage. The style applied is  display: none, which completely hides the element.

In summary, the provided CSS styles set the overall styling of the webpage, including the body background color, container layout, heading and paragraph text styles, button appearance, and the hidden class for hiding elements. These styles create a visually appealing and well-structured webpage.

Now Our Webpage looks nice

Now when the button is clicked, the code toggles the visibility of a paragraph element. If it is hidden, clicking the button will make it visible and change the button text to "Hide". If it is visible, clicking the button will hide it again and change the button text to "Toggle". This provides a simple mechanism to show or hide content on a webpage.

To do so here is the code:

<body>
  
  <h1>Welcome Beginners</h1>
  <p>Click the button to toggle the visibility of the paragraph below:</p>
  <button id="myButton">Toggle</button>
  <p id="myParagraph" class="hidden">This paragraph is initially hidden.</p>
  <p>Move your mouse over this paragraph to see it highlighted.</p>



<script>
   var button = document.getElementById('myButton');
    var paragraph = document.getElementById('myParagraph');

    button.addEventListener('click', function() {
      if (paragraph.classList.contains('hidden')) {
        paragraph.classList.remove('hidden');
        button.textContent = 'Hide';
      } else {
        paragraph.classList.add('hidden');
        button.textContent = 'Toggle';
      }
    });
</script>
</body>

Inside the script tag, we can write our Javascript code. 

The code adds an event listener to a button element using JavaScript. The event listener listens for a “click” event on the button. When the button is clicked, the function inside the event listener is executed.  Within the function, there is a conditional statement that checks if a paragraph element has a CSS class of "hidden". This CSS class is typically used to hide an element from being visible on the webpage. 

 If the paragraph element has the "hidden" class, it means that it is currently hidden. In this case, the function removes the "hidden" class from the paragraph element using the classList.remove() method. This makes the paragraph element visible on the webpage. Additionally, the text content of the button is changed to "Hide" to reflect the action. 

 On the other hand, if the paragraph element does not have the "hidden" class, it means that it is currently visible. In this case, the function adds the "hidden" class to the paragraph element using the classList.add() method. This hides the paragraph element on the webpage. The text content of the button is then changed to "Toggle" to reflect the action.

After clicking the button our webpage will look like this:

Complete Code: 

<!DOCTYPE html>
<html>
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Beginners Guide</title>

  
  <style>
    /* CSS styles */
    body {
      font-family: Arial, sans-serif;
      background-color: #f2f2f2;
      margin: 0;
      padding: 0;
    }

    .container {
      max-width: 800px;
      margin: 0 auto;
      padding: 20px;
      background-color: #fff;
      box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
    }

    h1 {
      color: #333;
      text-align: center;
    }

    p {
      color: #666;
    }

    #myButton {
      display: block;
      width: 120px;
      height: 40px;
      margin: 20px auto;
      background-color: #4CAF50;
      color: #fff;
      font-size: 16px;
      text-align: center;
      line-height: 40px;
      cursor: pointer;
      border-radius: 4px;
      text-decoration: none;
    }

    .hidden {
      display: none;
    }

   
  </style>
</head>
<body>
  <div class="container">
    <h1>Welcome Beginners</h1>
    <p>Click the button to toggle the visibility of the paragraph below:</p>
    <button id="myButton">Toggle</button>
    <p id="myParagraph" class="hidden">This paragraph is initially hidden.</p>
    
  </div>

  <script>
    // JavaScript code
    var button = document.getElementById('myButton');
    var paragraph = document.getElementById('myParagraph');

    button.addEventListener('click', function() {
      if (paragraph.classList.contains('hidden')) {
        paragraph.classList.remove('hidden');
        button.textContent = 'Hide';
      } else {
        paragraph.classList.add('hidden');
        button.textContent = 'Toggle';
      }
    });

  
  </script>
</body>
</html>


Here is the link to the GitHub repository: 

Conclusion: 

HTML, CSS, and JavaScript are the building blocks of modern web development. HTML provides the structure and content, CSS adds styling and layout, while JavaScript adds interactivity and functionality. By mastering these technologies, beginners can create dynamic and visually appealing websites. Remember to practice and experiment with different concepts to enhance your skills further. Good luck on your web development journey!
