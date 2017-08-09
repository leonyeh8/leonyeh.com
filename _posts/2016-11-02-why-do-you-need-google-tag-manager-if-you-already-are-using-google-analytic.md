---
layout: post-sidebar
date: 2016-11-02 00:00:00
categories:
  - business
author_name: Leon Yeh
author_url: /author/leon-yeh
author_avatar: leonyeh
show_avatar: true
feature_image: /img/post-assets/searching.jpg
read: 15
show_related_posts: false
square_related: recommend-san-fran
social-message: Great post over at Writer Theme - You dont have to be great to get started
---


Google Analytics' main job is really just generating the reports and statistics about your website, like how many people saw your website yesterday, what web browser they used, which pages were the most popular etc. The only way it can know this stuff is if you put a "tag" on all of your pages. The tag is the javascript code on your pages that runs on the visitor's browser, which tells Google Analytics' servers that they are visiting the page right now.

There's no problem if you just want to put the tag in the master file of your website so it shows up on all of your pages. Google Analytics can use the "referrer" parameter to figure out which page the visitor is on and can do all the simple stuff like counting page views.

However, you may want to track how many people use a specific feature. Maybe you want to group certain pages together, or count some similar but different URLs as being the same page. Now you need unique tags for all these different features and groups of pages so Google can identify which feature or type of page got used or visited. Now it's complicated! You have multiple tags, and you only want the tags to "fire" sometimes (e.g. don't fire unless they click this button or use this feature.)

Google Tag Manager makes it easier to manage this mess of tags by letting you define rules for when your tags should fire. It also lets you test your tags to make sure they go off when you load the right page or click a certain button. This is done by putting the Tag Manager's code on your website instead of the actual tags, and as Crayon's answer points out, the tag manager outputs the tags for you. This gives you another cool benefit: you can change your tags and the way they work without actually changing the source code of your website (which you may not be able to do because of slow release cycles) – instead you just change it from the Google Tag Manager website, and it will spit out different code on your pages dynamically when they're loaded in the visitor's browser.