## Markdown syntax

### Headings
Headers: begin a line with a hash. Each additional hash makes the header smaller

# 1st level heading
## 2nd level heading
### 3rd level heading
#### 4th level heading
##### 5th level heading
###### 6th level heading

### Emphasis

Bold: enclose text in double asterisks
**Bold**

Italics: enclose text in single asterisks
*Italics*

Bold italics: enclose text in asterisks and underscores
**_Bold italics_**

Strikethrough: enclose text in two tildes
~~Strikethrough~~

### Paragraphs

Paragraphs: add either a backslash or 2 blank spaces at the end of the line

This is a section of text which uses a line break to introduce a        

new paragraph.

### Links

Links: place link text in brackets and the URL in parentheses

Download and install the latest version of R [here](https://www.r-project.org)

### Images

Embed images: place optional explanatory text in brackets and the image URL or path in parentheses, preceded by an exclamation mark
![](https://cran.r-project.org/Rlogo.svg)

### Code

Inline code: wrap code in single backticks 

Today’s date is `r format(Sys.time(), '%d %B, %Y')`

Code block: place 3 backticks on a line above and below the code block

```
head(mtcars)
```

### Blockquotes

Blockquotes: begin line with the greater than symbol

> Statistical thinking will one day be as necessary a qualification for efficient citizenship as the ability to read and write.    

(H.G. Wells)

### Lists

Bullet points: Precede each line in a list with a single asterisk, hyphen or plus sign

- readr
- tidyr
- dplyr
- ggplot2

Numbered lists: Precede each line in a list with a number and full stop

1. readr
2. tidyr
3. dplyr
4. ggplot2

To prevent text starting with a number being formatted as a numbered list just add a backslash.

4\. ggplot2

Nested lists: indent each item in the sublist by four spaces

1. tidyverse packages for importing data:
    - readr
    - readxl
    - haven

### Footnotes

Footnotes: place square brackets in text with a caret inside which precedes the footnote text.

Some text with a footnote[^Source: Grolemund and Wickham, 2017.].

### GitHub Flavored Markdown

Task lists: add a space between a dash and an open bracket

- [x] Import data
- [x] Tidy data
- [ ] Transform data
- [ ] Visualise data

Tables: divide words with hyphens to create the column names and then separate each row with a pipe. Colons are used to align the values in the cells.

| Package | Purpose |
|:----- |:---- |
| readr | importing data |
| tidyr | tidying data |
| dplyr | manipulating data |
| ggplot2 | visualising data |

Syntax highlighting: place 3 backticks on a line above and below the code block with the language after the first three backticks

``` r
library(ggplot2)
ggplot(mpg, aes(class)) + 
  geom_bar(colour = "white")
```
