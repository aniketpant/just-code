# Chapter 4: Working with HTML

HTML stands for HyperText Markup Language. It's very much like English and simple to pick up. For basic purposes it won't be a hassle at all but to write good scalable code, you will need a lot of experience along with in-depth knowledge of HTML.

As you might have read in Chapter 03, writing HTML is like building your house. HTML creates a structure for the page which the browser can render. There are very few rules which make a lot of sense.

Let me first list down a few things you need to keep in mind before you start with writing HTML.

## There are things called as tags

When we talk about HTML, it uses a number of tags which come in two categories. One is a self-closing and the second needs to be closed manually. We will take a look at both these categories soon.

## Tell the browser where you code starts and ends

It's extremely important to the browser where your HTML code starts and where it ends. This is done by using a `<html>` tag.

    <html>
      ...
    </html>

## The DOCTYPE

The DOCTYPE also known as document type declaration, is an instruction which associates a webpage with a document type definition (DTD). The DTD is the formal definition for a particular version of HTML. This is all you should know about the DOCTYPE because it has been rendered useless (but required) header only to trigger "standards mode" in common browsers.

The doctype precedes the `<html>` tag.

    <!DOCTYPE html>
    <html>
      ...
    </html>

## The head

Moving on another step, you will come across something called as the `<head>` tag. The section between `<head>` and `</head>` houses a lot of information of the webpage. The title you see on the title bar, the stylesheets required by the webpage, other meta information and at times even JavaScript.

    <!DOCTYPE html>
    <html>
    <head>
      <title>Your page title</title>

      <link rel="stylesheet" type="text/css" href="path/to/some/stylesheet">
      <style type="text/css">
        /**
         * You can write some CSS here
         */
      </style>

      <script type="text/javascript" src="path/to/some/script"></script>
      <script type="text/javascript">
        /**
         * You can also write JavaScript here.
         */
      </script>
    </head>
      ...
    </html>

### Title

We can start with `<title>`. Whatever text you put between `<title>` and `</title>`, it will be rendered in the title bar of the page.

### Stylesheets

There are three ways to write CSS. We will discuss the technicalities of it in the next chapter. For now, you should know that we can link our webpage with an external stylesheet using the `<link>` tag. We can also write CSS in the page between `<style>` and `</style>` tags.

### Scripts

Similar to stylesheets, JavaScripts can be either requested on a page or written. To use an external JavaScript, you can make use of the `<script>` tag.

Note: The number of `<link>` and `<script>` you have on your page, is equal to the number of GET requests sent.

## Body

Whatever comes inside the body is what you see on the page excluding the stylesheets and the JavaScripts linked beforehand.

    <!DOCTYPE html>
    <html>
    <head>
      ...
    </head>
    <body>
      <h1>Sample Page Title</h1>

      <p>This is some paragraph text. This text can also contain a <a href="#">link</a>.</p>
    </body>
    </html>