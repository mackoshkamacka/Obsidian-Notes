2024-07-3120:07
Status: #CS50 #Incomplete 


![[oihoihoi.png]]

HTML (Hypertext Markup Language) is a language but not a programming language as it lacks variables, logic, function etc. It is a markup language, using angle bracket enclosed tags to semantically define the structure of a web page, causing the plain text inside of sets of tags to be interpreted by web browsers in different ways.

```html
//Example of 'Hello world' on a website
<html>
//Indicates that the language being used
	<head> 
//What shows in the tab of your browser
		<title> 
//Displayed text 
			Hello, world 
		</title> 
//Closes the operation (done automatically) 
	</head> 
	<body> 
//content of the page 
		World hello 
	</body>
</html> 

==
<html><head><title>Hello, world</title></head><body>World, hello</body></html>
//Removed white space

```

```html
//Common HTML tags 
<b>, </b> //Where it bolds the surrounded text 
<i>, </i> //Text is in itallics 
<u>, </u> //Text is underlined 
<p>, </p> //Text is rendered as a paragraph 
<hX>, </hX> //Where x is = to level section header (size of header) 
<ul>, </ul> //Demarcate an unordered, bulleted list 
<ol>, </ol> //Demarcate the beginning and end of an ordered (numbered) list
<li>, </li> //Demarcate list items with an ordered or unordered list 
<table>, </table> //Demarcate the beginning and end of a table definition 
<tr>, </tr> //Demarcate the begining and end of a row within a table
<td>, </td> //Demarcate the begining and end of a column within a row within a table
<form>, </form> //Demarcate the begining and end of an HTML form (
<div>, </div> //Demarcate the begining and end of an arbitrary HTML division
<a href=X>, </a> //Creates a hyperlink to a webpage X, with tw=ext being refered to as linked text
<!DOCTYPE html> //Specific to HTML5, lets browser know that's the standard you're using 
<!--,--> //Demarcates the begining and end of a comment <!--,(comments)-->  
<img scr=X.../> // Displays an image located at X (has additional attributes, such as specifying width/height) 
<input nuam=X type=Y/> // (Self closing tags) Define a field withing an HTML form. X is a unique ID for theat field, Y is what data type it accepts 


# Source(s)