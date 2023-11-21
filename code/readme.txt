explain here what is in the code folder, possibly git submodules and which commit is suppsed to be used of those

note: git submodules can be easily added by going into the folder and running:
$ git submodule add <clone path>

the submodule repo can be used like normal when simply going into the folder, git will know that you are in the other repository and act accordingly.
for example changing branch with
$ git checkout <branch name>
the parent repo will remember changes to the submodule too.
