This document has some informations about the code and instructions about
execution.

Consider as the root folder the folder that has the sub folders spec and lib.


# INSTALLATION AND PRE-REQUISITES

The program do not requires installation. It's very simple. Just execute. But it
has some pre-requisites. As the program was developed in Ruby, you need the
installed (version 2.2.1) and some interactive shell to run it. Installing Ruby
you already have the IRB (interactive Ruby shell). Just type

$ irb

in the terminal and enter the shell.

OBS: any command instruction will be preceded by a '$' symbol.

With Ruby installed, first thing is to install the gem bundler. So, just run

$ gem install bundler

and the job will be done. Then,if you want to run the tests, you'll need Rspec
installled. Rspec is a tes framework for Ruby. All you need to do is run in the
bash - inside the root folder

$ bundle install

and Rspec will be installed for you.


# TESTS

To execute the tests, at the root folder just run

$ rspec

and the result of the tests will is shown.


# EXECUTION

I will indicate the irb mode with an 'irb>' at the begin of the instruction.
But, to run the instruction, ignore it just typing all the instruction after
'irb>'.

To execute the program, firstly enter the IRB mode

$ irb

then load the file. To do that, just type

irb> load 'lib/number_prettifier.rb'

Now you have the file and it content loaded in the Ruby console. Let's play.

As the challenge asked, you have a function that accepts a parameter as the
number you want to prettify. For example, if you import the file/code inside
another program and want prettify a number, could just invoke the function like
this

NumberPrettifier.prettify(number_you_want_prettified)

But, to be more cool and interactive to play in the terminal, I put too a mode
where you will be asked for the number. So, at the Ruby shell, just type

irb> NumberPrettifier.prettify

and will be asked a number. If you put a number greater then the major trillion
number, will be asked to you enter a new number, for example.

To finish the execution at any time, press Ctrl + c


# FINAL CONSIDERATIONS

Was a very funny and constructive. Practically any thing in development is
funny. I love it. But, to clarify some things, I could do a more verbose and
more separated job. But I thought that it was not necessary. I would not want
to make more classes just to do a UML diagram more beautiful. It's unnecessary
and only would make my code blow up. Other thing I thought to do was inherit
the Ruby Numeric class and put my methods inside it. But I chose not to do for
no particular reason. Just a matter of simple choice.
