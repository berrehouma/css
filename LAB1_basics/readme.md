Objective:

By the end of this lab, students will be able to:

    1- Understand and apply basic CSS selectors.

    2- Differentiate between inline, internal, and external CSS.

    3- Understand the CSS box model.

    4- Apply basic CSS properties to common HTML elements.

    5- Create a simple webpage using the concepts learned.

Part 1: Basic Steps
Step 1: Setting Up the HTML File

    1- Create a new folder on your computer named CSS-Lab.

    2- Inside the folder, create a new file named index.html.

    3- copy the  index.html in a text editor (e.g., VS Code, Sublime Text).

Step 2: Inline CSS

    1- In the index.html file, add inline CSS to style the <h1> element: 
       <h1 style="color: blue; text-align: center;">Welcome to the CSS Lab!</h1>
    2- Save the file and open it in a browser to see the changes.

Step 3: Internal CSS

    1- Remove the inline CSS from the <h1> element.

    2- Add a <style> block in the <head> section of the HTML file:
        <head>
            <meta charset="UTF-8">
            <meta name="viewport" content="width=device-width, initial-scale=1.0">
            <title>CSS Lab</title>
            <style>
                h1 {
                    color: blue;
                    text-align: center;
                }
                p {
                    font-family: Arial, sans-serif;
                    font-size: 16px;
                    color: green;
                }
            </style>
        </head>

    3- Save the file and refresh the browser to see the changes.   

Step 4: External CSS

    1- Create a new file in the CSS-Lab folder named styles.css.

    2- Move the CSS rules from the <style> block in index.html to styles.css:  
        /* styles.css */
                h1 {
                    color: blue;
                    text-align: center;
                }

                p {
                    font-family: Arial, sans-serif;
                    font-size: 16px;
                    color: green;
                }
    3- Link the external CSS file to the HTML file by adding the following line in the <head> section of index.html:
       <link rel="stylesheet" href="styles.css">
    4- Save both files and refresh the browser to ensure the styles are applied.

Step 5: CSS Selectors

    1- Add more HTML elements to index.html:

         <div class="container">
            <h2>This is a subheading</h2>
            <p id="special-paragraph">This is a special paragraph with an ID.</p>
            <ul>
                <li>Item 1</li>
                <li>Item 2</li>
                <li>Item 3</li>
            </ul>
        </div>

    2- Add CSS rules in styles.css to target these elements using class, ID, and element selectors:
            /* Target the container class */
        .container {
            border: 2px solid black;
            padding: 20px;
            margin: 10px;
        }

        /* Target the h2 element */
        h2 {
            color: purple;
        }

        /* Target the paragraph with the ID */
        #special-paragraph {
            font-weight: bold;
            color: red;
        }

        /* Target list items */
        li {
            list-style-type: square;
        }
    3- Save the files and refresh the browser to see the changes.

Step 6: Box Model

    1- Add a new <div> element with some content in index.html:
    <div class="box">
        <p>This is a box to demonstrate the CSS box model.</p>
    </div>

    2- Add CSS rules in styles.css to style the box and demonstrate the box model:

    .box {
    width: 300px;
    height: 150px;
    padding: 20px;
    border: 5px solid orange;
    margin: 30px;
    background-color: lightyellow;
        }
    3- Save the files and refresh the browser to see the box model in action.

Part 2: Final Result
Task: Create a Simple Webpage

Using the concepts learned in this lab, create a simple webpage that includes:

    A centered heading with a custom color.

    A paragraph with a different font and color.

    A list with custom bullet points.

    A styled box with padding, border, and margin.

    Use external CSS to style the page.

Example Final HTML:

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CSS Lab - Final Result</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <h1>My Styled Webpage</h1>
    <p>This is a paragraph with custom styling.</p>
    <ul>
        <li>List item 1</li>
        <li>List item 2</li>
        <li>List item 3</li>
    </ul>
    <div class="box">
        <p>This is a box demonstrating the CSS box model.</p>
    </div>
</body>
</html>

Deliverables:

    1- A folder containing:

        index.html

        styles.css

    2- Screenshots of the final webpage displayed in the browser.

Grading Criteria:

    1- Correct use of inline, internal, and external CSS.       2 pts

    2- Proper application of CSS selectors (element, class, ID).      5 pts

    3- Demonstration of the box model (padding, border, margin).      8 pts 

    4- Overall design and creativity in styling the webpage.          5 pts

