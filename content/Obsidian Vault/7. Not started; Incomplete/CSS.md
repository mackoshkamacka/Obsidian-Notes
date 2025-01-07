CSS (Cascading Style Sheets) is also a language used to construct websites. While HTML is used to make the website functional, CSS is used for the aesthetic aspects of a website. A common way to include CSS information into a HTML file is through linking

```css
/*Example of property usage:*/
body'
{
background-color: blue; 
} 
```

```css
//Common CSS porperties
border: style color width
backgroun-color: [keyword e.g.blue|Hex code]
color: [keyword e.g.blue|Hex code] -> ususally applies to text
font-size: [absolute size|relative size]
font-family: [font name|generic name]
text-align: [left|right|center|justify]
```

```css
//ID attributes, an ID selector will apply to an HTML tag with a unique identiifier'
#unique 
{
	border: 4px dotted blue; 
	text-align: right; 
} 
```

```css
//Classes are selectors that will apply only to those HTML tags that have been given identical class attributes'. 
.students 
{
	background-color: yellow;
	opacity: 0.7;
}