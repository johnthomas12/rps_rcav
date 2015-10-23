# Rock Paper Scissors

We are going to build a simple game. Users are allowed to choose Rock, Paper, or Scissors by visiting one of the following URLs:

 - [http://localhost:3000/rock](http://localhost:3000/rock)
 - [http://localhost:3000/paper](http://localhost:3000/paper)
 - [http://localhost:3000/scissors](http://localhost:3000/scissors)

And we will tell them whether they won or lost. Your target, in the end, is this:

https://rps-rcav-target.herokuapp.com

### Setup

 - First **fork**, and *then* clone.
 - `cd` to the root folder of the application.
 - `bundle install` (or just `bundle` for short).
 - `rails server` (or just `rails s` for short).
 - Once the server has booted up successfully, visit [http://localhost:3000](http://localhost:3000) in Chrome. If all went well, you should see the "Welcome Aboard" page.
 - Open up the entire folder of code in Sublime (on Windows, **File → Open Folder...**; on Mac, you can select a folder using the usual **File → Open...** dialog).

### Part 1

This is currently a brand new Rails app, with absolutely no routes, controllers, etc.

Add support for [each](http://localhost:3000/rock) [of](http://localhost:3000/paper) [our](http://localhost:3000/scissors) three URLs one at a time. For each one,

 1. Complete the [RCAV](https://gist.github.com/rbetina/c200d88adcfe0d4dcd04) and display "Hi!" to prove that you did so. Make up whatever names you want for the controller and action.
 1. Now step back into the action and write some logic to determine whether the player won or lost. Put the computer move and the outcome into instance variables.
 1. In the view template, display the instance variables. Format it a little with some markup and some copy.

### Part 2

Once you have completed the above for all three URLs,

 1. On each page, add links to get to the other two pages (so that our users don't have to keep typing into the address bar).
 1. I dropped three images in the `public/assets/images` folder: `rock.png`, `paper.png`, and `scissors.png`. Therefore, they are available to use (e.g., as the `src=""` of `<img>`s) at [http://localhost:3000/assets/images/rock.png](http://localhost:3000/assets/images/rock.png), etc. Use the images on your pages as you see fit.
 1. I also dropped `bootstrap.css` in the `public/assets/css` folder. `<link>` to it in `app/views/layouts/application.html.erb`, and use Bootstrap styles to make everything look nicer.
 1. Add a root URL such that visiting the bare domain, [http://localhost:3000](http://localhost:3000), defaults to playing rock.
