---
title: 'What is DNS?'
taxonomy:
    category:
        - docs
visible: true
---

Remember back before everyone had computers that fit in their pocket, how companies would ship a book full of phone numbers to your doorstep? We might have known who we were looking for, but we needed to look up phone numbers unless they were your crazy relatives that you learned to memorize. When you get your own domain name, by default it’s nothing more than a shortcut, an address, or (to fit this very imperfect analogy) a phone number. When you type a domain name into the address bar of your browser, someone has to identify it and tell it what to display. That’s where a name server comes in.

A name server is a computer, running as a server, that keeps a record of all the domain names that are associated with it and keeps track of where those domains should go. In the case of rutgers-sci.domains, the nameserver is the same computer that runs the hosting. You can peek under the hood and see this in action by going to the Websites and Domains tab of your cPanel account and clicking on DNS Settings. DNS stands for Domain Name System and the name server on rutgers-sci.domains gives control to it to identify what should be displayed when someone types in your domain. Consider the fact that you might have one or more [subdomains]() in your account. The name server and DNS are able to identify those subdomains and let the world wide web know that they exist and point to some files/folders on a computer somewhere.

When you signed up for a domain through the rutgers-sci.domains system your nameservers were chosen for you. So when people type in your address, the server responds with information about your account. When you migrate an account away from one hosting platform like rutgers-sci.domains and onto a new service, it will require you to change the nameservers so that your domain name points to a new server with its own files and structure. It’s also possible to have subdomains that point to entirely different servers than rutgers-sci.domains. For example, you could have a subdomain that looks to Tumblr for files.
