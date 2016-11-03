Step to run project
Optimization
1. Open https://dohuul.github.io/WebOptimizationProjects/index.html
    + The following optimization was made to index.html to improve loading time
        - Minify all CSS and Javascript files
        - Reduce the Critical Rendering Path from 2 to 1 and reduce the number of critical resource from 5 to 1
            Inline all CSS rules in style.css
            Add media query for print.css
            Asynchronously load the GoogleAnalytic script, and move all JS to bottom of page
            Use Web API to load font
        - Optimize all images by using compression and resize

2. Open https://dohuul.github.io/WebOptimizationProjects/views/pizza.html
    + The following optimization was made to improve resposiveness
        - Improve page FPS close to 60 during scroll
            Refactor update function to remove Forced Synchronous layout
        - Improve page FPS close 60 during pizza resize
            Refactor resize function to remove Forced Synchronous layout

GitHub source
1. https://github.com/dohuul/WebOptimizationProjects/