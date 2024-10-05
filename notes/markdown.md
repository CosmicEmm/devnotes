# Markdown
* Markdown is a markup language that is used to produce beautifully formatted text documents.
* Markdown also works on Discord and Reddit.
* There are many flavors of markdown. The flavor of markdown specifically for GitHub is called GFN.
* A markdown file has the .md extension.
* One of the most common applications of markdown is a **README.md** file.
* To start a new paragraph, separate it from the previous one by one empty line.
## Markdown Syntax
### Headings
There are six levels of headings available.
```md
# Heading 1
## Heading 2
### Heading 3
#### Heading 4
##### Heading 5
###### Heading 6
```

### Bold
```md
**Nike** or __Adidas__
```
**Nike** or __Adidas__
### Italics
```md
*Rome* or _Milan_
```
*Rome* or _Milan_
### Bold and Italics
```md
***Chocolate*** or ___Vanilla___
```
***Chocolate*** or ___Vanilla___
### Strikethrough
```md
~~Tesla~~
```
~~Tesla~~
### Highlight
```md
==Deep Work==
```
==Deep Work== (not supported by GitHub)

HTML Alternative:
```html
<mark>Deep Work</mark>
```
<mark>Deep Work</mark>
### Superscript and Subscript
```md
x^2^
H~2~O
```
x^2^

H~2~0

GitHub's markdown (GFN) doesn't support superscript and subscript.

HTML Alternative:
```html
x<sup>2</sup>
H<sub>2</sub>O
```
Superscript = x<sup>2</sup>

Subscript = H<sub>2</sub>O
### Emojis
```md
:smile:
```
GitHub doesn't support this markdown syntax.

Alternative:

😊

Copy and Paste the actual emoji in your GitHub markdown file.
### Checklist
x within the square brackets indicates a ticked checklist.
```md
- [ ] Read Book
- [x] Exercise
- [ ] Journal
```
- [ ] Read Book
- [x] Exercise
- [ ] Journal

### List
#### Unordered List
```md
* Apples
    * Golden Apples
    * Green Apples
* Oranges
* Grapes
* Strawberries
```
Substituting * with - or + will give the same result. To nest a list within a list, press the Tab key once or the Space key 4 times.
* Apples
    * Golden Apples
    * Green Apples
* Oranges
* Grapes
* Strawberries
#### Ordered List
```
1. Game of Thrones
2. Clash of Kings
3. Storm of Swords
4. Feast for Crows
5. Dance with Dragons
```
1. Game of Thrones
2. Clash of Kings
3. Storm of Swords
4. Feast for Crows
5. Dance with Dragons
### Code
#### Inline Code
Enclose in single backticks. The code will be displayed in monospace font.
```md
This is `let c = 10`
```
This is `let c = 10`
#### Code Block
* Place three backticks ``` on a line above and below the code block.
* You can indicate the programming language after the opening backticks (e.g. js, py, md, html, etc.). That will render out the correctly formatted and highlighted version of the code.
```md
const a = 10
let y = 8
```
### Table
```md
|Player|Team|
|---|---|
|Kroos|Real Madrid|
|Scholes|Man United|
|Pirlo|AC Milan|
```
* The divider separates the header from the rest and must be atleast three dashes.

* The bars don't have to line up although you can do that for better readibility.

|Player|Team|
|---|---|
|Kroos|Real Madrid|
|Scholes|Man United|
|Pirlo|AC Milan|
#### Changing Text Alignment
```md
|Right|Center|Left|
|----:|:----:|:----|
|Steve Jobs|Apple|US|
|Bill Gates|Microsoft|US|
|Jack Ma|Alibaba|China|
```
|Right|Center|Left|
|----:|:----:|:----|
|Steve Jobs|Apple|US|
|Bill Gates|Microsoft|US|
|Jack Ma|Alibaba|China|
### Convert Text to Link
#### Relative Link
Link directly between different documentation files.
```md
[Dev Logs](/README.md)
```
[Dev Logs](/README.md)
#### External Link
```
[Follow me on X](https://x.com/Philomath4Life)
```
[Follow me on X](https://x.com/Philomath4Life)

If the display text and link are the same, a shortcut is to use <>
```md
<www.reddit.com>
```
<www.reddit.com>
### Render an Image
```md
![Coding](https://cdn-icons-png.flaticon.com/256/10817/10817310.png)
```
![Coding](https://cdn-icons-png.flaticon.com/256/10817/10817310.png)
### Block Quote
```md
>Those who don't study history are doomed to repeat it. - Lex Fridman
```
>Those who don't study history are doomed to repeat it. - Lex Fridman

You can even create nested block quotes.
```md
>Three Fs of Business:
>>* Freedom
>>* Fulfillment
>>* Finance
```
>Three Fs of Business:
>>* Freedom
>>* Fulfillment
>>* Finance
### Horizontal Ruler
```md
*** or ___ or ---
```
---



