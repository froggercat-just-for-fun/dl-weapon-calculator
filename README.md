# dl-weapon-calculator
Dragalia Lost Weapon Calculator based on the gamepedia cargo query.

[Link to Gamepedia API Explorer](https://dragalialost.gamepedia.com/Special:CargoQuery)

## Clone the repo
This repository uses git lfs. Be sure to install it if you don't have it already.

## Installation
You can, ofc, ignore all these environment doohickeys and just run the `pip install -r requirements.txt` if you don't care about environment management. The code here will run on all versions of Python3.

If you want to use it as nature intended ...

This repository has been set up for the following environment managers:

* asdf (allows you to install multiple versions of many interpreters/ compilers)
* direnv (allows for folder-based environment management from your terminal)
* asdf-direnv (to tie the two together)

Install these if you don't have them.

Then, you'll need the following in asdf (there are detailed instructions on their website):

* The python version we use in this project (check the `.envrc` file)
* `virtualenv` (or `venv`/`pyenv` depending on which virtual environment your copy of `direnv` uses.)

You'll then be ready to run `direnv allow .envrc` to enable direnv in this directory. Direnv should then set up a python virtual environment for you in this folder.

Now you're ready to install the library dependencies. Run `pip install -r requirements.txt` to install the necessary libraries in your shiny new virtualenv.

I've also included some settings for VSCode. They expect the following extensions to be available:

* Python
  * Sets Python intepreter to use the correct direnv virtual env.