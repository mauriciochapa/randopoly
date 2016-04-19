## Website Performance Optimization portfolio project


To get started and check the PageSpeed, check out the repository or you can run a local server:

  ```bash
  $> cd /path/to/your-project-folder
  $> python -m SimpleHTTPServer 8080
  ```

1. Open a browser and visit localhost:8080
1. Download and install [ngrok](https://ngrok.com/) to make your local server accessible remotely.

  ``` bash
  $> cd /path/to/your-project-folder
  $> ngrok http 8080
  ```

1. Copy the public URL ngrok gives you and try running it through PageSpeed Insights! Optional: [More on integrating ngrok, Grunt and PageSpeed.](http://www.jamescryer.com/2014/06/12/grunt-pagespeed-and-ngrok-locally-testing/)

### Getting started

####Part 1: Optimized PageSpeed Insights score for index.html

Google font was too heavy, so it was removed <br>
Inlined css file <br>
CSS media call print was added <br>
Reduced image size for pizzeria2.jpg<br>
Minified both CSS files


####Part 2: Optimize Frames per Second in pizza.html

For Pizza.html<br>
Optimized CSS by inlining critical CSS as follows and minifying the files<br>
https://developers.google.com/speed/docs/insights/OptimizeCSSDelivery#example <br>
Minified the CSS and JS files

For main.js<br>
optimized JS by takig the variables outside of the for-loops( lines 452, 506) therefore reducing the amount of times we redefined the variables, resulting in less FPS

### Customization with Bootstrap
The portfolio was built on Twitter's <a href="http://getbootstrap.com/">Bootstrap</a> framework. All custom styles are in `dist/css/portfolio.css` in the portfolio repo.

* <a href="http://getbootstrap.com/css/">Bootstrap's CSS Classes</a>
* <a href="http://getbootstrap.com/components/">Bootstrap's Components</a>
