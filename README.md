## Prior Requirements
 - [Web Fundamentals Track][web-fundamentals]
 - [Javascript Track][javascript-track]

----------

## Introduction
Maybe you are a good website programmer, a born coder but you suck terribly bad in art and overall design. 
Maybe your job demands fast websites for clients to see and you can't waste time. 
Maybe you even are a talented artist, but you fight a never ending battle to make sure your website looks consistent in all browsers.
Maybe your projects have become tangled with many sets of random tools and you just need a framework that encompasses all of your basic needs.

Bootstrap is one of the many solutions out there that will help you fix these problems!
By the end of this tutorial, you should be able to answer the following questions on your own:
 1. What is Bootstrap?
 2. What is the need of Bootstrap?
 3. What are its features?
 4. How does it work?
 5. How is the community support for Bootstrap?
 6. What are Bootstrap Problems?
 7. Are there are any other alternatives to Bootstrap? 
 
**So, troops! Let's advance...**

## Twitter Bootstrap 
### What is Twitter Bootstrap ? 
Twitter Bootstrap (mainly known as **Bootstrap** only) is a framework developed by Mark Otto and Jacob Thornton when they were creating Twitter (that is why some people call it Twitter Bootstrap).

Bootstrap is a fast, intuitive and powerful front-end framework for faster and easier web development. It gives you all the tools you need to make websites, web applications and prototypes.

Bootstrap has template files, as well as a lot of optional JavaScript extensions that allow you to make modal windows, drop down menus, tab controls and carousel controls, which are all styled in advance, saving you from the trouble.

As if that was not enough, it also comes with styles for buttons, forms, tables,  typography and a collection of over 140 icons in both black and white versions.

Another very important feature of Bootstrap is that it comes with a 12 column grid system. If you don't know what that is, there is no problem - just know that it allows you to divide your website in equally spaced columns, thus making it look the same in all computers, with big screens, small screens, and even smartphones and tablets. 

Bootstrap was originally designed to help provide some consistency across tools the guys were building internally. Since its first public (open source) release in 2011 (see the blog post [here][4]) it has found huge popularity among web developers for its ease of use and feature set, and in 2012 was the most popular project on [GitHub][5]. Its advocates praise Bootstrap’s ability to build usable applications, with clean code, quickly and easily. 

### Purpose of Development ? 
Before Bootstrap, various libraries and tools were used for interface development and overall web design, which led to inconsistencies and resulted in code very hard to maintain over time. According to Twitter developer Mark Otto, in the face of those challenges:

 > (...) [A] super small group of developers and I got together to design and build a new internal tool and saw an opportunity to do something more. Through that process, we saw ourselves build something much more substantial than another internal tool. Months later, we ended up with an early version of Bootstrap as a way to document and share common design patterns and assets within the company. (...)

Bootstrap was born from the need to fix this problem, and it is this focus that made it the popular framework many know and use today.

### At its heart 
At its heart, Twitter Bootstrap is basically simple good old CSS, but it uses the [LESS][6] pre-processor to add a lot more functionality than CSS could otherwise provide, together with JavaScript plugins and an HTML grid system.
Because you can actually choose what you want to download from the web page, the package size is variable, giving you a lot of choice to make, or if you are like me, just download everything without second thoughts :P

### Features
 - **Fixed and Fluid Layouts** - A standard 940 pixel wide and 12 column grid system is provided, in a fixed and fluid version. The fixed version defines column's size by  pixels and the fluid version uses % instead. One way or another, the grid system allows you to make Fixed or Fluid layouts and to easily structure your website skeleton.
 - **Support for responsive design** - Bootstrap allows you turn on the responsive design feature. This feature will adjust your website to other screen sizes (from other devices, such as tablets or smartphones) making it work without you having to change single line of code.
 - **Interface components** - A large number of interface components are also provided. These include standard buttons, labels, pre-formatted warning and system messages, navigation controls, wizard controls, pagination, and breadcrumbs.
 - **JavaScript snippets** - Again the focus here is on user interface elements. Included is code to help build tool tips, dialog boxes, as well as more traditional form and input elements (including a nice auto complete feature).

