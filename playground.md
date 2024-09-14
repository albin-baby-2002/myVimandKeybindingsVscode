Modes

Before we go ahead and open Vim up for her maiden voyage we must talk about modes. Modes, in my opinion, are the real genius of Vim, especially for coding purposes. There are a number of Modes in Vim, but I’ll highlight the most important (you’ll use them 99.9% of the time) ones below.

It’s well known that code is read more than it is written and/or changed. So why then are most IDEs always in “edit” mode. That is, when you type letters on your keyboard they are spit out wherever your cursor currently happens to be.

Not in Vim. In Vim when you fire it up you’ll find yourself in something called Normal Mode.
Normal Mode

This is where you’ll spend most of your time. This is where you will read code and navigate files. Since in Normal Mode you aren’t editing text, we are now free to use all the keys on the keyboard to navigate text. This is Vim’s secret-sauce. More about navigating below.
Insert Mode

Insert Mode is entered whenever you’re ready to edit text. There are a few ways to enter Insert Mode which we’ll walk through later in this post. The main thing to remember is you’ll only want to enter Insert Mode when you want to change text, and you’ll want to leave it as soon as you’re finished editing. This is because you lose your ability to navigate efficiently whilst in Insert Mode.
Visual Mode

Visual Mode is probably used a little less than the first two modes mentioned, but can still be extremely useful. It’s mostly used to highlight blocks of text, and then perform a command on the entire block. For example, you maybe highlight a block and indent the entire thing.
ing.
Command Mode

Commands are essential for Vim, and will be used heavily, especially when we get to plugins. Commands, as we’ll see, make Vim do something. To enter a command you simply type : while in Normal Mode and then the command.
Opening NeoVim

Once you’ve got NeoVim installed you can launch it by typing:

nvim

I’ve aliased it in my terminal (I use iTerm2 and Z shell btw):

alias n="nvim"

Then you can launch NeoVim by simply typing n in your terminal. Imagine that?? One character and BOOM your (soon-to-be) IDE is good to go. You’ll notice that Vim launches near instantaneously. That’s a user-experience that just can’t be matched by IntelliJ, or even VS Code which is much lighter and speedier than IntelliJ.

To open a file in Vim, it’s as easy as putting the file name (or path to the file) after the command. For example:

nvim my_file.txt

If you omit a filename Vim will open up in whatever your present working directory is, but you won’t see anything just yet.
Closing Vim

There’s an old adage:

    How do you make a random-string generator?
    Open Vim and ask a non-Vim user to close it.

Or something like that. It’s true though, Vim doesn’t close like most programs because it runs inside your terminal. You don’t want to close your terminal just to exit Vim. So how do you do it? Simply type…

:q

Simple sure, but still a little strange. Let’s break it down.

:

The colon will become very familiar to you while using Vim. Typing : brings you into Command Mode, from Normal Mode, as we learned above. It can be a little cumbersome to always be typing : because you have to Shift+; but we’ll get to a workaround later.

q

This is your first lesson in mnemonics. You can remember q: quit and with that…
Mnemonics

Mnemonics are the key to learning the Vim-grammar. From the outside it looks like knowing Vim is just memorizing a bunch of hotkeys. Nope. It’s really speaking the language of hotkeys, using mnemonics. In the next section you’ll see that almost all commands have a mnemonic, and it makes them 1000x easier to remember.
Navigation Commands

These commands will all be used in Normal M

we do
here