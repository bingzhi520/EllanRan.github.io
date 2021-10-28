---
layout: default.html
title: Markdown语法
---

# Heading level 1
###### Heading level 6 {#custom-id}

Heading level 1	
===============

Heading level 2 
---------------

The**bold**text. 
The **bold** text. 
The __bold__ text.
<br>

The*Italic*text. 
The *Italic* text. 
The _Italic_ text. 
The <em>Italic</em> text. 
<br>

The***Italic blod***text. 
The ***Italic blod*** text. 
The ___Italic blod___ text. 
The __*Italic blod*__ text. 
The **_Italic blod_** text. 

~~The world is flat.~~

> safcsd
> 
> sdgfasdhga

> safcsd
> 
>> sdgfasdhga

1. First item
    1. Indented item
2. Second item

- First item
    - Indented item
- Second item

* First item
    * Indented item
* Second item

+ First item
    + Indented item
+ Second item

1. First item
    - Indented item
2. Second item

* This is the first list item.

    I need to add another paragraph below the first list item.

* Here's the second list item.

- [x] Write the press release
- [ ] Update the website
- [ ] Contact the media

First Term
: This is the definition of the first term.

Second Term
: This is one definition of the second term.
: This is another definition of the second term.

| Syntax | Description | Test Text |
| :--- | :----: | ---: |
| Header | Title | Here's this |
| Paragraph | Text | And more |

Use `code` in your Markdown file.
``Use `code` in your Markdown file.``
<br>
```
<html>
    <head></head>
```
~~~
<html>
    <head></head>
~~~
Code blocks are normally indented four spaces or one tab. When they’re in a list, indent them eight spaces or two tabs.

    <html>
      <head></head>

1.  Open the file.
2.  Find the following code block on line 21:

        <html>
          <head></head>

3.  Update the title to match the name of your website.

To create a horizontal rule, use three or more asterisks (***), dashes (---), or underscores (___) on a line by themselves.

***

---

___

You can use a backslash to escape the following characters.
\\  \`  \*  \_  \{ \}  \[ \]  \( \)  \#  \+  \-  \.  \!  \|

<br>
it was a [footnote][1] in file last.
<br>
it was another footnote[^footnote] in file.
<br>

![Markdown示例图片描述](https://ellanran.github.io/articles/markdown/markdowneg.png "示例图片")
[![Markdown示例图片描述](https://ellanran.github.io/articles/markdown/markdowneg.png "示例图片")](https://www.exzample.com/)

My github websit is [https://ellanran.github.io/](https://ellanran.github.io/ "ellanran的主页")
<br>
See the section on [`XXXXX`](#custom-id).
<br>
link[my great page](https://www.example.com/my%20great%20page)
<br>
<https://ellanran.github.io/>
<br>
https://ellanran.github.io/
<br>
`https://ellanran.github.io/`
<br>
<599136946@qq.com>


[1]: <https://www.example.com/> "footnote"
[^footnote]: 脚注：巴拉巴拉
