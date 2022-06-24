## Implicit vs. Explicit CSS

Photo by <a href="https://unsplash.com/@lazycreekimages?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText">Michael Dziedzic</a> on <a href="https://unsplash.com/s/photos/css?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText">Unsplash</a>
  
#### Background
As a matter of a long over-due change I needed to make, that is what drove me, to write up this article. So If you find yourself having to read articles from me, please realize, that I have very much deliberated inwardly first, before going ahead to write.

First, this article was born out of the desire to maintain relevance within an ever-dynamic web developer/tech community across the globe. In every sincerity, the hardship at a time or circumstances might have been my first reason for practicing, and learning to code in isolation.  Although the hardship still persists, I have gathered enough experience to break away from that loop thus, going ahead with even this article.

When I first started, there was little of everything and thus triggered a survival instinct, and a scarcity mindset of trying to manage resources, and skills especially those skills, that I found myself to be comfortably conversant with and tried to avoid the outer 'disruptive' world for a while as much as possible.

Until days, turned weeks, weeks into months and years went by, and I forgot my keys to open the doors to the outer world. If you read this, it's because I am breaking the locks to the doors I put in place.

While in isolation, I noticed the bad, the good, and the ugly. To highlight the negative that lies within, practicing programming in isolation or accepting to work solely in isolation, I shall say that in isolation one fails and dies in silence - like a self-imposed-imprisonment, alone and poor. And if one ever succeeds it leads to even more misery inwardly thus hampering mental health, stunting social growth, and eventually leading to the death of brilliance. But more of such discussions I shall save for another article. 

> ***While in isolation, I noticed the bad, the good, and the ugly. To highlight the negative that lies within, practicing programming in isolation or accepting to work solely in isolation, I shall say that in isolation one fails and dies in silence - like self-imposed imprisonment, alone and poor.***

### Introduction

In this article, however, I shall be sharing a discovery I made while working or rather mostly experimenting with ideas in isolation for this has been the whole nature of my advent into programming for the vast majority of the time. There were a few times, I got hired to work freelance. And there was this one time I got hired by a non-profit group, whose aims and objectives were to build entrepreneurial capacities. They hired me to teach a class they had organized on web development(i.e. HTML CSS, and JavaScript), and so I needed to prepare and so I did. 

While preparing for this class I noticed something interesting pop up as I code the examples I'd wanted to teach to my class. These discoveries I made were concerning HTML Markups.

.... Yeah! You can smile at that...

So I know for a fact most people crack up into laughter and a frenzy, when a programmer that they are looking forward to collaborating with, shows up and tends in his or her resume and a link to his or her GitHub projects, and most of them have the category, showing up as HTML underneath there. 

But after reading this article, you can think it up for yourself, whether I am that developer with some "dangerous" levels, of a deeper understanding of 'HTML', that you even require on your team or not.

For a lot of people, **HTML** should never be enumerated among programming languages, but here within this article, you will well find out that in a sense,  ***HTML***, is actually a **programming language** of some sort with specific functions that when you realize and utilize well, could make your life the lot simpler and easier.  We shall get into a few of those, that I may refer to, with regards to implicit CSS as;

- **1. Computed Markup function of HTML**
- **2.  And Innate Markup function of HTML**

#### 1. Computed Markup Function of HTML:

Let's consider this function of HTML, called, Computed Markup Function of HTML, as ***"CMF"***, I know some of you or most of you may go like -- ***[with a bugs bunny sort of voice], this is,  'new', what happened, where from this term,  or terms or concept. ***
 
Is it made up?

 You bet yeah! : D. 

When you work in isolation things like this ought to be documented regardless of whether you know the right word or not. Who knows? this may well become a globally accepted wording as the term, first coined by yours truly, **moi**, and when you just always have limited access to the internet or time or other resources, you begin to invent and coin terms or create utilities for an even greater invention.

Now let's examine together what this function does and where it often occurs. `CMF` of HTML. Consider the snippet below;

