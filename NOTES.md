## Notes

#### Team project workflow, step by step
![Team project workflow, step by step](https://git.generalassemb.ly/storage/user/6926/files/37342e3c-d5b6-11e7-8456-196762858c5b)

#### Assorted git info

Instructor note

  Be sure to emphasize the semantic difference between rebase and pull. (per issue #18)
  You should always use `git pull --rebase` when your changes do not deserve a separate branch.
  Make this distinction known: Your local branch, into which you pull changes, and remote branch, are actually different branches, and git pull is about merging them (through a fetch and merge). When it would be better for any two branches in question to be one branch is where git pull rebase comes into play. You no longer merge, you actually commit one branch on top of the other for unified history.

  merge -- applies commits from another branch on top of any commits you've made.

  rebase -- adds commits onto a shared commit in both branches history and then reapplies your commits on top of those. After a rebase, pushing to the branch will require --force-with-lease since the history has been rewritten

![git diagram](http://i.imgur.com/QBytN9P.jpg)
![git diagram](http://i.imgur.com/y5aLyg3.jpg)
![git diagram](http://i.imgur.com/0eCZbLT.jpg)
