Website Performance Optimization portfolio project

###Setting up Project:
#######  I installed node.js and gulp than re-organised the project folder so all the original HTML/CSS/JavaScript/images is in the 'Dev' folder. The system set up in a way that if I start gulp it will start a listener and will compress any element changed in the 'Dev' folder and move it in the right place in the project folder. <br/>Check ['Dev'](https://github.com/DevRob/Udacity-WebDev-project4/tree/master/Dev) folder for commented readable codes.

###Part 1: Optimize index.html

* removed render-blocking stylesheets by inlining it in HTML.
* async-ed JavaScripts.
* compressed images.
* [Hosted portfolio page on GitHub to analyse](http://devrob.github.io/Udacity-WebDev-project4)

###Part 2: Optimize pizza.html

* gulpfile.js contains gulp script to compress HTML/CSS/JS/images. (excluded node-modules folder from push due size and long filename issues, but I listed the plugins I used below.)
* moved variables out of for loops and saved array lengths, in a local variable, which are part of the condition statement.
* reduced the number of generated "flying pizzas" from 200 to 40
* moved style for '.mover class' to style.css and replaced
* Web API call tweak "document.getElementsByClassName()"
* [link for Pizza.html](http://devrob.github.io/Udacity-WebDev-project4/pizza.html)
* minified main.js ans style.css for pizza html(only in gh-pages branch)<br/>see comments and code style in ➤ [master/views](https://github.com/DevRob/Udacity-WebDev-project4/tree/master/views)
* Link for [Pizza.html](http://devrob.github.io/Udacity-WebDev-project4/views/pizza.html)

###Resources and tools I used:

* [Gulp plugins](http://gulpjs.com/plugins/)
    * [compress images with gulp-imagemin](https://www.npmjs.com/package/gulp-imagemin)
    * [compress javascript with gulp-uglify](https://www.npmjs.com/package/gulp-uglify/)
    * [compress CSS with gulp-minify-css](https://www.npmjs.com/package/gulp-minify-css)
    * [compress HTML with gulp-minify-html](https://www.npmjs.com/package/gulp-minify-html)
    * [pipe exeption handler gulp-plumber](https://www.npmjs.com/package/gulp-plumber)
    * [reload page upon change gulp-livereload](https://www.npmjs.com/package/gulp-livereload)

* [Google Dev PageSpeed Insights](https://developers.google.com/speed/pagespeed/insights)
* [Udacity Office Hours: P4 and Nanodegree Program Questions](https://plus.google.com/u/0/events/comnga3cdvrpkjm7dvb4l71ph2o)
* [Online image compressor](http://compresspng.com)
* [piazza Front-End Web Dev Nanodegree forum](https://piazza.com/class/i36sqlrb9xu332)
* [Udacity  Website Performance Optimization](https://www.youtube.com/watch?v=GNAENzKdciQ&list=PLAwxTw4SYaPmKmNX-INgcxQWf30KuWa_A)
* [Dev Tools](https://developer.chrome.com/devtools/docs/rendering-settings)
* [Timeline feature](https://developer.chrome.com/devtools/docs/timeline)


####Helpful links provided:
* [Chrome Dev Tools tips-and-tricks](https://developer.chrome.com/devtools/docs/tips-and-tricks).
* [Optimizing Performance](https://developers.google.com/web/fundamentals/performance/ "web performance")
* [Analyzing the Critical Rendering Path](https://developers.google.com/web/fundamentals/performance/critical-rendering-path/analyzing-crp.html "analyzing crp")
* [Optimizing the Critical Rendering Path](https://developers.google.com/web/fundamentals/performance/critical-rendering-path/optimizing-critical-rendering-path.html "optimize the crp!")
* [Avoiding Rendering Blocking CSS](https://developers.google.com/web/fundamentals/performance/critical-rendering-path/render-blocking-css.html "render blocking css")
* [Optimizing JavaScript](https://developers.google.com/web/fundamentals/performance/critical-rendering-path/adding-interactivity-with-javascript.html "javascript")
* [Measuring with Navigation Timing](https://developers.google.com/web/fundamentals/performance/critical-rendering-path/measure-crp.html "nav timing api").
* <a href="https://developers.google.com/web/fundamentals/performance/optimizing-content-efficiency/eliminate-downloads.html">The fewer the downloads, the better</a>
* <a href="https://developers.google.com/web/fundamentals/performance/optimizing-content-efficiency/optimize-encoding-and-transfer.html">Reduce the size of text</a>
* <a href="https://developers.google.com/web/fundamentals/performance/optimizing-content-efficiency/image-optimization.html">Optimize images</a>
* <a href="https://developers.google.com/web/fundamentals/performance/optimizing-content-efficiency/http-caching.html">HTTP caching</a>
