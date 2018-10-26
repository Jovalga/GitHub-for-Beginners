#First-Time Git Setup




Your Identity

The first thing you should do when you install Git is to set your user name and email address. This is important because every Git commit uses this information, and it’s immutably baked into the commits you start creating:

	$ git config --global user.name "John Doe"
	$ git config --global user.email johndoe@example.com

Again, you need to do this only once if you pass the --global option, because then Git will always use that information for anything you do on that system. If you want to override this with a different name or email address for specific projects, you can run the command without the --global option when you’re in that project.

Many of the GUI tools will help you do this when you first run them.
Your Editor

Now that your identity is set up, you can configure the default text editor that will be used when Git needs you to type in a message. If not configured, Git uses your system’s default editor.

If you want to use a different text editor, such as Emacs, you can do the following:

	$ git config --global core.editor emacs



Checking Your Settings

If you want to check your configuration settings, you can use the git config --list command to list all the settings Git can find at that point:

	$ git config --list
	user.name=John Doe
	user.email=johndoe@example.com
	color.status=auto
	color.branch=auto
	color.interactive=auto
	color.diff=auto
	...

You may see keys more than once, because Git reads the same key from different files (/etc/gitconfig and ~/.gitconfig, for example). In this case, Git uses the last value for each unique key it sees.

You can also check what Git thinks a specific key’s value is by typing git config <key>:

	$ git config user.name
	John Doe



