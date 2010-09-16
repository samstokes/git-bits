# Git Bits #

These are utilities for working with git, including some higher-level commands
to support certain workflows.

They rely on Git's behaviour of hooking into your PATH and turning any command
"git-foo" into a git subcommand "git foo".

They are largely undocumented and unsupported right now, so YMMV.  Happy to
discuss them - Github-message me.


## git-clarity ##
Shows a graph of branch points, merges and tagged commits. (see also git clarity -h)

## git-committool ##
Shortcut for using difftool to view the changes in a single commit.

## git-local ##
**TODO**

## git-merge-feature ##
Merges a feature branch into the current branch, then deletes the feature
branch.


## git-review ##
**TODO**

## git-review-commits ##
Uses 'git difftool' to review, one commit at a time, all commits in a specified
range.  Goes through the commits in the order you'd expect (i.e.  parents
precede children).

## git-wipify ##
**TODO**
