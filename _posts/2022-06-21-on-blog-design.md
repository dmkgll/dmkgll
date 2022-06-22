---
layout: default
title: On blog design
permalink: obd
---

Keeo in mind that these are really notes for myself. I'm not saying they are exhaustive or exclusive. Do what you want.

### Content

"The drama belongs in what you say, not the typeface". Ogilvy, D (1983), Ogilvy on Advertising.

Nobody really cares that much about your design. They want something good to read. Andy Weir serialized *The Martian* before it became an international bestseller on a plain HTML blog. 

### Graceful degradation

The site——or rather, the *blog* should be useable even if CSS and Javascript are disabled. See [Eric S. Raymond](http://www.catb.org/~esr/site-design.html) on this. The idea is that your content looks great in unstyled HTML first, and then you build up from that with your styling. This isn't actually hard to do, but very few sites do it.

### Speed

If it slows your site down, it's probably a bad idea. Clicking through normal posts and pages should be instant on any internet connection.

### Underlined links

It's not just an accessibility thing (my colorblind friend finds it so annoying to go to websites that don't underline links), it's just good practice. 

### Narrow content

See [Paul Graham's](http://www.paulgraham.com/gfaq.html) RAQ. "The aim of web design is not to use all available screen space. It is legibility. Text is most legible with no more than 70 characters per line."

### Short urls

URLS should be short, memorable, and follow a predictable schema. They should NOT be pumped full of keywords and run 10 words and dashes long. <code>dmkgll.com/about</code> is much better than <code>dmkgll.com/2022/12/05/about-dmkgll.com</code>.

### Link resilience

I don't quite know what the most practical way to handle this is, but links off your site should be live links. Maybe the best way is to try to always link to an Internet Archive version of the site you want to reference.





