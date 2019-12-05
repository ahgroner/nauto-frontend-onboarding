>### Welcome to Front End Development.

##### 💚🚦🚕 Nauto’s awesome, you’re awesome, let’s get to work. 💻📱🤘

#### Load up these tools, in order:
This is assuming you have a recent model MacBook Pro.

#### Apple Xcode:
Apple Developer App
Get it from the Apple App Store.  You’ll need to get an AppleID for that.
We don’t use this as such, but it provides us with the official xcode command line tools, which are required for everything else.

#### Brew:
MacOS Package Manager
https://brew.sh/
We use this to install several packages.
Installs with a terminal command:
```shell
ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
```

#### Git:
Super popular version control
Use Brew to install Git:
```shell
brew install git
```

*Slack @leipan to get access to the nauto organization repo on github.*

#### Node:
- **With NVM:**
```shell
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.35.1/install.sh | bash
```
**Or:**
```shell
wget -qO- https://raw.githubusercontent.com/nvm-sh/nvm/v0.35.1/install.sh | bash\
```

If you don’t have wget then:

```shell
brew install wget
```

Either of the following command will add 

```shell
export NVM_DIR="$([ -z "${XDG_CONFIG_HOME-}" ] && printf %s "${HOME}/.nvm" || printf %s "${XDG_CONFIG_HOME}/nvm")"
[ -s "$NVM_DIR/nvm.sh" ] && \. "$NVM_DIR/nvm.sh" # This loads nvm
```

To your `.bashrc` file, or `.zshrc` if you are on zsh.

You need to
```shell
source .bashrc
```
or
```shell
source .zshrc
```

**Check:**
```shell
nvm --version
```

**Install node**
```shell
nvm install 10.9.0
```
```shell
nvm alias default 10.9.0
```

- **With brew:**
The Node.js development system.
https://nodejs.org
Use Brew to install Node:

```shell
brew install node
```

Note: We should be using v10.9.0, although we need older versions for some apps. 

#### Yarn:
Package manager
https://yarnpkg.com
Use Brew to install Yarn:
```shell
brew install yarn
```

#### Microsoft Visual Studio:
Nice software development environment. 
https://visualstudio.microsoft.com
It’s free to download.

(end of Don’s section, the rest needs some work)

#### Github SSH key:
- Head to your github account and click on little triangle next to profile icon
- Choose settings from the dropdown
- On the left tabs select **SSH and GPG keys**
- Click on **New SSH key** button and give your SSH a name:
- Open your terminal and paste the following commands:
`cd`
`shell ssh-keygen -t rsa -b 4096 -C "your_email@nauto.com"`
Click enter all the way or rename your SSH key and add phrase if you wanted
`cat ~/.ssh/id_rsa.pub | pbcopy` or replacer id_rsa.pub with your public key name
Head back to the browser and paste your key and click add.
- To clone repos to your local use SSH mode
- You will get asked to use your key, type **yes** full word.
- In case if you did not get asked then add your key manually.
`ssh-add ~/.ssh/id_rsa` and `git clone repo` again.

More tools to load up
(under construction)

#### Phrase:
https://phrase.com/cli/

#### NPM:
https://www.npmjs.com/get-npm
Additional Steps

Get invited to https://www.npmjs.com/settings/nauto/packages. Please create an npm account if you don’t already have one.

- Create a Personal Access Token in npm (you’ll need this because w 2FA you can’t use your password)
- Login to npm CLI

#### AWS CLI
https://aws.amazon.com/cli
Additional Steps 
Create a Pull request in the infrastructure. The pull request would look similar to this: https://github.com/nauto/infrastructure/pull/457 - you need to make changes for every environment that you need access to. Here’s detailed info.

You will also need to decrypt the keys that you’ll get after having your PR approved. Here’s how to do it. You’ll need access to Nauto’s 1password Engineering vault - if you don’t see it, you can ask for access in Slacks #it-help.

### Web apps we use:

#### Jira:
You should have received an invite to Jira with your nauto email. If not, email it@nauto.com
Tickets in our component Fleet App (Web)


#### Figma:
Figma is our primary design tool
Create an account using google auth using your Nauto email.
 
Tickets in our component Fleet App (Web)

Launch Darkly
