## Website Performance Optimization portfolio project
To achieve the > 90/100 Pagespeed insights score of the given website: Cameron's profilo, optimizations for improvement were performed on index.html, style.css and images.
Index.html optimizations:
1. optimize images: by compressing and resizing images(profilepic.jpg and pizzeria-mini.jpg).
2. eliminate render blocking javascript and css: media query print.css, inline and minification of critical css and asynchronous parse blocking script.
3. avoiding landing page redirects: dicet images from sub-folder of the web site.  
To speed the frame per second rate up to 60fps while scrolling the pizza page, view/js/main.js were modified.
view/js/main.js optimizations:
1. move the var and redundant calculation outside the loop to reduce the unnecessary calculations.
2. updatePositions function (moves the backgound slidings based on the last position while scrolling): used style.transform and translateX(), calculate each sliding pizza's translate x position instead of additional compute left property every time.
3. The number of sliding pizzas in the background were reduced from 200 to 3(rows)*8(cols). 
and add backface-visibiligy to hidden to avoid repainting background .

Github link  http://ontheplanet.github.io/project4/
Github host link  https://github.com/ontheplanet/project4/

references:
https://developers.google.com/web/fundamentals/
http://www.html5rocks.com/en/tutorials/speed/high-performance-animations 
http://www.html5rocks.com/en/tutorials/speed/layers/
http://www.html5rocks.com/en/tutorials/speed/rendering/
http://www.feedthebot.com/pagespeed/critical-render-path.html
http://www.paulirish.com/2012/why-moving-elements-with-translate-is-better-than-posabs-topleft/


