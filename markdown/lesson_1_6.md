(lesson_1_6)=
# Setting up Anaconda & virtual environment
## Installing Anaconda
Anaconda is a Python and R distribution. It aims to provide everything you need for data science "out of the box".

### Practice 5
Make sure you are inside `yourname` folder. Download the Anaconda installer by copying the following link and pasting it in your terminal. 

```{margin}
- `wget`: download file
```
```{admonition} Url
https://repo.anaconda.com/archive/Anaconda3-2022.05-Linux-x86_64.sh
```

:::{admonition} Expected output
```{figure} ../pictures/lesson_1_6/Practice_5_1.png
```
```{figure} ../pictures/lesson_1_6/Practice_5_2.png
```
```{figure} ../pictures/lesson_1_6/Practice_5_3.png
```
:::

### Practice 6
To see if you download it correctly, try to list the contents of your folder now using **ls**.
:::{admonition} Expected output
```{figure} ../pictures/lesson_1_6/Practice_6.png
```
:::

If you see Anaconda3-2022.05-Linux-x86_64.sh, this means you downloaded the file correctly.

### Practice 7
Using your mouse, you can select the installer file name then copy it using `Ctrl+C`. Then, use `sh filename` to run the Anaconda installer.

```{margin}
- `sh *filename*`: execute/run file
```
:::{admonition} Expected output
```{figure} ../pictures/lesson_1_6/Practice_7_1.png
```
```{figure} ../pictures/lesson_1_6/Practice_7_2.png
```
```{figure} ../pictures/lesson_1_6/Practice_7_3.png
```
:::

### Practice 8
Don't install Anaconda in `/home/*groupname*/anaconda3`. Set the installation folder to be `/home/*groupname*/*yourname*/local/anaconda3`.
:::{admonition} Expected output
```{figure} ../pictures/lesson_1_6/Practice_8_1.png
```
```{figure} ../pictures/lesson_1_6/Practice_8_2.png
```
```{figure} ../pictures/lesson_1_6/Practice_8_3.png
```
```{figure} ../pictures/lesson_1_6/Practice_8_4.png
```
:::
### Practice 9
Start with typing `source .bashrc` from home folder to launch the shell instance. Then, use `conda -V` and `conda update conda` to update the current version.

```{margin}
- `source .bashrc`: launch an interactive shell instance
- `conda -V`: check `conda` is installed and in your `PATH`
- `conda update conda`: check `conda` is up to date
```

:::{admonition} Expected output
```{figure} ../pictures/lesson_1_6/Practice_9_1.png
```
```{figure} ../pictures/lesson_1_6/Practice_9_2.png
```
```{figure} ../pictures/lesson_1_6/Practice_9_3.png
```
```{figure} ../pictures/lesson_1_6/Practice_9_4.png
```
:::

## Setting up virtual environment
The main purpose of Python **virtual environments** is to create an isolated environment for Python projects. This means that each project can have its own dependencies, regardless of what dependencies every other project has.

### Practice 10
Using `conda`, make a new virtual environment (`yournameenv`) and activate it.

```{margin}
- `conda create -n *yourenvname* python=3.x anaconda`: create new virtual environment with Python 3.x.
- `conda activate *yourenvname*`: activate your virtual environment
```

:::{admonition} Expected output
```{figure} ../pictures/lesson_1_6/Practice_10_1.png
```
```{figure} ../pictures/lesson_1_6/Practice_10_2.png
```
```{figure} ../pictures/lesson_1_6/Practice_10_3.png
```
```{figure} ../pictures/lesson_1_6/Practice_10_4.png
```
:::

### Practice 11
Try to `exit` the current server to go back to your computer. Try to enter again with up arrow, and re-activate your virtual environment. Finally, exit one more time.

```{margin}
- `exit`: exit the current active server
```
:::{admonition} Expected output
```{figure} ../pictures/lesson_1_6/Practice_11.png
```
:::
