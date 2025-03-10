---
title: 'Static and Dynamic Websites'
taxonomy:
    category:
        - docs
visible: true
---

## Static Websites
In the early days of the Web, almost all Web sites were what is known as 'static sites.' Content (text, images, video, audio, etc), was placed or embedded in a file in which HTML tags were used to format it.

The content and the tags lived side-by-side. To edit the page, you’d open up the file (on your own computer) in a program capable of editing HTML files and make changes to either the content or the presentation. Every page had to be edited individually, even if the edits you were making were for common elements that appeared on many pages (like menu bars).

From a technical perspective, accessing a static Web site is fairly straightforward. When your computer is connected to the Internet, you can use a Web browser to access files on a Web server (as long as you know the address). The Web server delivers the contents of those files to your browser, and your browser displays them.

## Dynamic Websites
Over time, as the Web became more sophisticated, new systems emerged for creating and managing Web sites. These moved beyond the model of having content and HTML tags live in a simple HTML page which your browser accessed and displayed. Instead, these systems were Web applications – software that literally runs on the Web server and makes it possible to manage a Web site, often with very sophisticated features. One feature of these applications is that they separate content and presentation by storing most content (your text, images, etc) and data about the site (the title, options, etc). in a database.

On the Web server, the Web application installs files that are written in some kind of programming language. The server reads this code and obeys any requests in it to access data in the database (which lives on a separate server) and displays it according to the instructions in the code.

Essentially, the data for the site (living in a series of tables in a database on the database server) is entirely separate from the actual presentation of the site (living in the code of the programmed files on the Web server). Special software on both the Web server and the Database server enable the two to speak to each other and work together.

One of the benefits of using a Web application is that you usually don’t need to touch (or even look at!) the code in order to make changes to your content. In addition, editing the site usually involves accessing some kind of control panel through your Web browser and filling out a form, instead of having to download and access files in software on your own computer.

## Dynamic vs Static Content
Sometimes when we talk about the difference between dynamic and static content we get bogged down in the idea of whether or not the content is “fresh” (dynamic, regularly updated) or “old” (static, never updated). How frequently you update your content has nothing to do with what kind of system you are using to manage your site. You can manage a static Web site (as described above) and update the content every day. You can also have a dynamic Web site (running something like WordPress) and never change the content after you create it.

Generally speaking, it is easier to regularly update content on a dynamic Web site because the Web application just makes it easier. Sometimes, even when you just want a very basic page or placeholder, it’s easier to install a Web application (and only put up a single page) then to manually create an HTML page and upload it.

## A Side Note about Separating Content from Presentation: Style Sheets
Another aspect of separating content from presentation involves the use of 'Cascading Style Sheets' (CSS). These are special files that live on your Web server and are linked to your Web pages. They contain information (written in a special markup language) about how to make elements on your site look. For example, they allow you to define in a single location what all Level 1 Headings look like on your site. They are an important aspect of understanding how to separate content from presentation, but they’re not really an aspect of the difference between static and dynamic sites. Both static and dynamic sites can use style sheets.