# Beginnings
This is just a playground to get familiar with what you need for the other course we are working on. This is meant to be a place to learn, test coding, help each other, and above all else HAVE FUN! It could be said that the number one skill you need as a modern developer is how to effectively use source control.  As git (and GitHub) are the most widely used tools in modern development, investing the time to become a power user of these tools is critical for your success. I hope you enjoy the tasks and embrace the platform for a different type of collaboration. 

## The Ingredients
* [Team Members](#team-members)
* [Tools2Use](#Tools2Use)

## <a name="team-members"></a>Team Members
* "Patrick Stephens" <patsteph@cisco.com>
* Add Your Name Here

## <a name="Tools2Use"></a>Tools2Use
* [Github](https://www.github.com)
* [Visual Studio Code](https://code.visualstudio.com/)
* [Homebrew](https://brew.sh)
* [pip](https://pip.pypa.io/en/stable/)
* [Python 3.7.3](https://www.python.org/downloads/release/python-373/)
* [PC or Mac](https://youtu.be/qfv6Ah_MVJU)
* [Markdown Cheatsheet](https://guides.github.com/pdfs/markdown-cheatsheet-online.pdf)
* [A Healthy Curiosity](https://www.entrepreneur.com/article/345981)
__________________________________________________________________________________________

## The Recipe
* [Prepping your environment](#prepping-your-environment)
* [Challenge 1](#Challenge-1)
* [Challenge 2](#Challenge-2)
* [Challenge 3](#Challenge-3)
* [Challenge 4](#Challenge-4)
* [Challenge 5](#Challenge-5) Coming Soon!
* [Challenge 6](#Challenge-6) Coming Soon!
* [Bonus Time](#Bonus-Time)

## <a name="prepping-your-environment"><a/>Prepping your environment
  First things first lets make sure you have a Github account. Click [HERE](https://github.com/join) to get a github accont. Be sure to chooose a name you want to be around forever and also to secure it with a good password.
  
  Now that you have an account what can you do with Github? Well thats a little out of scope for what we are doing however [this](https://docs.github.com/en/github/getting-started-with-github/quickstart) is a good guide to get started with Github. 
  
  Since you have Github installed and spent 3 whole minutes perusing the quickstart guide before being bored you are now ready for a installing some software. 
  
  The first thing we need if we are going to be working with code is a code editor. For the sake of this work we will be using Vissual Studio Code. There are quite a few code editors oout there and whiel they are all good and customizable we will be using Visual Studio Code for our work. If you want to look into some other vode editors I have compiled a few other options for you.
  * [Brackets](http://brackets.io/) A good editor from Adobe BUT they are discontinuing it in Septemeber of this year. Maybe Dan can talk to them about keeping it around. 😄
  * [Atom](https://atom.io/) Another really cusstomizable eidtor and this one is made by Github.
  * [Notepad++](https://notepad-plus-plus.org/) Windows only editor that has a cult following and gets love from everyone for being a great free editor.
  
  To install Visual Studion code you click [HERE](https://code.visualstudio.com/docs/setup/setup-overview) and follow the platfrom specific instructions. 
  
  Now that that is done, select your platfrom from below for some more things to install. 
  
  [PC Instructions](https://www.apple.com/shop/buy-mac/macbook-pro)
  
  Did you click that? Are you mad now? It is a joke. (but do you really hav a PC)
  
  [Mac Installation]
  
  Step 1. Install [Xcode](http://itunes.apple.com/us/app/xcode/id497799835?ls=1&mt=12) on your Mac. Once it is installed move on to step 1a.
     Step 1a. Open Terminal and type the following: 
    
    ``` xcode-select --install ```
       
  Step 2. Run the following command to install Homebrew on your Mac.  
  
    ``` $ /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install.sh)" ```
     
  Step 3. Now we need to update the stock Python on the Mac from 2.x to 3.7. Let's run this in terminal to update Python.
  
    ``` brew install python ```
    
  Step 4. Now we are getting somewhere. BTW PIP should have been installed with Homebrew but we can uupdate it with the following command from terminal.
  
    ``` python -m pip install -U pip ```
  
  We should have all the software we need to get started. Now we are going to move onto Challenge 1. 
  
  ## <a name="Challenge-1"><a/>Challenge 1
  
  ### Hello World
  Build and run a Python script (Hello World), ensuring to use a virtual environment to do it per pluralsight course on setting up a workspace and using PIP all using Visual Studio Code.
  
  ## <a name="Challenge-2"><a/>Challenge 2
  
  ### Local to Git
  Create a new git repo locally, commit your script to it and push it to a new repo on Github.
  
  ## <a name="Challenge-3"><a/>Challenge 3
  
  ### Build as a team - Forking
  Step 1. Fork this reposiory.(You are already looking a the README.md so you are on the right site to fork, but just to make sure and look in the URL for github.com/GESWCollab/beginnings
  Once you fork the repository you will see it has all the ssame components as this main site but it will be in your github environment. 
      Example: I forked the repository logged in as me and it creates https://github.com/patsteph/beginnings 
  
  Now lets get the file local so we can work on it. 
  
```
cd ~/coding
git clone https://github.com/<YOUR GITHUB USER>/beginnings
```

Change into that local directory and make sure you see the README.md file.

```
cd beginnings
ls -la
```

Now that you know the file is there lets open it with Visual Studio code and make some Markdown changes. 

In Code click File --> Open... Navigate to your coding/beginnings folder and select the README.md file. 

Once the file opens find the Team Members section and add your name and email with appropriate formatting. Now that you have it updated we need to push it back up tot the cloud.

```
git add README.md
git commit -m "Added <your name> to README file"
git push
```

You have now written a code change but that code is only in your FORK of the repository, not the original repo.  We can ask that the ppstream repository to "PULL" our changes into it by opening a "Pull Request"

In GitHub in your repository, click the "New pull request" button

You'll be given a chance to view the changes, and then click "Create pull request" Be sure and add a note with it so I know what I am pulling into the main repo. 

After opening, you'll be taken back to the PR list on the upstream repository. 

## <a name="Challenge-4"><a/>Challenge 4

Why dont we try working on some Python code specific to our endpoints. Chris had posted this in our Webex space. Lets get a copy of the xAPI over WebSockets Library and work with it on our local machine. The main github site for this library is here [PYOWS](https://github.com/cisco-ce/pyxows).

```
git clone https://github.com/cisco-ce/pyxows.git
```

Now that you have your own copy you can work on it. Navigate locally to your pyxows directory. Once in your pyxows directory run the setup script.

```
python setup.py install
```

Now install the async library. 

```
pip install asyncio
```

## <a name="Challenge-5"><a/>Challenge 5 Coming Soon!
  
## <a name="Challenge-6"><a/>Challenge 6 Coming Soon!

## [Bonus Time](#Bonus-Time)
What are some other things we could create in this way?

* Slides 😑
* Upcoming team call topics ❓
* Take on a side projects 
   * Webex for Developers https://github.com/webex?language=python
   * Power Platform Connectors https://github.com/webex/PowerPlatformConnectors
   * Bot Framework https://github.com/jpjpjp/webex-bot-python
   * DevNet Webex Repo https://github.com/CiscoDevNet/awesome-webex
* Trick out this README?
   * https://shields.io/
   * https://coderwall.com/p/fy05hq/how-to-make-beautiful-github-readme
   * https://github.com/othneildrew/Best-README-Template


  
  
  
  
  
 
  
  