```
<!doctype html>
 <html lang="en">
    <head>
          <title>HTML is an Awesome Markup Language </title>
    </head>
     <body></body>
</html>
``` 

Supposing say we wanted to consider placing a loading animation or a spinner onto our website before any website loads from the body element. And we want to be a bit of clever, we would do this.

```
<!doctype html>
 <html lang="en">
    <head>
          <title>HTML is an Awesome Markup Language </title>
          <!--Our mischievous load spinner-->
           <div class="loader"></div>
    </head>
     <body></body>
</html>
``` 

Placing `<div>` element into a `<head>` element is forbidden, I think, but let's say we go ahead with our mischievous endeavor trying our clever way of achieving the load spinner and keeping our main markup clear of the loader code thats when you will notice HTML `CMF` kick into action.  

This function albeit a bit abstract, organizes HTML elements into the proper way it should be organized when your website runs. So say when you inspect your code after running the latter snippet? The snippet would show up instead of the markup you wrote in the browser.

```
<!doctype html>
 <html lang="en">
    <head>
          <title>HTML is an Awesome Markup Language </title>
    </head>
     <body>
          <!--Our mischievous load spinner-->
           <div class="loader"></div>
      </body>
</html>
``` 

#### 2. Innate Markup function HTML:

Again let's examine another instance where an HTML function runs automatically. This function, I shall refer to as, `IMF` short for `Innate Markup Function` of HTML.  And what it does, is automatically, apply some sensible default CSS style on the HTML elements right at birth. At birth implies when you introduce those element or include those element with your HTML Markup. 

Let's consider the snippet below. In this snippet, we introduce a block element. And what front-end developers sometimes forget when styling or writing CSS for this Element is that it has some innate properties already applied.

```
<!doctype html>
 <html lang="en">
    <head>
          <title>HTML is an Awesome Markup Language </title>
    </head>
     <body>
          <!--Block element introduced or born-->
           <div></div>
      </body>
</html>
``` 

So to style such and element when `IMF` has applied some styles, we need to consider what these properties applied are, perhaps interrogate the element :D . 

-  First, we should ask, ourselves, do we need to add, for example `display:block`? 
No!, As a sensible default, HTML already applied this rule for us on all block elements, Except, we want to do it differently. we may have to just leave it just as it is.

-   Second do we need to add a CSS rule for width? No!, Not always, because, you guessed it, `IMF`, already did it for us.

-  Thirdly, what rules can we apply to such an element if we gave birth to it, and it's were to also now become a parent? :D ... We tell it to stand tall. Yes I mean literally, then all we need to add to it, as CSS rules are maybe `height: 400px` or whatever height we should provide it as support. And to honor it with some color as I have done in the snippet below.

```
<!doctype html>
 <html lang="en">
    <head>
          <title>HTML is an Awesome Markup Language </title>
        <style>
            // Minimal CSS Rule set after considering all the div's elements innate properties
              div {
                 height: 400px;
                 background: pink;
              }
        </style>
    </head>
     <body>
          <!--Block element introduced or born-->
           <div></div>
      </body>
</html>
``` 

This `<div>` is just an example and I know there are a ton of other HTML Elements with bond to `IMFs`, you can research and update this article, I invite you to edit this article with your findings too. I shall make a repo available at https://github.com/huffypiet/implicit-vs-explicit-css-html, please kindly fork and PR if you find anything to update this article. Thanks.


#### Conclusion:

Waiting for that perfect day has instead turned out to be a mirage, I was rather not reaching, any sooner, no matter how long I waited or stayed not trying hard enough to make the change. 

If I were to stay the same, not changing from my old habits constantly and not finding a good rhythm to dance my way to Freedom, Freedom of expression through code, Freedom of association, and the Freedom to be Badass :D by often taking into account all of you, in the  ***Coding, Programming, Tech Community***, at large, and sharing with a whole lot of you, then the mission might turn out to become a great omission.


