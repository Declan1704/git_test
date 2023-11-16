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

### Opening links in a new tab

The method shown above opens links in the same tab as the webpage containing them. This is the default behaviour of most browsers and it can be changed.
All we need is another attribute: the `target` attribute.

While `href` specifies the destination link, target specifies where the linked resource will be opened. If it is not present, then, by default, it will take on the` _self` value which opens the link in the current tab. To open the link in a new tab or window (depends on browser settings) you can set it to `_blank` as follows:

`<a href="https://www.theodinproject.com/about" target="_blank" rel="noopener noreferrer">click me</a>`

You may have noticed that we snuck in the `rel` attribute above. This attribute is used to describe the relation between the current page and the linked document.

The `noopener` value prevents the opened link from gaining access to the webpage from which it was opened. 
The `noreferrer` value prevents the opened link from knowing which webpage or resource has a link (or ‘reference’) to it. 
It also includes the `noopener` behaviour and thus can be used by itself as well.

### Absolute and relative links

Generally, there are two kinds of links we will create:

1) Links to pages on other websites on the internet
2) Links to pages located on our own websites


#### Absolute Links

Links to pages on other websites on the internet are called absolute links. A typical absolute link will be made up of the following parts: `protocol://domain/path`. An absolute link will always contain the protocol and domain of the destination.

Ex: `https://www.theodinproject.com/about`

#### Relative Links

Links to other pages within our own website are called relative links. Relative links do not include the domain name, since it is another page on the same site, it assumes the domain name will be the same as the page we created the link on.

Relative links only include the file path to the other page, 
relative to the page you are creating the link on.

If suppose you want to link an html file (say about.html) from your main file (say index.html)
Then this is how its done

```
<body>
  <h1>Homepage</h1>

	<a href="about.html">About</a>
</body>
```

This is if your html file to be linked is in the same directory as the main file.

But if you want to link your html file which is in another directory (say pages directory),
Then this is how we do it:

```
<body>
  <h1>Homepage</h1>
  <a href="pages/about.html">About</a>
</body>
```

In many cases, this will work just fine; however, you can still run into unexpected issues with this approach. Prepending `./` before the link will in most cases prevent such issues. By adding `./` you are specifying to your code that it should start looking for the file/directory relative to the current directory.

Ex:

```
<body>
  <h1>Homepage</h1>
  <a href="./pages/about.html">About</a>
</body>
```

## Image

If you want to insert an image in your web page, then we use the tag `<img>`. But this tag is not sufficient enough.So we use something called an src which refers to the address of the image.
So in order mention the source, go to the image file in the net, copy the image address and the after typing the src, paste the address. 
Ex: `<img src="Address of the image">`

If you want to paste as image which is in your system, then paste the image in the root directory your html file and in the src mention the name of the image.
Ex: `img src="name of the image.jpeg"`


### Image size attributes

While not strictly required, specifying height and width attributes in image tags helps the browser layout the page without causing the page to jump and flash.

It is a good habit to always specify these attributes on every image, even when the image is the correct size or you are using CSS to modify it.

Ex:
`<img src="../images/dog.jpg" height="150" width="150">`





## File Structure

It's very important to organize your files as to read it becomes easy. If you're saving making a directory for images and saving your image in that directory, then its important to mention the directory path in 
the src. 
Ex: `<img src="folder name/image name">`

Make sure that the folder that youre making for the images should be in the same root directory as the html files.


# lists

# Introduction

Whether it be IMDB’s top 250 movies or the FBI’s most wanted, lists are everywhere on the web and you are going to need one eventually in your webpages.

## Unordered lists

If you want to have a list of items where the order doesn’t matter,then you can use an unordered list.

Unordered lists are created using the `<ul>` element, and each item within the list is created using the list item element `<li>`.

Each list item in an unordered list begins with a bullet point:

Ex:

```
<ul>
  <li>Item 1</li>
  <li>Item 2</li>
  <li>Item 3</li>
</ul>
```

## Ordered lists

If you instead want to create a list of items where the order does matter,then you can use an ordered list.

Ordered lists are created using the `<ol>` element. Each individual item in them is again created using the list item element `<li>`. 
However, each list item in an ordered list begins with a number instead:

Ex:

```
<ol>
  <li>Item 1</li>
  <li>Item 2</li>
  <li>Item 3</li>
</ol>
```

