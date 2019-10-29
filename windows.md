# Windows Setup Instructions

Once you have installed **the bash shell command line tool** follow these instructions for installing other important programs on a Windows laptop.

#### 1) Download Chrome Web Browser

We will be using tools included in Chrome web browser throughout the course so please ensure you have this downloaded and ideally set to your default web browser.

[Click here to Download Chrome](https://www.google.com/chrome/)

#### 2) Download Slack Desktop

We use Slack as our main communication tool so it's really worth having the desktop version, which can be downloaded [here](https://slack.com/downloads/windows).

We would also recommend downloading it on your phone, so you can let us know if you happen to be running late etc.

#### 3) Get a Github account

Github is a collaboration platform for developers. We will be using it to give you access to course material, and you'll use it to host and share your code.

It is also the place prospective employers often look to see evidence of projects you've worked on.

Sign up to a free account [here](https://github.com) and make sure to email james.heggs@techreturners.com and harriet.ryder@techreturners.com your username so we can add you to our organisation.

#### 4) Download Visual Studio Code

When writing software, developers use tools to help them. One of those tools is known as an Integrated Development Environment or IDE for short. This is a tool that helps the developer when writing code.

You use an IDE to write software in the same way that you might use Microsoft Word to produce a document.

On this course we use a tool called Visual Studio Code to support our writing of code. So firstly head over to their website to [download and install Visual Studio Code](https://code.visualstudio.com/). Select the version for Windows.

#### 5) Install Node

The next item to install is called NodeJS. Even if you already think you have NodeJS installed, please follow the below instructions to re-install it so we are all using the same type of installation.

To install Node, open the bash shell command line tool (search for Ubuntu in your list of applications) and run the following commands in the terminal window which opens. Run the commands in the following order:

```
sudo apt update
```

```
sudo apt install curl
```

Then we use to tool Curl to install a program called Node Version Manager, the recommended tool which can be used to install Node!

```
curl -o- https://raw.githubusercontent.com/creationix/nvm/v0.33.0/install.sh | bash
```

Then run:

```
nvm --version
```

To ensure that NVM is correctly installed. If it says "Command nvm not found" then try closing and reopening your Terminator application, and trying again. If it is installed correctly it should show a version number such as `0.33.0`

Then, use NVM to install NodeJS:

```
nvm install node
```

To check it's installed correctly, run:

```
node -v
```

Again you should see a version number such as `v12.4.0`. Your version might be a little different but if it's less than 8 please let us know!

NVM also should install an additional program called NPM. Verify it has installed by typing:

```
npm --version
```

If the output tells you the version is below 5.0.0 then run:

```
npm install -g npm
```

And check the version again.

###### What are Node and NPM?

Node provides the Javascript framework for running our code and applications. It basically allows us to run JavaScript code on our computers which we'll learn how do do throughout the Pre-Journey.

Node Package Manager (NPM) is a piece of software that allows you to install other Javascript packages that have been created by the global software development community.

The packages contain code written by other people and have been made available for everyone to use. Making your code available to the global community is a practice known as [Open Sourcing](https://en.wikipedia.org/wiki/Open-source_software) your software.

For example - lets say you want to convert a number to its English description. Convert the number **100** to its description of **one hundred**. In programming terms this is harder than you might expect - however someone has already [created a piece of code that does this](https://www.npmjs.com/package/number-to-words) and it saves us from having to write our own code to solve this problem. Effectively, leaving us to focus on writing code for our own unique problems and businesses.

#### 6) Install Git

Git is a [Version Control System](https://en.wikipedia.org/wiki/Version_control) (VCS for short). At this stage don't worry too much about what Git is or what it does, we cover Version Control Systems and Git in more detail later. For now we just need to make sure it is installed on your laptop.

First, maybe you have git installed already? Type:

```
git --version
```

If it says the command is not found, then you need to install it. To install Git run the following commands in order in your terminal:

```
sudo apt update
```

```
sudo apt install git
```

You can check that git is installed by running:

```
git --version
```

It should output something similar to:

```
git version 2.11.0
```

#### 7) Configure Git

When using Git, messages about what changes you have made to a codebase will be recorded using your name and email address. For this to work correctly, you should configure Git with your name and email address. You should choose the email address which you used to sign up to Github, so that Git and Github integrate correctly. Open your terminal application and type the fo

```
git config --global user.name "Your Name"
```

```
git config --global user.email "youremail@domain.com"
```

To see that the above steps worked correctly, type:

```
git config --list
```

and you should see your name and email outputted in the following format:

```
user.name=Your Name
user.email=youremail@domain.com
```

#### 8) Get a notetaking app

Throughout the course you will probably want to take lots of notes, often with code samples. Microsoft Word/Apple Pages are not good choices for this kind of notetaking as they won't format your code correctly and will try to autocomplete in an annoying way.

We recommend downloading a notetaking app which supports Markdown and inline code.

Examples are:

[SimpleNote](https://simplenote.com/?)

[BoostNote](https://boostnote.io/)

There are also more paid options but one of the above is a good start.

Congratulations, your laptop is now good to go 🎉
