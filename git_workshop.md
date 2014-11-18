###Github Tutorial Exercise

###Setup

- First, create an account at [github.com](https://github.com/).
- Next, download the [Sublime text editor](http://www.sublimetext.com/)
- Some of the exercises below will require you to use a text editor, which will get launched automatically from the terminal. Your computer uses something called *environment variables* to store information, including information used when navigating the terminal (your default directory, for example). The current text editor stored in the `EDITOR` environment variable is something super unfriendly (most likley vim, nano, or emacs, which are editors that open up in the terminal and are tricky to navigate). To store sublime in your `EDITOR` variable, first run this in the terminal:

`ln -s "/Applications/Sublime Text 2.app/Contents/SharedSupport/bin/subl" ~/bin/sublime`

which creates a new command in the terminal called `sublime`. When you type `sublime` the Sublime editor will launch.

Next run in the terminal:

`export EDITOR='sublime -w'`

which stores the `sublime` command in your `EDITOR` env variable.

###Github tutorail
These are bare bone notes, with the idea of slimming way down the amount of info you're blasted with. That being said, there are some great tutorials online, that are more in depth.

- [General github tutorial](https://try.github.io/levels/1/challenges/19)
- [Creating a new repo](https://help.github.com/articles/creating-a-new-repository/)
- [Forking a repo](https://help.github.com/articles/fork-a-repo/)
- [Submit a pull request](https://help.github.com/articles/using-pull-requests/)
- [Adding collaborators](https://help.github.com/articles/adding-collaborators-to-a-personal-repository/)

###Make a new repo
- On the github homepage, click the `+` icon in the toolbar and create a new repository.
- Give it a name, a description, make it public, initialize it with a `README`, and add a license.
- To copy the repo to your own computer, copy the clone URL in the righthand sidebar of the repository page (it will end with `.git`), then run in your terminal:

`git clone the_url_you_just_copied`
- Switch directories to your repo, by running `cd name_of_your_repo`
- Check you're in the right place by running `ls`

###Add content
- Make a new file in the repo. You can make a markdown file (ending in `.md`), which is what this tutorial is written in. It's basically a text file with special formatting.
- Save the file.
- Now, you're going to add it to your git repository. The general flow of adding a new file is:
	- `pull` to load any changes to other people have made to your repo
	- `add` the files you've changed to be staged (they're basically on deck)
	- `commit` your changes, lumping all the added files into one update and describing it
	- `push` your changes to the repo
- The actual commands are:
	- `git pull`
	- `git add your_new_file` or `git add -A` to add all changed files
	- `git commit -m "a message describing your changes"`
	- `git push`

###Collaborate!!
- Now partner up, you're going to collaborate on an open source project
- First, fork your partner's repo by clicking `Fork` in the top-right corner of his/her's repo's main page.
- Clone your fork, and navigate to your fork's directory (see "Make a new repo" above for these steps)
- Make some changes to the content!
- On your fork, click the green "compare and review" button to submit a pull request.
- Switch places with your partner

###Build a team
- In your own repo, you can navigate to `Settings` then `Collaborators` to add your partner as a permanent team member. Now he or she can push straight to the repo without having to submit a pull request.
