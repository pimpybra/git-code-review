# git-code-review
A simple custom bash script for generating a git branch for doing a locally rebased code review.

## Installation
Just simply copy the `src/git-code-review` bash script into a directory that is in your PATH. This could be `~/bin` or `/usr/local/bin` if you want everyone on the system to be able to use it.

## Usage
Type `git-code-review` to see usage.

To get started with a review, just run `git-code-review start YOUR-BRANCH-NAME-HERE`

## Assumptions
- You need to have a branch on the remote you want to pull down (this remote can be changed with `--remote` - defaults to `origin`)
- You don't already have a local `code-review/BRANCHNAME` branch.

## Bash Completion
In addition to the installation above, simply do one of the following:

- Copy `assets/bash_completion.d/git-code-review` into `/etc/bash_completion.d`
- OR Add the contents of `assets/bash_completion.d/git-code-review` to your `~/.bash_completion` file
- OR See the details of the [bash-completion readme for other assistance](https://github.com/scop/bash-completion/blob/master/README.md)
