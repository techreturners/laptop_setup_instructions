# MacOS Setup Instructions

#### 1) Download Chrome Web Browser

We will be using tools included in Chrome web browser throughout the course so please ensure you have this downloaded and ideally set to your default web browser.

[Download Chrome](https://www.google.com/chrome/)

#### 2) Download Slack Desktop

We use Slack as our main communication tool so it's really worth having the desktop version, which can be downloaded [here](https://slack.com/downloads/mac).

We would also recommend downloading it on your phone, so you can let us know if you happen to be running late etc.

#### 3) Get a Github account

Github is a collaboration platform for developers. We will be using it to give you access to course material, and you'll use it to host and share your code.

It is also the place prospective employers often look to see evidence of projects you've worked on.

Sign up to a free account [here](https://github.com) and make sure to email harriet.ryder@techreturners.com and james.heggs@techreturners.com your username so we can add you to our organisation.

#### 4) Download Visual Studio Code

When writing software, developers use tools to help them. One of those tools is known as an Integrated Development Environment or IDE for short. This is a tool that helps the developer when writing code.

You use an IDE to write software in the same way that you might use Microsoft Word to produce a document.

On this course we use a tool called Visual Studio Code to support our writing of code. So firstly head over to their website to [download and install Visual Studio Code](https://code.visualstudio.com/).

Once installed we can do one more enhancement to your laptop in order to make it even easier to get coding. We'll do this by adding a command line shortcut that will start up Visual Studio Code for us.

To do this firstly open Visual Studio Code on your laptop. This short video shows how you can open Visual Studio Code.
(https://storage.googleapis.com/tech-returners-course/001-fundamentals-launchingvscode.mp4)

Once opened you should then open the **Command Palette**. To do this simply hold the **Shift + Cmd** keys and whilst they are held press the **P** key.

You'll see a screen that looks similar to the following

![Visual Studio Code Shell Command](https://code.visualstudio.com/assets/docs/setup/mac/shell-command.png "Visual Studio Code Shell Command")

Search for **shell command** and then choose the option:

**Shell Command: Install 'code' command in PATH**

This will install the command line shortcut that allows you to start Visual Studio Code from the command line.

You can now quit Visual Studio Code.

Further info on this process can be found [here under the **Launching from the command line**](https://code.visualstudio.com/docs/setup/mac#_launching-from-the-command-line) heading

#### 5) Install iTerm

Your Mac comes with a built in terminal application (also referred to as _command line_ or _console_). However, there are better applications available with more features. We recommend downloading and using [iTerm2 for Mac](https://www.iterm2.com/downloads.html).

#### 6) Install Homebrew

Homebrew is a package manager which we will use to help us install other programs.

To install homebrew, open up the terminal (iTerm, from the above step) and run

```
/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
```

More details on HomeBrew can be [found here](https://brew.sh/)

If you run `brew --version` in your terminal and you see something like this, it has been successful:

```
Homebrew 2.0.4
Homebrew/homebrew-core (git revision 6464f; last commit 2019-03-12)
Homebrew/homebrew-cask (git revision dcbd02; last commit 2019-03-12)
```

#### 7) Install Node

The next item to install is [NodeJS](https://nodejs.org/en/). Node provides the Javascript framework for running our code and applications.

When you install Node it also installs [Node Package Manager](https://www.npmjs.com/) (NPM for short). Node Package Manager (NPM) is a piece of software that allows you to install other Javascript packages that have been created by the global software development community.

The packages contain code written by other people and have been made available for everyone to use. Making your code available to the global community is a practice known as [Open Sourcing](https://en.wikipedia.org/wiki/Open-source_software) your software.

For example - lets say you want to convert a number to its English description. Convert the number **100** to its description of **one hundred**. In programming terms this is harder than you might expect - however someone has already [created a piece of code that does this](https://www.npmjs.com/package/number-to-words) and it saves us from having to write our own code to solve this problem. Effectively, leaving us to focus on writing code for our own unique problems and businesses.

To install Node run the following command in your terminal:

```
brew install node
```

You should now see a lot of text on your console as Node gets installed. You can verify that node is installed by running:

```
node -v
```

It should output something similar to the example below. NOTE: The version you see might differ to the example below.

```
v8.11.1
```

#### 8) Install Git

Git is a [Version Control System](https://en.wikipedia.org/wiki/Version_control) (VCS for short). At this stage don't worry too much about what Git is or what it does, we cover Version Control Systems and Git in more detail later this week. For now we just need to make sure it is installed on your laptop.

To install Git run the following command in your terminal:

```
brew install git
```

You can check that git is installed by running:

```
git --version
```

It should output something similar to:

```
git version 2.11.0 (Apple Git-81)
```

#### 9) Configure Git

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

#### 10) Get a notetaking app

Throughout the course you will probably want to take lots of notes, often with code samples. Microsoft Word/Apple Pages are not good choices for this kind of notetaking as they won't format your code correctly and will try to autocomplete in an annoying way.

We recommend downloading a notetaking app which supports Markdown and inline code.

Examples are:

[Bear](https://bear.app/)

[SimpleNote](https://simplenote.com/?)

[BoostNote](https://boostnote.io/)

There are also more paid options like [Quiver](http://happenapps.com/#quiver) but one of the above is a good start.

Congratulations, your laptop is now good to go 🎉

If you've finished in mega-speedy time and you don't want to go home yet, take a look at the [Codecademy course on the Command Line](https://www.codecademy.com/learn/learn-the-command-line) and start getting used to using your new terminal application (iTerm).
