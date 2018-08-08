# Coding Lawyers Club – Getting Started
[Download iTerm](https://www.iterm2.com/). Drag it into your Applications folder

Drag iTerm to your Dock. Click on iTerm. Inside of iTerm, go to:

```
iTerm —> Profiles —> Default —> Edit Profile —> Working Directory (“Reuse previous session’s directory”)
```

While still in iTerm, install Oh My Zsh by copying the following command: 

```
sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"
```
(you may be asked to install git tools, say yes)

While still in iTerm, install Homebrew with: 
```
/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
```

[Download VS Code](https://code.visualstudio.com/). Drag it into your Applications folder

[Install command line shell by following these instructions](https://code.visualstudio.com/docs/setup/mac#_launching-from-the-command-line)

Sign up for [Github](www.github.com). Send me an email with your name and Github username

[Download Github Desktop](https://desktop.github.com/). Drag it into your Applications folder. Sign in with your Github username

[Fork the frontend-template repo](https://github.com/dbarabander/template-frontend) by clicking "Fork" in the top right and follow the instructions. Forking means you're making a copy of this code base. 

On your forked repository on Github.com (should look something like https://github.com/YOUR_USERNAME/template-frontend) select the green button to the right that says "Clone or Download" and select "Use SSH" on the top right. Then click the copy icon to the right. Go back to iTerm. Make sure you're located in `Desktop` and type `git clone` and then paste the url you copied. It should look look like the following, with your username instead of YOUR_USERNAME:

```
➜  Desktop git clone git@github.com:YOUR_USERNAME/template-frontend.git
```


[Fork the template-backend repo](https://github.com/dbarabander/template-backend) in the same way you did the `template-frontend`

Copy the link again by clicking the green button that says "Clone or Download"

In iTerm, clone this repository the same way you cloned the frontend one. It should look look like the following, with your username instead of YOUR_USERNAME:

```
➜  Desktop git clone git clone git@github.com:YOUR_USERNAME/template-backend.git
```

While in iTerm, install `yarn` by running:

```
brew install yarn
```

While in iTerm, install `nvm` by running:

```
curl -o- https://raw.githubusercontent.com/creationix/nvm/v0.33.11/install.sh | bash
```

While in iTerm, run:

```
source ~/.nvm/nvm.sh
```

While in iTerm, install node 9.11.1 by running: 

```
nvm install 9.11.1
```

Make sure you're in the `template-frontend` directory. In iTerm your current directory should still be `Desktop`. 

In iTerm, run the following:

```
cd template-frontend
``` 

Followed by:

``
code .
```

You should see VS Code open your `template-frontend` repository

Inside of `template-frontend`, install dependencies by running: 
```
yarn
```

Great. In iTerm, press `⌘ + N` to open a new window.

In iTerm, run:

```
cd ..
```

To move out one directory. You should be back in `Desktop`

Now in our new window, let's go into `template-backend`. Hopefully you're seeing the pattern now of what `cd` does. `cd` moves one layer into a directory. `cd ..` moves one layer out of a directory.

```
cd template-backend` 
```

Again, inside of `tempalte-backend` in iTerm, lets open the repo with: 

```
code .
``` 

Inside of `template-backend`, in iTerm, lets install the dependencies:
```
yarn
```

[Install MongoDb Compass](https://www.mongodb.com/download-center?jmp=tutorials&_ga=2.177525221.1936207160.1531960242-451401237.1531960242#compass). You'll need to sign up. You can give any email you want.

After downloading Compass, click “Connect.” You should now be able to view your database
