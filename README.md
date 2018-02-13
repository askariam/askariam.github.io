## Website Performance Optimization portfolio project

I Accepted the challenge. Please check Part 1 and Part 2. The site rating in the speed insight is better than 90% in both mobile device and computer device.

### Getting started
After downloading the .zip file, extract the content to a folder in your device.
1. Run the site on your local machine.

  ```bash
  $> cd /path/to/your-project-folder
  $> python -m SimpleHTTPServer 8080
  ```
1. Open a browser and visit localhost:8080
1. Download and install [ngrok](https://ngrok.com/) to the top-level of your project directory to make your local server accessible remotely.

    ``` bash
    $> cd /path/to/your-project-folder
    $> ./ngrok http 8080
    ```

1. Copy the public URL ngrok gives you and try running it through PageSpeed Insights!

1. For Part2, you can run the site locally and use developer tools in Google Chrome to inspect the FPS.

#### Part 1: Optimize PageSpeed Insights score for index.html

Optimized the images. Also, changed some js to async and moved some scripts to be executed at the end.

#### Part 2: Optimize Frames per Second in pizza.html

Mainly moved out all the DOM access out of the loops. Also, reduced the number of moving pizzas since this will not impact the view. Also, optimized the time of resizing the pizzas by calculating the new size as percentage.
