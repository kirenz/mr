# Anaconda environment

This section contains an overview about the programming environments you will need for our course. 


## Create environment: mr

We install some modules in a new Anaconda environment. We call this new environment `mr` (for market research). 


> On *Windows* open the Start menu and open the "Anaconda Command Prompt". 

> On *macOS*: Open a terminal ([learn how to open a terminal](https://support.apple.com/guide/terminal/open-or-quit-terminal-apd5265185d-f365-44cb-8b09-71a064a42125/mac)) 


- Copy this code and run it in your terminal: 

```bash
conda create -n mr python=3.9 pandas openpyxl jupyter scikit-learn altair vega_datasets matplotlib seaborn vega altair_saver --y
```

Activate the new environment:

```bash
conda activate mr
```


## How to select your environment

In Visual Studio Code:

1. [Create or open a Jupyter Notebook](https://code.visualstudio.com/docs/datascience/jupyter-notebooks#_create-or-open-a-jupyter-notebook)

1. Next, select a kernel using the kernel picker in the top right (select the Anaconda environment)

![](https://code.visualstudio.com/assets/docs/datascience/jupyter/native-kernel-picker.png)


If you can't see your newly created environment:

You can also manually specify an interpreter if Visual Studio Code doesn't locate your kernel automatically.

1. Show command palette: Press `cmd+shift+p` (Mac) or `strl+shift+p` (Windows)

1. Search for `Python: Select Interpreter´

1. Select it and you should see a list of your virtual environments

1. Select the environment of your choice and you are ready to go.



If the steps described above should not work for you, take a look at other tips at [StackOverflow](https://stackoverflow.com/questions/43351596/activating-anaconda-environment-in-vscode).



