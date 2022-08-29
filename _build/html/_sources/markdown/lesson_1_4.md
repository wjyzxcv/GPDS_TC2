(lesson_1_4)=
# Introduction to Terminal

::::{tab-set}
:::{tab-item} Windows
:sync: key1
1. Make sure you are connected to the VPN.
2. Download PuTTY:
https://www.putty.org/
3. Open the installer and proceed with the installation process.
4. Open PuTTY and enter `130.34.234.40` in **Host Name (or IP address)**. To save the setting for later use, enter a name for this configuration in **Saved Sessions**, then press **Save**.
    ```{figure} ../pictures/lesson_1_4/putty_1.png
    ```
5. Press **Open** to start the connection. 
6. Type `your group name`.
    ```{figure} ../pictures/lesson_1_4/putty_2.png
    ```
7. Type `your group password`.
    ```{figure} ../pictures/lesson_1_4/putty_3.png
    ```
8. When you see the $ symbol, it means you can start using Linux commands.
    ```{figure} ../pictures/lesson_1_4/putty_4.png
    ```
:::

:::{tab-item} Mac
:sync: key2
1. Make sure you are connected to the VPN.
2. Open the terminal.
    ```{figure} ../pictures/lesson_1_4/mac_term.png
    ```
3. Type `ssh groupname@130.34.234.40`
    ```{figure} ../pictures/lesson_1_4/mac_ssh_1.png
    ```
4. Type `your group password`
    ```{figure} ../pictures/lesson_1_4/mac_ssh_2.png
    ```
5. When you see the $ symbol, it means you can start using Linux commands.
:::
::::

## Practice 0
Log-in using ssh with your group ID and password.
:::{admonition} Expected output
```{figure} ../pictures/lesson_1_4/Practice_0.png

```
:::


## Practice 1
Print the working directory, make a folder with your name, list the folders in your group, then enter your folder.

```{margin}
- `pwd`: print working directory
- `mkdir *dirname*`: make directory
- `ls`: list files
- `cd *dirname*`: change directory 
```
:::{admonition} Expected output
```{figure} ../pictures/lesson_1_4/Practice_1.png

```
:::


## Practice 2
Inside `yourname` folder, make folders called `local` and `scripts`. Then, go back to the home folder with `cd`. From the home folder, make a folder called `python` inside folder `scripts`. Check if the folder is actually there.

:::{admonition} Expected output
```{figure} ../pictures/lesson_1_4/Practice_2.png

```
:::

## Practice 3
Without typing, press up (and down) until you see just `cd` then ENTER. Then, try to enter your folder by typing `SPACE + (first letter of your name)` then press tab.

```{margin}
- `up arrow` key: show the previous command you entered
- `down arrow` key: show the next command you entered
- `tab` key: autocompletion
```

:::{admonition} Expected output
```{figure} ../pictures/lesson_1_4/Practice_3_1.png
```
```{figure} ../pictures/lesson_1_4/Practice_3_2.png
```
```{figure} ../pictures/lesson_1_4/Practice_3_3.png
```
:::

## Practice 4
From the `home` directory, check all the hidden files by typing `cd+SPACE+TAB+TAB`. Then, also check what folders are inside yourname folder.

```{margin}
- `double tab`: see inside the folder/command without pressing `ENTER`
```
:::{admonition} Expected output
```{figure} ../pictures/lesson_1_4/Practice_4_1.png
```
```{figure} ../pictures/lesson_1_4/Practice_4_2.png
```
```{figure} ../pictures/lesson_1_4/Practice_4_3.png
```
:::
