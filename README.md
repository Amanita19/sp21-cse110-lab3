This is to be completed as a solo assignment.

The previous lab assignment had you creating a GitHub User Page using Markdown. For this week’s lab assignment, you’ll be exploring the basics of HTML and Chrome DevTools. The purpose of the first part of this lab is to get you familiar with the basics of HTML, as well as some of the lesser known parts. Your primary goal will be to explore and practice correct syntax and usage of tags, properties, links, etc. over visual execution. The second part of this lab will acquaint you with the Chrome DevTools by going on a scavenger hunt through a site that we’ve set up to find some hidden secrets. You may technically use any browsers’ DevTools for this section, but this lab will be written with Chrome DevTools in mind.

 

### **Resources**

[HTML Basics (Links to an external site.)](https://www.freecodecamp.org/news/html-basics-for-beginners/)

[Mozilla Developer Network (MDN) (Links to an external site.)](https://developer.mozilla.org/en-US/docs/Web/HTML/Element)

[Official HTML Specification (Links to an external site.)](https://html.spec.whatwg.org/)

 

### **Set Up**

1. [Fork (Links to an external site.)](https://docs.github.com/en/github/getting-started-with-github/fork-a-repo) the starter repository for Lab 2 here: [https://github.com/CSE110-SP21/Lab2 (Links to an external site.)](https://github.com/CSE110-SP21/Lab2) (only follow the tutorial through step 2. You don't need to sync your repo with the starter repo).
2. You might find the VSCode extension [LiveServer (Links to an external site.)](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer) useful for this and future labs. You can use this to open your html file while editing and see live changes.

 

### **Part 1. Intro to HTML - Journal Entries**

In this section, you will be building a simple webpage outlining journal entries for the past 3 days. When building this out, your site must use valid semantic and structural HTML. You should be handcrafting your site and **not using**[ Cascading Style Sheets (CSS) (Links to an external site.)](https://developer.mozilla.org/en-US/docs/Learn/CSS/First_steps/What_is_CSS),[ JavaScript (JS) (Links to an external site.)](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/First_steps/What_is_JavaScript), or any [frameworks (Links to an external site.)](https://developer.mozilla.org/en-US/docs/Learn/Server-side/First_steps/Web_frameworks). Don't worry if you haven't used HTML, CSS, or JS before; use the links from the **Resources** section above and the web to your advantage. 

**What do we mean by journal entries?** We do not care so much about how your entry looks visually since this is just a markup lab where styling with CSS or JS is strictly prohibited. You are to create 3 journal entries: One for 2 days ago, one for yesterday, and one for today. The content of these entries truly does not matter as long as they are appropriate and you use the markup correctly, but here are some ideas if you need some inspiration: 

- most journals have an overall **title**, then **subtitles** for each day and usually the **date** for that specific journal entry
- **list** of highlights and lowlights of the day
- **list** of things that needs to be done
- **paragraph** to vent about things you need to get off your chest
- **picture** of something you found interesting that day, or a funny meme
- **audio** recording of your favorite song, or a voice memo you recorded
- **video** of perhaps you and your friends or something you neat you found on a walk

### Creating an HTML Document

Here is a simple basic skeleton for you to start off your HTML document with.

```
<!DOCTYPE html>
<html lang=”en”>
    <head>
    </head>
    <body>
    </body>
</html>
```

**Key Terms:**

1. **<!DOCTYPE html>** : all HTML documents must start with a document type declaration
2. **<html lang="en"></html>** : the HTML document starts and ends with the <html> element, also known as the root element. The *lang* attribute declares the language of the page.
3. **<head></head>** : contains the document metadata, which is not displayed to the users.
4. **<body></body>** : contains the content of the page that is visible to users.

 

### Common Useful HTML Elements

Your website needs to include **at least one of each of the following HTML elements -- one of each that are explicitly listed, not just one from each section** (you are allowed to use other elements not listed here as well).

Note that you must use these elements properly on top of them being valid, such as making sure that your header element goes at the top of your page and similarly making sure that your footer element goes at the bottom of your page. Be creative with your usage of the elements to make this exercise more enjoyable. 

 

*Document metadata*

Metadata elements are not rendered to your webpage, rather they are used by the browser to provide extra information to your webpage like a title and icon in the browser tab bar or a description of your website

- title
- meta
- link (usually <link> is used to link a stylesheet, but since we're not using CSS, you can use it to link a favicon instead)

 

*Content sectioning*

Sectioning tags are necessary for your browser to correctly understand the structure of your webpage. Correct webpage sectioning helps in areas like Search Engine Optimization. Note that the way that you section your webpage does NOT have to be exactly how the webpage is structured visually, rather think of your section elements as a guide to your web browser on how your page should be interpreted.

- main
- header, footer
- nav
- h1, h2, h3
- section

 

*Text content*

Text elements help you format your text content allowing you to add styles and structure to how your text is rendered to the screen. A lot of these elements will produce the same effect visually, however remember that we are writing our HTML for the web browser so make sure to check out the Mozilla documentation to understand when to use each element. Your visual aesthetic can be developed using CSS - but we won't be using CSS for this lab :)

- div, span (these elements may not be too useful without CSS / JavaScript, but are too important to leave out, so just include them somewhere in your document. It’s okay if they aren’t useful)
- hr
- p
- ul
- ol
- li

 

*Inline text semantics*

Inline text elements are used inline with your text to provide meaning to specific parts of a text section.

- b
- strong (know the differences between b vs. strong)
- i
- em (know the differences between i vs. em)
- a
- br

 

*Images and multimedia*

- img
- audio
- video

 

*Interactive Elements*

Interactive elements provides your webpage with some basic interactive functionality without the use of Javascript. 

- details
- summary