<img class="toprightimg" src="http://cdn.flaticon.com/png/256/25231.png"/>


Throughout this course we'll use <strong>Git</strong> for version control, and <strong>Github</strong> as a platform for both collaboration and publication. LNU has a [good primer](https://coursepress.lnu.se/info/manual/kom-igang-med-github/) on Git, in Swedish.

For those of you who don't speak Swedish, here is a quick primer on the usage in the RIA course:

*    Install Git on your computer (you can test if you have it by typing `git --version` in the terminal)
*    Create an account on Github if you haven't already done so
*    Install a GUI if you don't want to work from the terminal. The main clients are [Github for Mac](https://mac.github.com) or [Github for Windows](https://windows.github.com).
*    Create a repository for this course. The repository must be public.
*    Create a folder on your computer for the course project.
*    Navigate to that folder and type `git init`
*    Create and switch to a branch named gh-pages by running `git checkout -b gh-pages`
*    Connect the folder to the repository on Github by running `git remote add origin git@github.com:<gituser>/<reponame>.git`, exchanging `<gituser>` and `<reponame>` for your user name and repository name respectively.

Since we're using the "magical" branch name gh-pages, your app will be published at `http://<gituser>.github.io/<reponame>`.

Throughout the course you will be forking other people's repositories, and also receive pull requests to your own repo as others are helping you out.

You can score bonus points by using more advanced Git and Github functionality, such as:

*    creating feature-specific branches where you work on new functionaloity, which is then merged back into the main gh-pages branch when (or if) it is finished
*    use issues on Github for project management (this will also help others to help you)
*    use labels for issues and pull requests
*    assign issues to users
*    sort issues and commits with milestones