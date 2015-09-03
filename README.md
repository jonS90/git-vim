If the current branch name contains a ticket number, `git-vim` will automatically prepend it to new commit messages.

Tested on mac and "theoretically" working on linux.

# Installation

1. Download `git-vim` somewhere. It doesn't have to be in `/usr/local/bin`.

  <pre>
    cd &lt;somewhere&gt;
    curl https://raw.githubusercontent.com/jonS90/git-vim/master/git-vim > git-vim
  </pre>

2. Make `git-vim` executable 

  <pre>
    chmod +x ./git-vim
  </pre>

3. Tell `git` to use `git-vim`

  <pre>
    git config --global core.editor `pwd`/git-vim
  </pre>

Now you're set up to use `git-vim`.
