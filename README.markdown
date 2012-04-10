# GIT Convenience Wrapper Script

## Requirements
Git

## Installation

clone the repo into a directory that is in your PATH system variable, or you can clone the repo and add the repo path to the PATH variable:
	git clone ssh://git@github.com:bmilesp/Gitty.git

## Usage

pass in the following arguments:

	new-branch 'branch-name'
Will create a new local and remote tracking branch and checkout the new branch

	submit 'branch-name' 'commit message'
Will commit all changes to branch-name, update develop, merge in develop, and push the result out to remote branch-name"

	retrieve-branch 'remote-branch-name'
Will create, checkout, track and pull a remote branch that does not yet exist locally


## Author
Brandon Plasters ([bmilesp] (http://twitter.com/bmilesp))

