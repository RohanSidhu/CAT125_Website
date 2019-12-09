---
layout: page-fullwidth
title:  "All About Me"
teaser: "Who am I?"
categories:
    - design
tags:
    - design
    - background color
header:
    title:  
#    pattern: pattern_concrete.jpg
    image_fullwidth: about_me.jpeg
---
I am a student at the University of California, San Diego pursing a Mathematics and Computer Science Degree. After taking my lower division computer science course, I've learned that I am a slow learner and needed other material beside a textbook to teach me information. 

All of the languages that I've learned were Object Oriented, hence I decided to make a website explaining it all! I remember struggling with Java as I had no idea what an object was. My TA's knew me by name because of how much helped I've needed. This website is a miniature guide for individuals who are learning about Object Oriented Programming!

Each of these projects below me all involved Object Oriented Programming! They were super fun when designing and I have learned so much through these projects.

<div class="row">
    <div class="medium-8 columns t30">
    <img src="{{ site.urlimg }}orb.png" alt="">
    </div><!-- /.medium-8.columns -->

    <div class="medium-4 columns t30">
      <img src="{{ site.urlimg }}city.png" alt="">
      <img class="t30" src="{{ site.urlimg }}mickey.png" alt="">
    </div><!-- /.medium-4.columns -->

</div><!-- /.row -->

The first one on the left is called CrazyOrbs! This game allows a user to click on the plane and place these dynamically changing orbs. These orbs change colors, can be moved around, and can shrink/enlarge at different speeds.

The second one is on the right, on the top. This project is about having multiple objects and creating simple pictures with them. This one is a cityscape that uses rectangles, triangles, and circles to create the picture. 

The last one is on the bottom right. This project was fairly simple and one of the one of beginning projects I completed. The user can click on the canvas and it will spawn a mickey silhouette. It is draggable and disappears if the user takes the mouse away from the canvas. 


~~~

---
#
# Use the widgets beneath and the content will be
# inserted automagically in the webpage. To make
# this work, you have to use › layout: frontpage
#
layout: frontpage
header:
  image_fullwidth: header_unsplash_12.jpg
widget1:
  title: "Blog & Portfolio"
  url: 'http://phlow.github.io/feeling-responsive/blog/'
  image: widget-1-302x182.jpg
  text: 'Every good portfolio website has a blog with fresh news, thoughts and develop&shy;ments of your activities. <em>Feeling Responsive</em> offers you a fully functional blog with an archive page to give readers a quick overview of all your posts.'
widget2:
  title: "Why use this theme?"
  url: 'http://phlow.github.io/feeling-responsive/info/'
  text: '<em>Feeling Responsive</em> is heavily customizable.<br/>1. Language-Support :)<br/>2. Optimized for speed and it&#39;s responsive.<br/>3. Built on <a href="http://foundation.zurb.com/">Foundation Framework</a>.<br/>4. Seven different Headers.<br/>5. Customizable navigation, footer,...'
  video: '<a href="#" data-reveal-id="videoModal"><img src="http://phlow.github.io/feeling-responsive/images/start-video-feeling-responsive-302x182.jpg" width="302" height="182" alt=""/></a>'
widget3:
  title: "Download Theme"
  url: 'https://github.com/Phlow/feeling-responsive'
  image: widget-github-303x182.jpg
  text: '<em>Feeling Responsive</em> is free and licensed under a MIT License. Make it your own and start building. Grab the <a href="https://github.com/Phlow/feeling-responsive/tree/bare-bones-version">Bare-Bones-Version</a> for a fresh start or learn how to use it with the <a href="https://github.com/Phlow/feeling-responsive/tree/gh-pages">education-version</a> with sample posts and images. Then tell me via Twitter <a href="http://twitter.com/phlow">@phlow</a>.'
#
# Use the call for action to show a button on the frontpage
#
# To make internal links, just use a permalink like this
# url: /getting-started/
#
# To style the button in different colors, use no value
# to use the main color or success, alert or secondary.
# To change colors see sass/_01_settings_colors.scss
#
callforaction:
  url: https://tinyletter.com/feeling-responsive
  text: Inform me about new updates and features ›
  style: alert
permalink: /index.html
#
# This is a nasty hack to make the navigation highlight
# this page as active in the topbar navigation
#
homepage: true
---

<div id="videoModal" class="reveal-modal large" data-reveal="">
  <div class="flex-video widescreen vimeo" style="display: block;">
    <iframe width="1280" height="720" src="https://www.youtube.com/embed/3b5zCFSmVvU" frameborder="0" allowfullscreen></iframe>
  </div>
  <a class="close-reveal-modal">&#215;</a>
</div>

~~~
