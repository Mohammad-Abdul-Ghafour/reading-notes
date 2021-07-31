# Introductory HTML, CSS and JavaScript

## **What is HTML, CSS and JavaScript?**

<div style="display:flex;">
<img src="https://upload.wikimedia.org/wikipedia/commons/thumb/6/61/HTML5_logo_and_wordmark.svg/512px-HTML5_logo_and_wordmark.svg.png" width="100px" height="100px"><p style="margin-top:40px"><strong>HTML </strong>: stands for Hyper Text Markup Language, HTML describes the structure of pages.</p>
</div>
<div style="display:flex;">
<img style="margin:10px 15px 5px 15px; float: left;" src="https://upload.wikimedia.org/wikipedia/commons/thumb/d/d5/CSS3_logo_and_wordmark.svg/1200px-CSS3_logo_and_wordmark.svg.png" width="73px" height="100px"><p style="margin-top:55px"><strong>CSS</strong> : stands for Cascading Style Sheets, CSS specify how the content of an element should appear.</p>
</div>
<div style="display:flex">
<img style="margin-left:1px" src="https://www.growingsearch.com/blog/wp-content/uploads/2019/02/Javascript-shield.png" width="100px" height="110px"><p style="margin-top:40px"><strong>JS</strong> : JavaScript is a interpreted scripting or programming language that allows you to implement complex and dynamical features on web pages to make web pages dynamic and interactive.</p>
</div>
<br>

## But before we continue to details we should know How the Web Works?
When you visit a website, the web server hosting that site could be anywhere in the world. In order for you to find the location of the web server, your browser will first connect to a Domain Name System (DNS) server. So it is the DNS servers that tell your browser how to find the website.

# HTML :
## As we said HTML Describes the Structure of Pages so how do we use HTML?

HTML uses elements (Tags) that act like containers. They tell you something about the information that lies between their opening and closing tags.

Let's take an example:
```
<!DOCTYPE html> 

 <html>
   <head>
     <title>
     Title of the web page
     </title>
   </head>
   <body>
     <h1 id="H1"> This is the Main Heading </h1>
     <p> This text might be an introduction to the rest of the page. And if the page is a long one it might be split up into several sub-headings.<p>
   </body>
 </html>
```
**DOCTYPE** declaration to tell a browser which version of HTML the page is using.
Because there have been several versions of HTML, each web page should begin with a DOCTYPE declaration

As we see we used `<!DOCTYPE html> ` to tell the browser we are using HTML version 5.

## Head Tag
The `<head>` tag is a container for data about the HTML document like title and metadata.

## Attributes:

Attributes provide additional information about elements and all HTML elements can have attributes and always specified in the start tag usually come in ( name of the attribute ) / ( value of the attribute ) pairs like ( name = "value" )

for example `id="H1"` is ID attributes used to uniquely identify that element from other elements on the page.

## HTML LAYOUT
An HTML layout is a blueprint used to arrange web pages in a well-defined manner. It is easy to navigate, simple to understand and uses HTML tags to customize web design elements.

![HTML LAYOUT](https://stuyhsdesign.files.wordpress.com/2016/05/yoko-html5.png)

## SITE MAP
A sitemap is a list of the pages of a website and how they’re related to each other. and it helps to decide what information should go on each page.

**Example Site Map**

![Example Site Map](https://spaciousphilly.com/wp-content/uploads/2020/02/Africa-Peacebuilding-Institute-New-Sitemap-2-1024x629.png)

## WIREFRAMES

Wireframing is a way to design a website at the structural level. It means that before we get into coding we need to drow the website or application user interface, that the client or user want. So wireframe is a layout of a web page that demonstrates what interface elements will contains.

![WIREFRAMES](https://www.comentum.com/images/wireframes-sample/ecommerce/home.png)

# JAVASCRIPT :
## JavaScript is a lightweight scripting or programming language that enables you to create dynamic behavior. But how to script?

To write a script, you need to first state your goal and then list the tasks that need to be completed in order to achieve it.

#### So what can it really do?
JavaScript language consists of some common programming features that allow you to do things like:
* Store useful values inside variables. for example:

`var name = 10`
Here we assigned to the variable (`name`) a value of `10`

* Running code in response to certain events occurring on a web page. for example:
```
var favMusic = prompt("what is your favorite music?")
if(favMusic == "Arabic"){

}
else if (favMusic =="English"){

}
else if(favMusic =="Global"){

}
else{
  
}
```

Here the user will enter his/her favorite music and with every choice he/she made will come with different response.

... And Much More ...