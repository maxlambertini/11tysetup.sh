# 11tysetup.sh

An [Eleventy](https://11ty.dev) site bootstrapper

## What is it? 

`11tysetup.sh` is an humble bash script that bootstraps an Eleventy site. It performs the following tasks:

- Creates a working directory tree
- Installs [Eleventy](https://11ty.dev) and a lot of accessories from npm
- Creates the skeleton of a working site with some styling
- Creates 20 random blog posts by invoking https://fakedown.xoxarle.com/eleventy-post 20 times
- Creates a random color scheme (three dark colors and three light colors. End result might be yucky. _You have been warned._)

However, [the end result](https://11tysetupsh.netlify.app/) is a responsive, complete mockup of a site that scores 400 points on [Google Page Speed Insight](https://web.dev/measure/)

## Requirements

Its only requirement is an Un\*x-y system using bash as its shell interpreter. This means that Linux and Mac users can deploy and use this script right away, while Windows users need to configure WSL to use it properly (this script has been developed and tested on Ubuntu on Windows, so Windows users, fear not.)

## Installation

- Download the script. 
- `chmod +x 11tysetup.sh`
- copy it in a folder included in your `PATH`. FWIW, I use `~/bin` and I include `$HOME/bin` in my path. 

## Using the script

Create a project directory

`$ mkdir ~/web/my-eleventy-site`

Go into it

`$ cd ~/web/my-eleventy-site`

Launch the script (be sure to be connected to the internet)

`$ 11tysetup.sh`

When it's over, launch `eleventy` in development server mode

`$ eleventy --serve`

Navigate to your site:

`http//localhost:8080`

Download the script and put 

## Inspiration

This script is a (very) partial instrumentation of [Learn Eleventy From Scratch](https://learneleventyfromscratch.com/) course. 

However, with the exceptiopn of CSS Reset and two partials, the remainder of the code is completely original (albeit heavily inspired from the aforementioned course.)

## Where next? 

The script lacks SASS and Gulp capabilities. 

## License

This code is put under the WTFPL. License text can be found [here](LICENSE.txt)

