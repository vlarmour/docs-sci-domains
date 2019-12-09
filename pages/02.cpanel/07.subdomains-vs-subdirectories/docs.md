---
title: 'Subdomains vs Subdirectories'
taxonomy:
    category:
        - docs
visible: true
---

When you’re first getting started with a new space on a new Web host, you might think of yourself as owning a small “territory” of the Web. Everything you place in your public folder on the server becomes available for anyone on the Web to see (assuming they know the address of your site and the files you’ve placed there).

If you’re just putting up a handful of static, HTML pages which you want to make available to colleagues, friends, or family by sending them links, then working with this large, unorganized space may work. But as soon as you get to the point where you want to organize your site, you’re going to need a new strategy.

Consider this scenario: you want to have a personal blog on your new Web space, where you share pictures and short written pieces with family, friends, and colleagues. In addition, you’re working on a large research project that requires you to build a Web-based repository of digital images related to your discipline. You want to use one application (say, [WordPress](http://wordpress.org/)) to manage your personal blog. For your research project, you’ve settled on another open-source application (Say, [Omeka](http://omeka.org/)). Both of these are applications that need to be installed on your Web host, but you can’t just put them both at your main domain name – if you did, both sites would quickly experience conflicts and errors. You need to cordon off separate spaces for your different Web “properties.”

There are two primary strategies for parceling up your Web space. You can create **subdomains** or **subdirectories**. But before you can understand the difference, you need to first understand what we mean when we talk about your root domain.

## Root Domain
Let’s say you’ve registered a new domain for rutgers-sci.domains called blog.rutgers-sci.domains. Anything that is stored at this core URL is considered to be at the **root** of your domain. Nothing comes before the address or after the address. You can certainly decide that you simply want to have a single site on your Web host (say a blog running WordPress), and you can set that blog up at your domain’s root. To get to your site in this scenario, users would simply go to blog.rutgers-sci.domains.

## Subdomains
When you want to do more than just have a single site at the root of your site, you need to decide now to organize your space. One way to do so is by setting up subdomains.

You’re may already be familiar with the concept of subdomains, even if you don’t know it. Consider Google’s website at https://google.com. As you browse features of that site, you’ll notice that the domain changes. When you’re looking at your Gmail account, for example, the domain changes to https://mail.google.com. Now the root of the url is mail.google.com, indicating that you’re on the part of the site that is dedicated to Google’s mail services.

In this instance, mail.google.com is a subdomain that provides a different utility than google.com. The domains serve two purposes: they help to organize the site from a technical perspective, but they also serve as indications to the users that they are in a new/different space.

As you work on your site, you’re welcome to create as many subdomains as you like, and in each subdomain you can actually create a distinct, individual Web site.

## Subdirectories
The alternative for organizing your space is to simply set up subdirectories. These function much like file folders on your computer. Instead of creating a blog at blog.yourdomain.com you would place it in a subdirectory called “blog” making the address yourdomain.com/blog. Setting up subdirectory is really easy. You can create folders on the fly when installing applications (like WordPress), and you can also manually create them in your file browser.

There is one particular issue you need to be aware of: Let’s say you’ve installed WordPress to be your primary blog at yourdomain.com. Later, you decide you want to install WordPress again for a separate image gallery site, and you want to place it at yourdomain.com/gallery. But, if for some reason you’ve already created a page on your WordPress site called “Gallery” then the url yourdomain.com/gallery will already be taken. If you try to create a subdirectory of the same name, you’ll get a conflict and errors.

## Tips & Review
* **Subdomains** are generally a cleaner, more elegant solution to organizing your site. You’re less likely to get conflicts or errors. However, when using subdomains the process is slightly more complicated: You must create subdomains first before you can install anything in them.
* **Subdirectories** don’t create as pretty URLs as subdomains, but they’re easier to set up. They can, however, result in conflicts with existing Web pages.
* As soon as you create subdomains or subdirectories to organize your site, you need to consider how people are going to find them. If you’ve created a new primary blog at **blog.yourdomain.com**, and someone goes to just **yourdomain.com**, they won’t see that new site. It is possible to set up **redirects** to avoid this issue. You can also always create links from pages on one subdomain of your site to another.
* If you really just need one site, sometimes installing at the root of your domain is the easiest thing to do, at least as you’re getting started. You can always add more pieces to your territory later with either subdomains or subdirectories.