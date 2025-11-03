---
layout: misc
title: Resources

---
## Using the workshop materials

Our materials are designed to be learned in one of our [Humble Data workshops](https://humbledata.org/pages/up-coming.html), where you'll have mentors to help and answer your questions. However, if you're unable to join us you're also welcome to work through these materials on your own. Below are instructions on how to access and work with the materials.

### Accessing the materials in browser

**The easiest way to access the materials for beginners is to use our [JupyterLite](https://jupyterlite.readthedocs.io/en/stable/) server.** Select a language below to get started:

- [English](https://humbledata.org/online-workshop/lab/index.html)
- [Spanish](https://humbledata.org/online_workshop_spanish/lab/index.html)
- [Italian](https://humbledata.org/online-workshop-italian-v2/lab/index.html).

Please contact us if you'd like to help out the project by translating the materials into other languages!  

### Installing the materials locally

If you're interested in learning how to manage your own Python Environment the materials can also be cloned from our [GitHub repo](https://github.com/HumbleData/beginners-data-workshop). If you want to use the materials this way, you will need to install them locally. Instructions on how to do this are provided below. Don't worry if you've never done this before—these instructions are designed for complete beginners and will walk you through each step.

#### Open up a new terminal
To get started, open up a new terminal on your computer. A terminal is a tool that allows you to interact with your computer by typing in commands. It allows you to do a very wide variety of things (as you'll see below) in an efficient way.

On Windows 10, you need to open the program "Command Prompt". To do so:
1. Press the Windows key or click the Start menu. 
2. Search for "Command Prompt" or just type `cmd`.
3. Click on the Command Prompt application.

On Windows 11, you need to open the program Windows Terminal. To do so:
1. Press the Windows key.
2. Search for "Windows Terminal."
3. Click on the Windows Terminal application.

Finally, on Mac, you need to open the program Terminal. To do so:
1. Press `Command (⌘) + Space` to open Spotlight Search. 
2. Type `Terminal` and press Enter.
3. The Terminal application will open.

#### Install Python

Next, we need to install Python. This section is a bit detailed, but stay with us—you'll only need to do this once!

To give a bit more context, Python works by installing a piece of software on your computer called the _Python executable_. In the following section, we're going to see how to install the Python executable in both Windows and Mac. Once installed, the Python executable can take pieces of code written in Python and run them. You'll see how to run Python code at the end of this tutorial.

There are many people working on incorporating new features into Python, making it possible for the language to do new things or make it run faster. (In fact, if you come to one of the Python conferences, called [PyCons](https://pycon.org/), you can meet some of these people! The community is very nice and friendly, and very welcoming to beginners, so we encourage you to think about attending.) All these updates to the language mean that the Python executable has a new release every year, denoted by the format 3.X. You'll see this when you try to first download a Python executable: there will be a range of choices of which version to use. We recommend using the latest version when you're starting.

**On Windows 10/11**  
First, download and install Python from [here](https://git-scm.com/download/win). Make sure you pick the `Latest Python 3 Release` to download. As described above, this will allow you to use the latest Python version.

Once it has downloaded, double-click on the file and follow the instructions in the wizard.
You will likely need to run the following steps to use Python (see [this link](https://realpython.com/add-python-to-path/#how-to-add-python-to-path-on-windows)) for more details:
1. Find where Python was just installed. Go to the Start menu, then type `Python`. It will be called something like `Python 3.12 (64 bit)` (the number after 3 will be different based on the version you downloaded). Right-click on this, and select `Open file location`.
2. Go back into the `Programs` folder.
3. The folder containing Python will have the name of the Python version you just downloaded (e.g., `Python 3.12`). Copy the name of this folder (e.g., `C:\Users\joana\AppData\Roaming\Microsoft\Windows\Start Menu\Programs\Python 3.12`). You might need to change the name of this path so it doesn't contain any spaces—try steps 4 through 7, and if they don't work, try changing the final `Python 3.12` to `Python_3_12` and then repeat steps 4 through 7.
4. Once you’ve located your Python executable, open the Start menu and search for the `Edit the system environment variables` command, which opens up a `System Properties` window. In the `Advanced` tab, click on the button `Environment Variables`. There you’ll see `User and System variables`, which you’ll be able to edit.
5. In the section entitled `User Variables`, double-click on the entry that says `Path`. Another window will pop up showing a list of paths. Click the `New` button and paste the path to your Python executable there. Once that’s inserted, select your newly added path and click the `Move Up` button until it’s at the top.
6. You may need to reboot your computer for the changes to take effect. 
7. You can now test whether Python is installed correctly. Open a new terminal window, and at the prompt (see the image below, where it says `C:\Users\joana>`), type `py --version`. It should print something like `Python 3.12.4`. Don't worry if the numbers are not exactly the same! As above, it depends on exactly which version you downloaded.

**Mac OS**

1. Go to https://brew.sh/ and follow the instructions. This will install a program called HomeBrew, which makes it a lot easier to install things like Python on your computer. As you can see from the instructions, you need to copy the line `/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"` and paste it at the prompt in the terminal, then press enter. 
2. We can now use Homebrew to install Python. At the terminal prompt, type in `brew search python`. You'll see a lot of versions of Python listed, but we're looking for versions that have the format `python@3.X` (where X is a number). These are the Python executables for Mac. Pick the latest version, and at the prompt in terminal, enter `brew install python@3.X` (where you need to replace `X` with the version number you're using. For example, if I wanted to install Python version 3.13, I would enter `brew install python@3.13`).

#### Install Git

Now we need to install something called Git. Git is essentially a sophisticated "save system" for your work. Unlike regular saving that overwrites previous versions, Git keeps a complete history of all changes. Think of it as a time machine for your files that lets you see what changed, when it changed, and who changed it.

At its core, Git works by taking "snapshots" (commits) of your project at different points in time. These snapshots are organized in "repositories" (called "repos" for short) which track the entire history of your project.

Git can also be used to share code through online platforms, using a system called Version Control or VCS. The platform we will in this workshop is called GitHub. You can download (called "cloning") code that others have shared on GitHub to your computer, and in the next step we'll be cloning the materials for this workshop. This process downloads not just the current version of the files, but the entire history of changes tracked by Git. Once cloned, you have all the materials locally and can work with them as needed, while also maintaining the connection to the original repository to potentially receive updates or contribute changes back.

First things first: let's download Git. Just like with installing Python, you'll only need to do this once.

**On Windows 10/11**

Follow the instructions on [this page](https://github.com/git-guides/install-git#install-git-on-windows).

**On Mac OS**

1. On Mac, we're going to use HomeBrew again to install Git. You can see how useful HomeBrew is - we can basically use it to install everything. In the terminal, type `brew install git` to install it.
2. Check that the installation worked by typing `git version` at the prompt. You should get something like `git version 2.39.3 (Apple Git-146)`, which will confirm that Git was indeed installed correctly.

#### Clone the repo using Git

Now that we have Git installed, we're going to use it to get the code for the workshop. As mentioned above, this is called "cloning the repository" or "cloning the repo", for short; that is, using Git to download all the files we need for the workshop. These files are hosted on GitHub, which as we mentioned earlier, is one of the online platforms for sharing code using Git. 

To clone the repo:
1. On your computer, go to the folder that you want to copy the workshop folder to (for example, you might make a folder in your Documents folder called "python"). On Windows, hold down the Shift key and right-click on the folder, and select `Copy as path`. On Mac OS, right-click on this folder and press Option, and select `Copy {folder name} as Pathname`. This will give us the location, or "path", of this folder.
2. In the terminal, enter `cd ` and then paste the folder name inside quotation marks. For example, it might look something like `cd "/Users/Jodie.Burchell/Documents/python"`. The `cd` command (which stands for "change directory") is simply your way of telling the computer "I want to go to this folder" when you're typing commands instead of clicking on icons. Make sure you keep this terminal window open.
3. Go to the [Humble Data repo](https://github.com/HumbleData/beginners-data-workshop) on GitHub.
4. Towards the top of the page, you'll see a green button that says "Code". Click on this button.
5. You'll now see a dropdown menu. You'll see a header that says "Clone" and a tab that says "HTTPS". Click on this.
6. You should see a link to `https://github.com/HumbleData/beginners-data-workshop.git` here. Click `Copy url to clipboard`.
7. We're now ready to clone the repo. Go back to the terminal window where you used `cd` to move to the correct directory. Enter `git clone https://github.com/HumbleData/beginners-data-workshop.git` at the prompt. The repo will now be cloned to your local machine.

As a note for the future, this is how you can clone any code from GitHub. So if you see a cool tutorial on GitHub you'd like to complete after you finish Humble Data, you can get the code on your machine by following these exact same steps!

#### Create a virtual environment

We're almost there! A couple of steps ago, we installed Python, which allows us to run basic Python code. As you continue learning, you'll discover that Python is an incredibly versatile language that powers everything from websites to cutting-edge scientific research. In fact, Python has been used at places as diverse as Instagram, Spotify, and the Large Hadron Collider, so as you can see, Python's applications are really just limited to your imagination!

However, this gives us a slight problem—these are _very_ different applications of the language, and building in functionality to cover all of them would make the base installation of Python absolutely massive. Instead, the base installation of Python allows us to do the "core" stuff (you'll learn about this in your first lesson of the workshop), while the code to do specialised tasks such as data transformations or visualisation is contained in additional units called packages. These packages can be downloaded and installed.

The recommended way to install packages is by creating something called a virtual environment to store them in. A virtual environment is like a separate, self-contained workspace on your computer for your Python project where you can install packages without affecting other projects. The reason this is needed is that packages, just like the Python executables, change over time and have different versions. This might involve changing the names of commands, or adding or removing commands entirely, meaning an older piece of code using that package might not work with newer versions of the package. Having a dedicated virtual environment for each project means that you don't have to worry about these incompatibilities between code and the installed packages. You can create a dedicated virtual environment for each project, and use the versions of the package which were current at the time you created your project.

To create a virtual environment, open a terminal window and navigate to the directory containing the repo with the Humble Data materials that you just cloned. Do this using the `cd` command we used in the last section when we cloned the repo - see if you can work out how to apply this to getting inside the folder containing the workshop materials!

Once you're inside this directory, type `python3 -m venv myvenv` at the terminal prompt. This is going to create a new folder inside the directory called "myvenv". This contains a bunch of code to make the virtual environment work. To use the virtual environment, we need to run a piece of this code, which will activate the virtual environment. At the terminal prompt, type:
* Windows 10: `myvenv\Scripts\activate.bat` 
* Windows 11: `myvenv\Scripts\activate`
* Mac OS: `source myvenv/bin/activate`

Activating the virtual environment allows us to go "inside" of it and install and use whatever packages we like, isolated from the rest of the system. You'll know it worked if the name of the virtual environment appears in parentheses somewhere in your terminal prompt (e.g., `(myvenv) PS C:\path\to\your\project>`).

To finish, we can install the packages we need to run the workshop materials. The packages we will need are:
* `notebook`: this will allow us to use Jupyter notebooks, which we'll explore more in the next section.
* `pandas`: a popular package for working with data.
* `matplotlib` and `seaborn`: two of the most popular packages for visualising data in Python.

To install these, we just need to type `pip install notebook pandas matplotlib seaborn` at the terminal prompt. (If this does not work, you may need to use `pip3 install notebook pandas matplotlib seaborn`). Make sure you keep this terminal window open, as we'll need it in the next section. 

And we're done—we're now ready to start running some Python code! 

#### Start the Jupyter notebook and the workshop materials

We're going to be running Python code inside something called a Jupyter notebook. This is a type of file that allows you to both write text and run Python code: as you'll see, this makes it very suitable for teaching materials! These are also a very popular file type for doing data science and data analytics.

To open a Jupyter notebook, go to the same terminal window where you activated your virtual environment and type `jupyter notebook`. You should now have a new tab open in your browser which looks something like below:

![jetbrains](/assets/img/tutorial/jupyter-notebook-browser.png)

Double-click on the file `1. Beginning with Python.ipynb`. This is a Jupyter notebook that contains the first part of the Humble Data workshop. Congratulations! You've finished all the set-up steps, and you're ready to start the workshop! Start reading the directions in the notebook to start working through the materials, and have fun!

#### (Optional) Use an IDE

As you can see, there are a lot of manual steps involved in getting a Jupyter notebook to run. Moreover, you'll need to complete all the steps between cloning the repo and starting the notebook from the terminal every time you want to start a new project. To make this (and many other coding tasks) easier, pieces of software called IDEs (integrated development environments) have been created to take care of a lot of these steps for you.

It's up to you whether you'd prefer to use an IDE or continue using the terminal. However, if you'd like to try out an IDE, one of the most popular is [PyCharm](https://www.jetbrains.com/pycharm/). This IDE is designed specifically for Python and has a free tier which will allow us to set up and work with the workshop materials.

To get started, first install PyCharm. You can find directions on how to install it [here](https://www.jetbrains.com/help/pycharm/installation-guide.html). You will automatically receive a 30-day trial to the Pro version, but after this expires you can continue to use the free version to work through this workshop.

Once PyCharm is installed, and you open it, you'll be shown the following landing menu. Select "Clone repository" from the top menu buttons.

![jetbrains](/assets/img/tutorial/new-pycharm-project.png)

You'll now see the following page. In the "URL" box, paste the repo containing the workshop materials (`https://github.com/HumbleData/beginners-data-workshop.git`). This is the same URL we used when we cloned the repo using the terminal. (As a reminder, to get this URL, we go to the [GitHub repo](https://github.com/HumbleData/beginners-data-workshop) containing the workshop materials, go to the "Code" button, and under the Clone tab select "HTTPS", then copy the URL.) In the "Directory" box, paste the path to the directory where you want to save your files for the workshop. Then press the `Clone` button at the bottom.

![jetbrains](/assets/img/tutorial/clone-project.png)

After this, you'll be presented with a dialogue box asking if you want to trust and open this project. Select `Trust Project`.

PyCharm will now be able to automatically create a virtual environment for you, provided you have Python installed on your computer. Moreover, it will spot that the repo contains a file called `requirements.txt`, which lists all the packages we need to install for the workshop. PyCharm will be able to use this file to automatically install the required packages, saving us from doing this step manually. You should see a dialogue box like the one below-just click `OK` and PyCharm will take care of the rest.

![jetbrains](/assets/img/tutorial/create-venv.png)

If you need to install any more packages in PyCharm (or for some reason, PyCharm does not install the required packages for you), you can do so using the "Python packages" tool window, as you can see below. For example, if we wanted to install a different visualisation package like Plotly (feel free to start playing with this once you finish the workshop!), we just need to type "Plotly" into the search box, select the package name from the list, and select `Install`. It will then be installed into the virtual environment. On top of all these nice features, PyCharm also remembers the virtual environment associated with your project, so the next time you open PyCharm and work on the workshop materials, the virtual environment will be ready to go.

![jetbrains](/assets/img/tutorial/packages-tool-window.png)

We're now set up and ready to work on the workshop materials! To do this, double-click on the first notebook (`1. Beginning with Python.ipynb`), and get started as per the instructions. And have fun!
