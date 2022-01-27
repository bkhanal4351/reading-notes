**What Is CSS?**

CSS(Cascading Style Sheets) is a design language used to simplify the process of making web pages presentable. CSS gives the look and feel part of a web page. CSS can be used to color the text, change fonts, change background colors, how columns are sized, where to position the text/images, padding etc.

***How to Add CSS**
There are three ways to insert style sheet.

1. External CSS: By just chaging one file, you can change the look of an entire website.

<!DOCTYPE html>
<html>
<head>
<link rel="stylesheet" href="mystyle.css">
</head>
<body>

<h1>This is a heading</h1>
<p>This is a paragraph.</p>

</body>
</html>


2. Internal CSS: The internal style is defined inside the element, inside head section.

<!DOCTYPE html>
<html>
<head>
<style>
body {
  background-color: red;
}

h1 {
  color: maroon;
  margin-left: 40px;
}
</style>
</head>
<body>

<h1>This is a heading</h1>
<p>This is a paragraph.</p>

</body>
</html>
\


3. Inline CSS An inline style is used to apply a unique style for a single element.

<!DOCTYPE html>
<html>
<body>

<h1 style="color:red;text-align:center;">This is a heading</h1>
<p style="color:blue;">This is a paragraph.</p>

</body>
</html>


**CSS COLOR**

Color specifies the color of the text or bacgrounds.