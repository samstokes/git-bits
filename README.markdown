# Git Bits #

These are utilities for working with git, including some higher-level commands
to support certain workflows.

They rely on Git's behaviour of hooking into your `PATH` and turning any
command `git-foo` into a git subcommand `git foo`.

They are largely undocumented and unsupported right now, so YMMV.  Happy to
discuss them - Github-message me.

## git-beta-features ##
Shows a graph of all branches that have been merged into beta, but not into
master.

## git-clarity ##
Shows a graph of branch points, merges and tagged commits.
(See also `git clarity -h`.)

## git-committool ##
Shortcut for using `git difftool` to view the changes in a single commit.

## git-local ##
**TODO**

## git-merge-feature ##
Merges a feature branch into the current branch, then deletes the feature
branch.

## git-nows ##
Remove all the "bad whitespace" (as defined by git) from your uncommitted
changes.

## git-pdf ##
Given the name of a feature branch, builds a beautifully syntax-highlit PDF
file containing all commits on that feature branch since it diverged from
`master`, and also shows the full text of all source files touched somewhere
in the branch. Useful for doing code reviews on a mobile device, e.g. iPad.

## git-review ##
**TODO**

## git-review-commits ##
Uses `git difftool` to review, one commit at a time, all commits in a specified
range.  Goes through the commits in the order you'd expect (i.e.  parents
precede children).

## git-russet ##
Safer, saner alternative to `git reset`.  Takes the same arguments and options,
but adds saner semantics: for example, `--hard` prompts you if it would lose
changes.

This is mostly for use in aliases: some of `git reset`'s behaviour is too
verbose to type often, but too dangerous to be easy to type, so this gives you
something that's safe to alias to something short.

## git-wipify ##
**TODO**

***
vim:tw=79
