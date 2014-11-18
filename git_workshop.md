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

###Make a new repo
- On the github homepage, click the `+` icon in the toolbar and create a new repository.
- Give it a name, a description, make it public, initialize it with a `README`, and add a license.