### Download Bootstrap
There are two ways to get Bootstrap:
 1. Download everything
 2. Customize your download

#### Download everything
 1.  Go to the [Bootstrap homepage](http://twitter.github.com/bootstrap/)
 2.  Click on the large Download Bootstrap button.
 3. Locate the download file and unzip or extract it. 


For version 2.3.2, you should get a folder named simply bootstrap. Inside this folder you should find the folders and files shown:

    bootstrap/
        ├── css/
        │   ├── bootstrap.css
        │   ├── bootstrap.min.css
        │   ├── bootstrap-responsive.css
        │   └── bootstrap-responsive.min.css
        ├── js/
        │   ├── bootstrap.js
        │   └── bootstrap.min.js
        └── img/
            ├── glyphicons-halflings.png
            └── glyphicons-halflings-white.png

#### Customize your download
 1. Click the **Customize** tab on the top of the page.
 2. Check, uncheck and modify everything you want for your customized download.
 3. Click the Customize Download button and done!

### Get Started
For this simple example, I am going to focus on the following functionalities of bootstrap:
 - Responsive design
 - Navigation Bar
 - Fluid Layout
 - Sidebar

Once we are done with this lesson, your website will look like this (click the image to visit the website!):
[![website-screenshot][website-screenshot]][get-started-website]

#### Files and Resources
As you can see, this website comes loaded with some resources, namely images. Although I could use a link to the images I decided not to do so because that would be a bad practice, thus I downloaded all the necessary images into a nice folder. You can download all the necessary images by clicking the following links:
 - [codecademy-logo-white][codecademy-logo-white]
 - [gridbg][gridbg]

The full CSS file and HTML files can also be found here:
 - [style.css][style.css]
 - [index.html][index.html]

Before we start with the mini-guide, I want to make clear, that although this website does have a CSS file, the main focus of this lesson will be the Bootstrap code, which is all in the HTML file. That is the beauty of Bootstrap, you don't need to worry about anything else.

#### Folder Organization
One important aspect of any web developer is how he/she organizes the files of the website. In my case, I will be using the following folder structure:

    myBootstrapWebsite/
          ├── css/
          │   └── style.css
          ├── html/
          │   └── index.html
          ├── image/
          │   ├── codecademy-logo-white.png
          │   └── gridbg.gif
          └── library/
              └── bootstrap (folder, with all extracted files)

So, as you can see the structure of my website is quite simple. Just as any first example should be :P

#### Responsive design
Responsive design is an optional feature that you can enable in your website. It basically allows you to display your website in multiple devices of various screen sizes making it look consistent and readable without you having to change a single line of code.
By detecting the size of the screen Bootstrap automatically adjusts your website in the best possible way.

This power however, should **not** be abused. Bootstrap official documentation defends that if you are ever to be serious about web development, you should make a version of your website for each device. For the purposes of this simple tutorial however, we will be using the responsive design feature, so you can see it in action.

To enable the responsive design feature to your website, you have to add the following piece of HTML code to the header:

    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link href="../library/bootstrap/css/bootstrap-responsive.css" rel="stylesheet">

And you are done! Just remember to **update the paths**!

How can you test it? Well, that is easy. You can simply resize your browser to any size. In fact, you can try it with my example website. 

This is what it looks like when I have responsive design **enabled**:
![responsive-design-true][responsive-design-true]

And this is what happens when I have responsive design **disabled**:
![responsive-design-false][responsive-design-false]

As you can see there is quite a difference. By just entering 2 lines of code, my website now looks presentable to a client in an Android Tablet or to a client in an iPhone.

#### Navigation Bar
The navigation bar is quite simple. The following code example is quite straight:

    <div class="navbar navbar-fixed-top navbar-inverse">
        <div class="navbar-inner">
            <div class="container-fluid">
                <a class="brand" href="#"><img src="../image/codecademy-logo-white.png" width="111" height="30" alt="w3resource logo"></a>
                <div class="nav-collapse">
                    <ul class="nav">
                        <li class="active"><a href="#">Home</a></li>
                        <li><a href="#about">About</a></li>
                        <li><a href="#contact">Contact</a></li>
                    </ul>
                    <p class="navbar-text pull-right">Logged in as <a href="#">username</a></p>
                </div>
            </div>
        </div>
    </div>  

So, let us now decompose what is happening. This is structured as a set of nested HTML `<div></div>` elements, with some links `<a ...></a>` and an unordered list `<ul><li></li></ul>`. If you made the [Web Fundamentals Track][web-fundamentals] you should be quite familiar with these tags by now. 
The amazing and important thing here, are the classes. They are what defines the style of everything in your page.  

So, with no further delay, by reading the [Twitter Bootstrap How-To][twitter-bootstrap-web-development-how-to] guide, you can easily find out that:

 - `navbar` provides the outside containing element for all contents of the navbar. 
 - `navbar-inverse` calls for a dark navbar background with light font color.
 - `navbar-fixed-top` fixes the navbar at the top of the window and lets page content
scroll underneath it (this requires padding at the top of the body element. See it in
the embedded style sheet in the head of the index.html file.)
 - `navbar-inner` provides height, padding, and background color and gradients.
 - The div of class `nav-collapse` serves as the containing element for the menu
items which are dropped down in narrow-viewport navigation.
 -  `class="active"` on the Home navigation item provides the darkened
background color which indicates the current page.
 - `container-fluid` is the fluid brother of `container` and it constrains the width of the navbar contents, centers them within a wide screen, and includes a clearfix so that it will contain floated child elements.
 - Last, `navbar-text pull-right` simply define that its a text field and we want it placed in the right.

See? Reading the documentation actually helps! And this was pretty much easy :p

#### Fluid Layout
Bootstrap has two options for your 940 grid layout. One of them is the **fixed** grid layout. In this layout, everything is measured by pixels, and the website overall will look like what you expect if all the screens have a similar size or width-height ratio.
The other option, and the one I use, is the **fluid** grid. This fluid grid allows us to build fluid layouts. These layouts use `%` instead of pixels for the measurements, and so everything will always scale accordingly, even if the screen sizes differ significantly or their ratio is not perfect.

Fixed and Fluid grids allows us to do Fixed and Fluid Layouts respectively (you can actually mix them, but **you should never do that**). The two have some basic differences and I understand that it may be confusing for some beginners. For this reason, I strongly recommend watching and reading the following sources:
 - [tuts-plus-grid][tuts-plus-grid]
 - [stackoverflow-layout-grid-explained][stackoverflow-layout-grid-explained]

Now that you probably understand better the differences between fixed and fluid layouts (and why I decided to use a fluid layout) let us delve into the code:

    <div class="container-fluid">  
        <div class="row-fluid">  
            <div class="span3">
                <!-- Stuff inside -->  
            </div>  
            
            <div class="span9">
                <div class="row-fluid">  
                    <div class="span3">
                        <!-- Stuff inside -->  
                    </div> 
                        
                    <div class="span3">
                        <!-- Stuff inside -->  
                    </div> 
                    
                    <div class="span3">
                        <!-- Stuff inside -->  
                    </div> 
                </div>  
                <!-- More stuff inside, like footers and such -->
            </div>
        </div>

Presented here is the skeleton of the application, the Fluid Grid that I used. Assuming that you have seen the previous video on grid systems and that you played a little bit with the stackoverflow question that I presented earlier, this should be familiar.

First I define a `container-fluid`, which will hold my rows, and then I create one giant row for the website. This row shall be the mother row. I divided the mother row into two spans, one with size 3 and another with size 9. The span3 portion will receive a sidebar, which we will discuss later. The span9 portion is a little more tricky. Inside this portion I add a leaderboard and create another row, dividing the later one evenly with three span4 tags.

To better understand this concept you should fire up [Chrome Dev Tools][chrome-dev-tools], or in may case (Firefox Fanboy), [Firebug][ff-firebug]!

Firebug will highlight the areas of the respective HTML tags that we have selected. 

Mother Row:
![mother-row][mother-row]

As you can see, the mother row encompasses all. 
 
Then we have the span3 (with a sidebar child tag) and span9 tags, which are children of the mother row:
![span3][span3]
![span9][span9]

span9 has a leaderboard (which we do not really care about) and another row.
![leaderboard][leaderboard]
![child-row][child-row]

And now, the row inside span9, has three span4 tags.
![span4-1][span4-1]
![span4-2][span4-2]
![span4-3][span4-3]

By now the Fluid layout on my website should be clear to you. If not, I strongly recommend that you either install and use [Firebug][ff-firebug], or use [Chrome Dev Tools][chrome-dev-tools] to toy around with the example.

#### Sidebar
With the skeleton base explain we can now go to the sidebar:

    <div class="well sidebar-nav">  
        <ul class="nav nav-list">  
            <li class="nav-header">Frontend</li>  
            <li class="active"><a href="#">HTML 4.01</a></li>  
            <li><a href="#">HTML5</a></li>  
            <li><a href="#">CSS</a></li>  
            <li><a href="#">JavaScript</a></li>  
            <li><a href="#">Twitter Bootstrap</a></li>  
            <li><a href="#">Flex</a></li>
            <li><a href="#">JQuery</a></li>
            <li><a href="#">Javascript</a></li>
            <li class="nav-header">Backend</li>  
            <li><a href="#">PHP</a></li>  
            <li><a href="#">Ruby</a></li>  
            <li><a href="#">Python</a></li>  
        </ul>  
    </div>


The sidebar is quite simple as you can see. You create a sidebar by adding `class=sidebar-nav`. The `well` part is just to give a simple inset effect to the bar.
The content of the sidebar is an unordered list.The classes `nav nav-list` set our sidebar with a content that we can "navigate" through. 
Finally, `nav-header` defines a header, or a separation if you will, on our bar. 

#### Conclusion
And that is it! By pulling all of these concepts together you should now have your first Bootstrap website done! This website is responsive and fluid, so it will work in pretty much every device!
Here we explored some of Bootstrap basic concepts, but trust me, your journey has only begun, there is a lot more for you to learn! 

### Learning Resources 
Bootstrap is quite a complex framework, and so you have a lot of learning to do. In this section we provide guides and links for you to learn more. If you find any resources you feel like sharing, please suggest them!

 1. [Official Website][official-website] - for everything about Bootstrap.
 2. [w3resources][w3r-bootstrap] - for code examples. Careful though, they use a customized version of Bootstrap 2.1.0 in their examples, and you have a more recent version.
 3. [Twitter Bootstrap Web Development How-To][twitter-bootstrap-web-development-how-to] - a free PDF book that explains everything about Bootstrap and aids you in the creation of examples.
 4. [Youtube series][youtube-bootstrap] - a set of Youtube videos made by an amateur that introduce you to the basic functionalities of Bootstrap.
 5. [Tuts Plus Introduction to Bootstrap][tuts-plus] - a set of 2 videos that introduces you to bootstrap and explains very clearly the concept of grids and layouts. By far the best in the matter.

### Bootstrap community and free resources
One of the main advantages of using a well known framework is the community support. This is very helpful in our case, mainly because it means we can use free template and themes from the Internet to develop our websites. Following are a few examples of websites that fill this niche:
 - http://bootswatch.com/
 - http://www.bootstrapfree.com/
 - http://bootstrapstyler.com/
 - http://responsivewebinc.com/bootstrap-themes/

There are far more free themes and templates in the Internet that you can explore, in fact these are just some of the top results from my Google search. If however you find something worth mentioning, please suggest it here so we can add it!

### Bootstrap problems
By now you probably think that Bootstrap is the *holy grail*. Well, Bootstrap is very good, but it also has many problems. Some of the mains hassles you will find when working are:
 - There is a large set of customization to Bootstrap. This divides communities and thus there are many customized and personalized versions of Bootstrap out there. Remember that although a website may use Bootstrap, its customized features may make it completely different from what you would normally expect. Furthermore, different customizations of Bootstrap are not compatible between them.
 - Bootstrap has quite a limited set of art and design tools. Some people try to fix this by creating kits that expand Bootstrap's capabilities, such as [Flat UI][flat-ui].
 - Bootstrap had many version before, and their compatibility changes significantly from version to version.

### Bootstrap alternatives and competition
 1. [Foundation][8] - Advertised as "The most advanced responsive front-end framework in the world" Foundation directly competes with Twitter Bootstrap in the same area. For more information, feel free to read [this blog that compares the two][bootstrap-vs-foundation].
 2. [Sassaparilla][9] - Sassaparilla is a fast way to start your responsive web design projects that harness the power of SASS and Compass.
 3. [Compass][10] - Quick start Compass with Mixture, Compass is an open-source CSS Authoring Framework.
 4. [inuit.css][11] - A powerfull, scalable, Sass-based, BEM, OOCSS framework.
 5. [Bourbon][12] - A simple and lightweight mixin library for Sass.
 6. [Nib][13] - Nib is a small and powerful library for the Stylus CSS language.
 7. Additionally, you should also check the following pages:
   - [listly alternatives][listly-alts]
   - [stackoverflow alternatives][stackoverflow-alts]
   - [alternativeto.net list][alternativeto-alts]

## Conclusion
This tutorial served as a **small** introduction to Bootstrap. If you have never heard of it before then now you should be at least familiar with the basic concepts of the framework, and hopefully ready to expand your knowledge and fly on your own.
If you have read / watched all of our recommendations, you should now be able to answer all of the introductory questions. Still, here is a small summary:

 1. Bootstrap is a framework with CSS and Javascript files that helps you developed websites faster by giving you a pre-defined, customizable and expandable set of tools that you can use.
 2. In the old days, people had to use several different tools to make their websites work. These would eventually lead to projects hard to maintain and tangled code. Furthermore, there was no easy way for people to make their website consistent in multiple devices, screens and it was very hard to develop a website without art design resources. Bootstrap was born from these needs and it addresses them all.
 3. Bootstrap has many features. For a detailed information guide you should check the [Bootstrap official website][official-website]. However, the ones that we addressed in this tutorial are the fixed and fluid layouts, responsive design, many interface components and Javascript snippets as well.
 4. Bootstrap works by adding specific code to your HTML. There you use pre-defined classes for your tags, and you let Bootstrap do the magic.
 5. The community support for Bootstrap is great, to say the least. There plenty of tutorials out there, free templates and books that you can read for free. 
 6. This big diversity can ultimately harm Bootstrap because it divides the community and therefore its resources. Also, bootstrap differs significantly from version to version and its artistic tools are quite limited. 
 7. This list could go on and on. In fact the answer to this question has a chapter on its own. You should totally go and read it again :P

## MORE GUIDES
Here are more guides from me

 - [Automaticaly Deploy your site with GITHub][14]
 - [GITHub Patch Mode: git add -p: The most powerful git feature you're not using yet][15]

## Sources 
 - Bootstrap Tutorial: http://www.w3resource.com/twitter-bootstrap/tutorial.php
 - Bootstrap info: http://en.wikipedia.org/wiki/Twitter_Bootstrap
 - What is Bootstrap?: http://www.infragistics.com/community/blogs/marketing/archive/2013/04/17/what-is-twitter-bootstrap.aspx
 - Official page: http://twitter.github.io/bootstrap/
 - Bootstrap info: https://dev.twitter.com/blog/bootstrap-twitter

## Special Thanks
 - To [Ksenja][ksenja] for supporting me and being the only person doing so. It is thanks to her that I got the strength to finish this ahead of time. Hopefully I did not screw up and hopefully it was worth it. 

  [4]: https://dev.twitter.com/blog/bootstrap-twitter
  [5]: https://github.com/twitter/bootstrap
  [6]: http://lesscss.org/
  [8]: http://foundation.zurb.com/
  [9]: http://www.sass.fffunction.co/
  [10]: http://compass-style.org/
  [11]: http://inuitcss.com/
  [12]: http://bourbon.io/
  [13]: http://visionmedia.github.io/nib/
  [14]: https://github.com/Dev-Dipesh/automatic-deploy-site-with-git
  [15]: https://github.com/Dev-Dipesh/Guide-to-GIT-patch-mode

  [web-fundamentals]: http://www.codecademy.com/tracks/web
  [javascript-track]: http://www.codecademy.com/tracks/javascript
  [poll-results]: https://docs.google.com/forms/d/1Q-UlF0ddhX34HO3Q6wa92cztAVKbj4vqQUYLWRYKZSE/viewanalytics

  [official-website]: http://twitter.github.io/bootstrap/index.html
  [tuts-plus]: https://tutsplus.com/lesson/bootstrap-overview-and-installation/
  [tuts-plus-grid]: https://tutsplus.com/lesson/the-grid-system/
	  
  [stackoverflow-layout-grid-explained]: http://stackoverflow.com/questions/9780333/fluid-or-fixed-grid-system-in-responsive-design-based-on-twitter-bootstrap
  
  [w3r-bootstrap]: http://www.w3resource.com/twitter-bootstrap/tutorial.php
  [twitter-bootstrap-web-development-how-to]: http://www.it-ebooks.info/book/2188/
  [youtube-bootstrap]: http://www.youtube.com/watch?v=BVFQc0iGFwU&list=PL7029EEFC21D2DC58
  
  [chrome-dev-tools]: https://developers.google.com/chrome-developer-tools/ 
  [ff-firebug]: http://getfirebug.com/

  [bootstrap-vs-foundation]: http://designshack.net/articles/css/framework-fight-zurb-foundation-vs-twitter-bootstrap/
 
  [listly-alts]: http://list.ly/list/303-alternatives-to-twitter-bootstrap-html5-css3-responsive-framework

  [stackoverflow-alts]: http://stackoverflow.com/questions/9212536/alternatives-to-twitter-bootstrap

  [alternativeto-alts]: http://alternativeto.net/software/bootstrap/
  [flat-ui]: http://designmodo.github.io/Flat-UI/
	
  [ksenja]: http://www.codecademy.com/ksenja
  [Dispesh]: http://www.codecademy.com/dev-dipesh
  [Pedro]: http://www.codecademy.com/fl4m3ph03n1x

  [get-started-website]: http://tinyurl.com/n3fnyeh
  [website-screenshot]: http://tinyurl.com/loboll6
  [codecademy-logo-white]: http://tinyurl.com/ljwoh2d
  [gridbg]: http://tinyurl.com/lpd47yp
  [style.css]: http://tny.cz/edba6574
  [index.html]: http://tny.cz/ba9a9b74
  [responsive-design-true]: http://tinyurl.com/lb6lwne
  [responsive-design-false]: http://tinyurl.com/l6bkofv
  [mother-row]: http://tinyurl.com/ldh4mf4
  [span3]: http://tinyurl.com/kkwhb4o
  [span9]: http://tinyurl.com/k6vlzkc
  [leaderboard]: http://tinyurl.com/ldef7o2
  [child-row]: http://tinyurl.com/kz5l8l3
  [span4-1]: http://tinyurl.com/nxxmd5y
  [span4-2]: http://tinyurl.com/n7tkppv
  [span4-3]: http://tinyurl.com/mnm374f
