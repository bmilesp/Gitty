# GIT Convenience Wrapper Script

## Requirements
Git

## Installation

Clone the repo into a directory that is in your PATH system variable, or you can clone the repo and add the repo path to the PATH variable:
	
	git clone ssh://git@github.com:bmilesp/Gitty.git

## Usage

pass in the following arguments:


	new-branch <branch-name>
Will create a new local and remote tracking branch and checkout the new branch


	submit <branch-name> 'commit message'
Will commit all changes to branch-name, update $DEVELOP, merge in $DEVELOP, and push the result out to remote branch-name


	retrieve-branch <remote-branch-name>
Will create, checkout, track and pull a remote branch that does not yet exist locally


	delete <branch-name> [-force]
Will delete local and remote branch but will check if they are merged with other branches first for safety. Passing the optional -force parameter will force the deletion even if it is not merged in.


	merge-stage <branch-name>
Will update $DEVELOP branch from $ORIGIN, then merge branch-name into $DEVELOP, then push changes to the stage and test sites


	merge-master <branch-name>
Will make sure branch-name is merged into $DEVELOP first, merge branch-name into $MASTER, then push to the live site


	update-branch <branch-name>
Will fetch and merge a specific branch that exists both locally and remotely

## Authors
Brandon Plasters ([bmilesp] (http://twitter.com/bmilesp))

Benjamin Talavera ([btalavera] (http://twitter.com/alfaben))

