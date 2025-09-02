### This is page 1
<!-- 
Note in the following, I use the ../ to go up one directory level
to access the Resources folder.
-->
#### This is an image from Resources:
![green_folder](/Resources/green_folder.png | site.baseurl)

#### Two images from Resources on same line:
![green _folder](/Resources/green_folder.png) ![blue_folder](../Resources/blue_folder.png)

#### This uses an image to link back to the home page:
<!-- 
Note in the following, if I use index.md, VSCode previews correctly but the 
browser displays the markdown file as plain text. If I use index.html, the browser
renders the page correctly, but the link is broken in VSCode. 
Use this technique to create a clickable image link back to the home page.
-->
[![yellow_folder](/yellow_folder.png)](/index.html)

#### Fix the dimensions of the green image using attribute list:
![green_folder](/Resources/green_folder.png){:height="150px" width="150px"}

#### This creates a long block of text that will wrap in the browser. 
<!-- 
Note in the following, I am attempting to break a long line
of text into multiple lines in my editor for readability.
The first two lines I copied and pasted from a reference.
At the end of the second line, I used a fn-return keystroke,
then typed the third line manually.
-->
This very long line of text will be broken into multiple lines in my editor for readability.
This is the second line in my editor, but the rendered output will ignore the line break.
And this is the third line, created after typing fn-return 

#### This demonstrates how to style text, in this case, adding color

<span style="color: purple;">Here is another line of text that I would like to appear as purple </span>>

<span style="color: #FF0000;">Here is a line of text that should appear in red font </span>>

#### Return to opening page (home):
[home](/index.md)