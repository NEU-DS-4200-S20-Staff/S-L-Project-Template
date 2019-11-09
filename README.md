# S-L Project Template

This template will help you get started with your project. Please look through all these materials so you know how to organize your project.

## The Associated GitHub Pages Website

This web page is served automatically from the default `gh-pages` branch at https://northeastern-ds-4200-f19-staff.github.io/S-L-Project-Template/

## Setup

**Under no circumstances should you be editing files via the GitHub user interface.** Do all your edits locally after cloning the repository.

1. Clone this repository to your local machine. E.g., in your terminal / command prompt `CD` to where you want this the folder for this activity to be. Then run `git clone <YOUR_REPO_URL>`

1. In `README.md` update the URL above to point to your GitHub pages website. E.g., http://northeastern-ds-4200-f19.github.io/project-team-#-topic where `#` and `topic` are customized.

1. `CD` or open a terminal / command prompt window into the cloned folder.

1. Start a simple python webserver. E.g., one of these commands:
    * `python -m http.server 8000`
    * `python3 -m http.server 8000`
    * `py -m http.server 8000`
    If you are using Python 2 you will need to use `python -m SimpleHTTPServer 8000` instead, but please switch to Python 3 as [Python 2 will be sunset on 2020.01.01](https://www.python.org/doc/sunset-python-2/).

1. Wait for the output: `Serving HTTP on 0.0.0.0 port 8000 (http://0.0.0.0:8000/)`

1. Now open your web browser (Firefox or Chrome) and navigate to the URL: http://localhost:8000

## Root Files
* `README.md` is this explanatory file for the repo.

* `index.html` contains the main website content. It includes comments surrounded by `<!--` and `-->` to help guide you through making your edits.

* `style.css` contains the CSS.

* `LICENCE` is your source code license.

## Folders
Each folder has an explanatory `README.md` file

* `data` is where you will put your data files.

* `favicons` contains the favicons for the course projects. You shouldn't change anything here.

* `files` will contain your slides (PDF) and video (MP4).

* `images` will contain your screenshots, diagrams, and photos.

* `js` will contain all JavaScript files you write.

  * `visualization.js` is the main code that builds all your visualizations. Each visualization should be built following the [Reusable Chart model](https://bost.ocks.org/mike/chart/)
  
* `lib` will contain any JavaScript library you use. It currently includes D3.

## Workflow

As you work with your team, you may have issues merging your changes. We recommend you pick one member of the team to be the project manager and deal with merging any pull requests.

Instead of all working directly out of the main `gh-pages` branch, you can try adopting a Git branching model for development. See, e.g., [this article by Vincent Driessen](https://nvie.com/posts/a-successful-git-branching-model/) and the included image:

![Image of Git branching model by VIncent Driessen](http://www.ccs.neu.edu/home/cody/courses/shared/git-model.png)

## Grading

Make sure to check these aspects of your work, which are important for every submission:

* Coding was done properly:
    * Your code was regularly committed and not edited via the GitHub user interface online.
    * You have clear, commented, and validated code.
    * Your web page loads properly and looks as expected in the latest Firefox and Chrome browsers.
    * Any code from other sources (modified or copied straight) is acknowledged.

* Your visualization works as required:
    * Styles are consistent across views.
    * None of the visualizations change size or move on the screen as you interact with them.
    
## Template Repository Setup (For Instructors)

### GitHub Pages

It is necessary if using GitHub Classroom to set up GitHub pages for the students, as they do not have admin permissions on their repository. To do this, we need to create and move everything to the `gh-pages` branch and delete the `master` branch.

1. Commit the files to the `master` branch on GitHub.

1. `git branch gh-pages`

1. `git checkout gh-pages`

1. `git branch -D master`

1. `git push origin gh-pages`

1. On GitHub, go to `Settings`->`Branches` and set the default branch to `gh-pages`.

1. `git push origin :master`

### Template Repository

1. On GitHub, go to `Settings` and check the box for `Template repository` at the top. This makes GitHub Classroom copies much faster.