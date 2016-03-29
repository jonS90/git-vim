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

# Configuring the commit prefix

You can configure different repostories to use different commit prefixes. To do
so, `cd` into the repo and set the editor.

<pre>
git config core.editor 'path/to/git-vim "custom prefix %t: "'
</pre>

Whenever `git-vim` sees a ticket number in a branch, it will prepend new commit
messages with `custom prefix %t: `, substituting `%t` with the actual ticket
number.
