This repository contains some shared commands, aliases, and configurations to make development processes easier and more consistent across teams.

## Usage
Add a variable to your .bash_profile or .zshrc or equivalent file if it changes in the future, which contains the path to your workspace directory (where you keep your git repositories).
```
WORKSPACE_PATH=~/path/to/your/workspace
```

### Including everything
To include the contents of all of the dotfiles, simply source the `all.sh` file in this repository. You can do this by adding the following to your .bash_profile or .zshrc file (after the variable from above).
```
source $WORKSPACE_PATH/dotfiles/all.sh
```

After any changes have been made to any `.sh` file you will need to close all terminal window & reopen them or type
```
source ~/.zshrc
```

### Including individual dotfiles
The dotfiles are broken into domain-specific files, so if you prefer to have your own commands for a given topic you can. The following files can be included individually.
```
source $WORKSPACE_PATH/dotfiles/git.sh          # aliases for git
source $WORKSPACE_PATH/dotfiles/directories.sh  # aliases for repo directories
```
