# clc-getting-started

* [Download iTerm](https://www.iterm2.com/)
* Go to iTerm —> Profiles —> Default —> Edit Profile —> Working Directory (“Reuse previous session’s directory”)
* Install My Zsh with: `sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"`
(you may be asked to install git tools, say yes)
* Install Homebrew with: `/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"`
* [Download VS Code](https://code.visualstudio.com/)
* [Install command line shell by following these instructions](https://code.visualstudio.com/docs/setup/mac#_launching-from-the-command-line)
* Sign up for [Github](www.github.com). Share your Github profile to CLC Admins
* [Fork the clc repo](https://github.com/dbarabander/clc)
* Clone the fork with `git clone https://github.com/YOUR_USERNAME/clc.git`
* [Fork the clc-server repo](https://github.com/dbarabander/clc)
* Clone the fork: `git clone https://github.com/YOUR_USERNAME/clc-server.git`
* Install Yarn: `brew install yarn`
* Install nvm: `curl -o- https://raw.githubusercontent.com/creationix/nvm/v0.33.11/install.sh | bash`
* Run `source ~/.nvm/nvm.sh`
* Install node 9.11.1: `nvm install 9.11.1`
* `cd clc` to enter to repo and `code .` to open the repo
* Inside of `clc`, install dependencies with `yarn`
* `cd clc-server` to enter the repo and `code .` to open the repo
* Inside of `clc-server`, install the dependencies with `yarn`
* [Install MongoDb Compass](https://www.mongodb.com/download-center?jmp=tutorials&_ga=2.177525221.1936207160.1531960242-451401237.1531960242#compass)
* After downloading Compass, click “Connect.” You should now be able to view your database
