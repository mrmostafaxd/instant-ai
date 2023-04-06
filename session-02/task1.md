# Task 1
## Table of Contents
- [Description](#description)
- [Enable auto-completion](#enable-auto-completion)
- [Display run-time](#display-run-time)

## Description
How to enable auto-completion (without pressing `tab`) and display execution time in Jupyter Notebook.

## Enable auto-completion
### Description
The following 2 methods will enable auto-completion without pressing **Tab**:
- [How to enable auto-completion 1](#how-to-enable-auto-completion-1)
- [How to enable auto-completion 2](#how-to-enable-auto-completion-2)

### How to enable auto-completion 1
#### Open Anaconda Navigator
You can open it by searching for it in windows search bar
![search image](./images/img-01.png)
#### Go to Environment tab and select the desired Conda Environment
In this case it is base(root)
![select enivronment](./images/img-02.png)
#### Click on the green button shown below and click on Open terminal
![click on Open Terminal](./images/img-03.png)
#### Paste the following command in the terminal and press Enter
`pip install jupyter_contrib_nbextensions && jupyter contrib nbextension install`

![terminal with command image](./images/img-04.png)

#### After it finishes downloading the necessary packages Open Jupyter notebooks, it will show an additional tab called *Nbextensions*
![Jupyter notebook tabs](./images/img-05.png)

#### Press on the tab then uncheck the marked checkbox
![uncheck box](./images/img-06.png)
#### Search in the filter for `hinterland` then check the highlighted checkbox 
This will enable Hinterland which is the extension for auto-completion without pressing tab
![enable hinterland](./images/img-07.png)

[(return to top)](#task-1)

### How to enable auto-completion 2
#### Open new jupyter notbook and run the following commands in separate cells
`!pip install jupyter_contrib_nbextensions && jupyter contrib nbextension install --user`

`!jupyter nbextension enable hinterland/hinterland`

![2 commands in jupyter notebook](./images/img-08.png)

[(return to top)](#task-1)

<hr>

### Display Run-time
#### Follow the [first method](#how-to-enable-auto-completion-1) of installing the auto-completion extension till [this step](#search-in-the-filter-for-hinterland-then-check-the-highlighted-checkbox), where you will instead search for `executetime` and enable it.
![enable executetime](./images/img-09.png)

[(return to top)](#task-1)
