# Coding Lawyers Club – Getting Started
[Download iTerm](https://www.iterm2.com/). Drag it into your Applications folder

Drag iTerm to your Dock. Click on iTerm. Inside of iTerm, go to:

```
iTerm —> Profiles —> Default —> Edit Profile —> Working Directory (“Reuse previous session’s directory”)
```

For this tutorial, whenever you see `$` you do NOT include it. The `$` is simply meant to represent that you're putting the command in the command line

While still in iTerm, install Oh My Zsh by copying the following command: 

```
$ sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"
```

(you may be asked to install git tools, say yes)

Install Homebrew with:

```
$ /usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
```

Move into the `Desktop` direcotry with:

```
$ cd Desktop
```

[Download VS Code](https://code.visualstudio.com/). Drag it into your Applications folder and then onto your Dock

[Install command line shell by following these instructions](https://code.visualstudio.com/docs/setup/mac#_launching-from-the-command-line)

Sign up for [Github](www.github.com). Send me an email with your name and Github username

[Download Github Desktop](https://desktop.github.com/). Drag it into your Applications folder and then onto your Dock. Sign in with your Github username

In iTerm run (make sure to put the email you signed up with Github!):

```
ssh-keygen -t rsa -b 4096 -C "your_email@example.com"
```

When you're prompted to "Enter a file in which to save the key," press Enter. This accepts the default file location:

```
Enter a file in which to save the key (/Users/you/.ssh/id_rsa): [Press enter]
```

At the prompt about passphrase, just press enter twice:

```
Enter passphrase (empty for no passphrase): [Press Enter]
Enter same passphrase again: [Press Enter]
```

Run:

```
eval "$(ssh-agent -s)"
```

Followed by:

```
ssh-add -K ~/.ssh/id_rsa
```

And finally copy this key to your clipboard with:

```
pbcopy < ~/.ssh/id_rsa.pub
```

On Github, go to [keys](https://github.com/settings/keys)

Click "New SSH key"

For "Title" put "YOUR_NAME_HERE's Computer" (obviously replace with your name)

Under "Key" simply ⌘ + V to paste. Click "Add SSH key". 

Note: If you received an error, you most likely copied something to your clipboard in between instructions. Go back to iTerm, run `pbcopy < ~/.ssh/id_rsa.pub` and immediately go back into the "Key" field and paste.

[Fork the frontend-template repo](https://github.com/dbarabander/template-frontend) by clicking "Fork" in the top right and follow the instructions. Forking means you're making a copy of this code base. 

On your forked repository on Github.com (should look something like https://github.com/YOUR_USERNAME/template-frontend) select the green button to the right that says "Clone or Download" and select "Use SSH" on the top right. Then click the copy icon to the right. Go back to iTerm. Make sure you're located in `Desktop` and type `git clone` and then paste the url you copied. It should look look like the following, with your username instead of YOUR_USERNAME:

```
$ git clone git@github.com:YOUR_USERNAME/template-frontend.git
```

[Fork the template-backend repo](https://github.com/dbarabander/template-backend) in the same way you did the `template-frontend`

Copy the link again by clicking the green button that says "Clone or Download"

In iTerm, clone this repository the same way you cloned the frontend one. It should look look like the following, with your username instead of YOUR_USERNAME:

```
$ git clone git clone git@github.com:YOUR_USERNAME/template-backend.git
```

While in iTerm, install `yarn` by running:

```
$ brew install yarn
```

While in iTerm, install `nvm` by running:

```
$ curl -o- https://raw.githubusercontent.com/creationix/nvm/v0.33.11/install.sh | bash
```

While in iTerm, run:

```
$ source ~/.nvm/nvm.sh
```

While in iTerm, install node 9.11.1 by running: 

```
$ nvm install 9.11.1
```

Make sure you're in the `template-frontend` directory. In iTerm your current directory should still be `Desktop`. 

In iTerm, run the following:

```
$ cd template-frontend
``` 

Followed by:

```
$ code .
```

You should see VS Code open your `template-frontend` repository

Inside of `template-frontend`, install dependencies by running:

```
$ yarn
```

Great. In iTerm, press `⌘ + N` to open a new window.

In iTerm, run:

```
$ cd ..
```

To move out one directory. You should be back in `Desktop`

Now in our new window, let's go into `template-backend`. Hopefully you're seeing the pattern now of what `cd` does. `cd` moves one layer into a directory. `cd ..` moves one layer out of a directory.

```
$ cd template-backend
```

Again, inside of `template-backend` in iTerm, lets open the repo with: 

```
$ code .
``` 

Inside of `template-backend`, in iTerm, lets install the dependencies:

```
$ yarn
```

[Install MongoDb Compass](https://www.mongodb.com/download-center?jmp=tutorials&_ga=2.177525221.1936207160.1531960242-451401237.1531960242#compass). You'll need to sign up. You can give any email you want.

After downloading Compass, click “Connect.” You should now be able to view your database
