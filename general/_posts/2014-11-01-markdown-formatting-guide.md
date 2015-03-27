---

title: Markdown Formatting Guide
layout: post
permalink: markdown-formatting-guide 
sequence: 7
tags:
- general
- markdown
- editor

---

## Markdown Formatting Guide

### Headings
You can use up to up to three levels by typing `#` plus a space before a heading; the number of hashtags defines the hierarchy of the heading. 

```
# Heading 1 (Ctrl/⌘ + 1)
## Heading 2 (Ctrl/⌘ + 2)
### THeading 3 (Ctrl/⌘ + 3)
```

### Emphasis
Italics and bold are written by putting `*` or `_` around the text you want to format.

```
**bold** or __bold__ (Ctrl/⌘ + B)
*italics* or _italics_ (Ctrl/⌘ + I)
***bold+italics*** or ___bold+italics___
```

### Strikethrough
You can add a strikethrough to any text by putting `~~` around the text you want to format.

```
~~text~~
```

### Dashes
Beegit supports en-dashes and em-dashes.

```
-- En-dash
--- Em-dash
```

### Numbered lists

Type `1.` then a space. Any number (followed by a period and space) can be used and the list items will be ordered from 1.

```
1. Numbered item 1
2. Numbered item 2
3. Numbered item 3
```

### Bulleted lists
Create a bulleted list by using an asterisk `*`, hyphen `-`, or plus sign `+`, followed by a space.

```
* Bulleted item 1
* Bulleted item 2
* Bulleted item 3
```

### Nesting lists
You can also nest lists several levels deep.

```
1. First level
1.1. Second level
```

```
* First level
    * Second level
```

```
1. First level
    1. Second level
```

### Blockquotes
To make a blockquote, type a `>` symbol plus a space 

> A quoted paragraph

### Links
Create a link by surrounding the link text in square brackets `[]`, followed immediately by the URL in parentheses `()`.

You can manually type a link, or click on the add link icon in the editor bar.

```
[text to link](http://example.com/)
```

### Images
You can link to an image that is hosted outside of Beegit, or we can host it for you through our image CDN. An image link is similar to a link, but it has an exclamation point `!` in front of it. Create an image link by forst typing an exclamation point `!`, then adding an image title in square brackets `[]`, followed immediately by the URL of the image in parentheses `()`.

You can manually type an image link, or click on the add image icon in the editor bar.

```
![image title](http://example.com/image.jpg)
```  

### Code
You can mark up code in-line using backticks ( ` ), or add a fenced code block by four backticks or by adding at least four spaces to the start of a line:

```
This is `inline code`
```

```
```This is a fenced code block```
```

### LaTex Mathematical Expressions
You can render LaTeX mathematical expressions inside Beegit using MathJax. We support both math blocks and inline math.

```
$$
f(n) = n^5 + 4n^2 + 2 |_{n=17}
$$
```

```
Using subscript notation \\(f(n) = n^5 + 4n^2 + 2 |_{n=17}\\)
```


### Footnotes
A footnote label must start with a caret `^` and may contain any inline text (including spaces) between a set of square brackets `[]`. Only the first caret has any special meaning.

A footnote content must start with the label followed by a colon and at least one space. The label used to define the content must exactly match the label used in the body (including capitalization and white space). The content would then follow the label either on the same line or on the next line. 

```
Some text with a footnote label [^1].
```

```
[^1]: Here is the footnote content.
```

The footnote content is added immediately after the footnote label, but appears at the end of the document.

### Tables
To make a table, use vertical bar characters to denote the content that goes into each cell. Start with column headers, separate with a row of cells with dashes, then add further rows of cells.

```
|Column 1 | Column 2 | Column 3  | 
|:---- |:----:| ----:|
|left | center | right  |
|aligned | aligned | aligned  | 
```
**The above code renders this:**

|Column 1 | Column 2 | Column 3  | 
|:---- |:----:| ----:|
|left | center | right  |
|aligned | aligned | aligned  | 


### Separating paragraphs
A new paragraph requires two returns. **Hitting only one return will not create a new paragraph.**


### Escaping
Place a `\` before special formatting characters like `*` `_` to use the literal character instead of using the character as formatting


### Horizontal rules
You can add a horizontal line to your content to help provide a visual break. To do so, add three or more asterisks `*`, hyphens `-`, or underscores `_` on a line by themselves.

```
* * *
```

or

```
-------------
```

or

```
___
```