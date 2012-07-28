## Dropbox Installation

Go to [http://www.dropnbox.com](http://www.dropbox.com) and set up an account. Once you've installed the application, you'll have a folder `$HOME\Dropbox`. Create a new folder `$HOME\Dropbox\config`--this is where we'll store all of our personalized configuration files. 

You can store these configuration files in Github or Bitbucket--but that may be overkill for files that rarely, if ever, need to be merged. Dropbox stores prior versions of files--that should be good enough.

## Configuration

Create a folder for any application that you wish to configure. For example, create `$HOME\Dropbox\config\vim` to store all of your `vim` configuration files. When you move from machine to machine, you can symlink your `vim` configuration files from your home folder to the corresponding files in your Dropbox folder.

For example:

    $HOME/.vimrc -> $HOME/Dropbox/config/vim/.vimrc
