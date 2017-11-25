## Udacity Website Performance Optimization portfolio project

Getting started:
* Clone the reposittory and launch an HTTP server. This can be acheived by:

* NPM package http server (npm install-i http-server)
* Invoke [http-server] form the project

#### Optimized Page Speed Scores to 96 for Mobile and 98 Desktop and an FPS average of 58-60 by:
* Minified CSS and js files
* Inline style.css in index.html
* Added async to js and moved down
* Reduced pizza jpg size using resource in pagespeed insights
* Added system fonts instead of web fonts
* reduced FPS 
* Changed [document.querySelector] to [document .getElementById] for faster performance
* Removed leading #'s when using js API call
* Moved newwidth and dx variables out of the loop
* Created a local variable to save [document.getElementsByClassName('randomPizzaContainer') outside the loop (e.g. var container = document.getElementsByClassName('randomPizzaContainer'))], so the DOM is not explicitly touched in every iteration
* Declared the [pizzaDiv] outside the loop on only 1 DOM call is made
* Declared the phase variable [var phase;] in the initialisation of the for loop will prevent it from being created every time the loop is executed 
* Declared the elem variable [var elem;] in the initialisation of the for-loop will prevent it from being created every time the loop is executed 


### References used:
* https://developer.mozilla.org/en-US/docs/Web/API/Document/getElementById
* https://css-tricks.com/snippets/css/basics-of-google-font-api/ 
* https://github.com/typekit/webfontloader
* https://developer.mozilla.org/en-US/docs/Web/HTML/Element/link 
* https://developer.mozilla.org/en-US/docs/Web/HTML/Element/script
* Udacity discussion forums' for help and feedback 
