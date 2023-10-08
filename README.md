# Git Collaboration Practice - Cafe Delight Website

Let's practice working together in Git. I need help creating a splash page for a local cafe. Here are a couple tasks that need to get one

* In the **index.html** file, add a section named _specials_ between the _about_ and _menu_ sections. In the _specials_ section, replace the content in the `<p>` tag to let people know about a BOGO deal on scones

* In the **style.css** file, change the `body` background color to value to `#f0e6f7`. Also change the `header` and `footer` `background-color` values to `#7d5e93`

## Getting the Repo to a Local Machine
1. Click the green **Code** button on this repository in GitHub
2. Copy either the HTTP or the SSH link (SSH is preferred)
3. In your machine, open the terminal and `cd` into the directory where you usually create projects
4. Run the following command to download the repository from GitHub onto your machine: `git clone <LINK-YOU-COPIED>`
5. Open the cloned folder in VS Code and make changes to the codebase according to your assigned issue.

## Creating & Working with Branches
Projects that use git for version control often have a similar structure.
* There is a **main** branch. This is the most "sacred" part of our codebase. In the case of a website, the **main** branch is what is deployed and is what users interact with. 
* There is a **dev** branch. This is a branch for developers to test new feature and fix bugs without affecting the user's experience.
* The **dev** branch will have branches within it so that developers can work on issues without stepping on each other's toes. Naming conventions for these branches vary, but they typically follow a formula of **category/short-description** e.g. **feature/add-contact-form** 

For our project, you'll need to start by creating a branch off of the **dev** branch. 
1. First, make sure that you are in the **dev** branch. Run `git checkout dev` to move into the **dev** branch from **main**. 
2. Once you're in the **dev** branch, run `git checkout -b <NEW BRANCH> dev` to create a new branch from the **dev** branch. 

If you're working on the .html, name your branch `feature/add-specials-section`. If you're working on the .css, name your branch `fix/make-site-purple`

Make changes to the codebase in your branch. Once you have made your changes, it's time to push your code.

## Pushing Your Code
1. Make sure your work is saved. In the terminal, run `git add .`. This "stages" all the changed files in your project, which let's GitHub know that you are wanting to upload changes to the codebase
2. Run `git commit -m "<COMMIT MESSAGE>"`. This is where you "commit" to the code changes you make. We also include a commit message that describes what changes we made to the code.
3. Run `git push origin <BRANCH NAME>` to upload your code to GitHub
4. In GitHub, open a pull request (PR) either by pressing the green button that appears on the repo page after pushing your code or through the "Pull Request" tab. 
5. After submitting a PR, your code will be reviewed and pulled, edited as necessary, and "pulled" into the **dev** and **main** branches.

### Congrats on a successful PR!