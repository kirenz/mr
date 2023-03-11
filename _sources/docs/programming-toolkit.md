# Programming toolkit

This section contains an overview about the programming toolkit you will need for our course. 

You will need to install:

1. the latest version of Anaconda (includes Python and some toolkits) 
2. Visual Studio Code (a code editor)

Please read the following instructions.

---

(anaconda)=
## Anaconda

The open-source Anaconda Individual Edition is one of the easiest ways to get started with data science projects. It is a data science toolkit which already includes most of the data science modules we need.


### Uninstall your old version

To avoid compatibility problems with older versions of Anaconda, I recommend to uninstall Anaconda and install the latest version.

#### Windows


```{admonition} To do
:class: tip

1. Open the file explorer.
1. Delete your environment (anaconda3\envs) and package (anaconda3\pkgs) folders in your user folder.
1. Open Add or remove programs and uninstall your Anaconda installation.

```

#### macOS


> Open your terminal ([learn how to open your terminal](https://support.apple.com/guide/terminal/open-or-quit-terminal-apd5265185d-f365-44cb-8b09-71a064a42125/mac))


````{admonition} To do
:class: tip

Remove your entire Anaconda directory with `rm -rf`. 

If you are not sure where anaconda is installed, simply enter all commands:

First try the opt folder:

```bash
rm -rf ~/opt/anaconda3
```

Then this location:

```bash
rm -rf anaconda3
```

Finally, enter:

```bash
rm -rf ~/anaconda3
```

````

### Install Anaconda

Install the latest version of the Anaconda Individual Edition:

```{admonition} To do
:class: tip

- [💾 Anaconda installation](https://www.anaconda.com/products/individual)

```


### Use conda-forge

Instead of the conda default package manager, we want to use the community-led alternative `conda-forge` to install Python modules.


> On *Windows* open the Start menu and open the "Anaconda Command Prompt". 


> On *macOS*: Open your terminal ([learn how to open your terminal](https://support.apple.com/guide/terminal/open-or-quit-terminal-apd5265185d-f365-44cb-8b09-71a064a42125/mac))



````{admonition} To do
:class: tip

Type this in your terminal to add `conda-forge`:

```bash
conda config --add channels conda-forge
```

Then make `conda-forge` the priority channel: 

```bash
conda config --set channel_priority strict
```

````

---

(vscode)=
## Visual Studio Code 
 
Visual Studio Code is a code editor that can be used with a variety of programming languages including Python.


### VS Code installation

Install VS Code:

:::{warning}
Move VS Code to the Applications ("Programme") folder after you have downloaded it.
:::


```{admonition} To do
:class: tip
- 💾 Install [VS Code](https://code.visualstudio.com/)  

Download ➜ Move to Applications ("Programme") folder ➜ Double Click

```


### Install extensions

VS Code extensions let you add tools to your installation to support your development workflow.


```{admonition} To do
:class: tip

- 💾 Install the [Python extension](https://marketplace.visualstudio.com/items?itemName=ms-python.python)

```

<!--
- 💾 Install the [Live Share Extension Pack](https://marketplace.visualstudio.com/items?itemName=MS-vsliveshare.vsliveshare-pack)
-->

Now close and restart VS Code.

### Jupyter Notebook extension

We usually work with Jupyter Notebook files in VS Code. 

```{admonition} To do
:class: tip

- 💾 Install the [Jupyter extension](https://marketplace.visualstudio.com/items?itemName=ms-toolsai.jupyter)

```

Now close and restart VS Code.

Open a Juptyer Notebook in VS Code:

```{admonition} To do
:class: tip
- Learn how to use [Jupyter Notebooks in VS Code](https://code.visualstudio.com/docs/datascience/jupyter-notebooks)
```

If you can't select a kernel (like the so called `base` kernel), try to close and restart VS Code once again.

---
