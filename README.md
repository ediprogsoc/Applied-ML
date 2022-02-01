# Applied Machine Learning
Repository containing materials for the Programming Society applied machine learning curriculum.

## Getting Set Up

The following will walk you through creating an environment in which you will be able to run all the code we use in the machine learning sessions. This way, you do not need to worry about installing libraries and dependencies, and have a consistent setup with us and other members, so we can easily troubleshoot.

Make sure you have `anaconda` (or `miniconda`) installed on your system. Click [here](https://docs.anaconda.com/anaconda/install/index.html) to install if you don't. You should be able to run

```console
conda --version
```
in a terminal session and get a version number out.

Next, run
```console
conda env create -f environment.yml
```

and accept the defaults when prompted. You should now have the environment successfully set up!

## Running Code

We need to activate the environment before using it. **This needs to be done every time you open a new terminal session**.

```console
conda activate applied-machine-learning
```

You should now see the text `(applied-machine learning)` appear before your standard shell prompt in the terminal window.

You can now run python scripts which use the libraries discussed in the sessions. You are free to edit/run these however you wish, but we recommend using JupyterLab, as described below.

### JupyterLab

Make sure you are in this directory in the terminal and then run the command

```console
jupyter lab
```
This should open a web browser where you will be presented with a screen like this:

![JupyterLab Launcher](https://doc.cocalc.com/_images/jlab-launcher.png)

On the left are the files and folders in the current directory. On the right is an option to create a new file. To create a new notebook, make sure to select the option under the heading **Notebook** that says `Python [conda env:applied-machine-learning]`. Otherwise just open an already existing file by clicking on it on the left.

Type code in cells and use the keyboard shortcut `Shift + Enter` to run them. Happy Coding!

## Tips

To get `.md` files to display correctly in jupyterlab, go to *Settings -> Advanced Settings Editor -> Document Manager* and replace the `{}` in the pane marked *User Preferences* with:

```json
{
defaultViewers:{
    markdown: "Markdown Preview"
    }
}
```
Why this isn't default is incredible...