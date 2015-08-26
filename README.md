If the current branch name contains a ticket number, `git-vim` will automatically prepend it to new commit messages.

Tested on mac and "theoretically" working on linux.

# Installation

1. Make `git-vim` executable 

  <pre>
    chmod +x ./git-vim
  </pre>

2. Put it in `/usr/local/bin/` (or run the command below)

  <pre>
    ln -s `pwd`/git-vim /usr/local/bin/git-vim
  </pre>

3. Tell `git` to use `git-vim`

  <pre>
    git config --global core.editor git-vim
  </pre>

Now you're set up to use `git-vim`.
