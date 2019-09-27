# Tips for typography on the web

90 percent of design is typography. And the other 90 percent is whitespace — Jeffrey Zeldman

1. Measure

- it is the length of a line of type. 
- for single column between 40 to 80 chars is good
- 65 chars is ideal 

Robert Bringhurst's method multiples the type size by 30. 

- So if the type size is 10px, multiplying it by 30 gives you a measure of 300px or around 65 characters per line. The code would look something like this: 

```css
p {
  font-size: 10px;
  max-width: 300px;
}
```

2. Leading

- this is the space between the lines
- a tip is to give around 2pt to 5pt larger than your type
- see the exmaple below, it also depends on your type, color and size etc. 

```css
body {
  font-family: Helvetica, sans-serif;
  font-size: 12px;
  line-height: 16px;
}
```

3. Hanging Quotes

- these should not disrupt the rhythm of left indented paragraphs. 
- the quote should be pushed left into the margin like so

```css
blockquote {
  text-indent: -0.8em;
  font-size: 12px;
}
```


