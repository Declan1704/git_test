# Writing Your First HTML Code

`<!DOCTYPE html>` - This tells the browser that it is an html file


`<html></html>` - This tells the browser where the file starts and end


`<title> </title>` - This tag gives the name of the website

`<meta>` - This tag tells the browser the type of characters that we will be using. This type we will be using is
utf-8. The syntax is `<meta charset="utf-8">`


# Paragraphs and Headings

`<p> </p>` - This tells the browser that the content withis this tag is a paragraph. The remaining content will be displayed on the next line after the </p> tag ends.

## Headings
This is used to make a particular line as a heading.


The tag used here is `<h1>`. There are a total of 6 heading tags, `<h1>` to `<h6>`. As it the number goes on increasing, the size of the content within the heading tag goes on diminishing.

Ex: `<h1> Heading 1</h1>`

   ` <h2> Heading 2 </h2>`

# Bold and Italics

## Bold

`<strong></strong>` - This tag is used to convert the normal content within it to bols characters

## Italics

`<em></em>` - This tag is used to convert a normal content within it to italic text.

## Note:
`<b></b> <i></i>` tags also make a content within it as bold and italic. But it is not usually
used.

## Comment 
`< !-- Enter your comment -->` - This is used to write a comment.

## Link

To convert a text to a link, we use the `<a></a>` tag. But only using this tag wont convert it to a link. Hence we use something called as href (hypertext reference). In the href we mention where should the marked text which is converted to a link will take us to.

Ex: `<a href="https://destination link"> Sample text </a>`. Here destination is the link where you want to take the user to.

If you want to make a link that opens another page on the web, then make another html file and write your code. After writing then in your source html file, 
to where you want to mention the link, apply the `<a href="name of the second file">Your content</a>`. Make sure that your second file is in the same directory
as your first file.
