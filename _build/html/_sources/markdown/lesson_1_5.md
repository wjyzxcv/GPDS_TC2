(lesson_1_5)=
# Setting up FTP
::::{tab-set}
:::{tab-item} Windows
:sync: key1
```{margin}
- If you have already set up PuTTY, WinSCP should be able to import the settings and fill in `Host Name` automatically.
```
1. For the file transfer client, we recommend downloading **WinSCP**: https://winscp.net/eng/download.php
2. Open the .exe file and proceed with the installation process.
3. Open WinSCP
    ```{figure} ../pictures/lesson_1_5/winscp_1.png
    ```
4. Enter the following:
- File Protocol: SFTP
- Host Name: 130.34.234.40
- User name: *Your group username*
- Password: *Your group password*
    ```{figure} ../pictures/lesson_1_5/winscp_2.png
    ```
5. Check if you are connected (it shows /home/*groupname*)
    ```{figure} ../pictures/lesson_1_5/winscp_3.png
    ```
6. You can easily drag and drop files from and to your PC
    ```{figure} ../pictures/lesson_1_5/winscp_4.png
    ```

:::

:::{tab-item} Mac
:sync: key2
1. For the file transfer client, we recommend downloading **Cyberduck**:
https://cyberduck.io/download/
2. Open the .zip file and click & drop to the Applications folder.
    ```{figure} ../pictures/lesson_1_5/cyberduck_inst.png
    ```
3. Open Cyberduck and click **open connection**
    ```{figure} ../pictures/lesson_1_5/cyberduck_1.png
    ```
4. Enter the following:
- File Protocol: SFTP
- Server / Host Name: 130.34.234.40
- User name: *Your group username*
- Password: *Your group password*
    ```{figure} ../pictures/lesson_1_5/cyberduck_2.png
    ```
5. Check if you are connected (it shows /home/*groupname*)
    ```{figure} ../pictures/lesson_1_5/cyberduck_3.png
    ```
6. You can easily drag and drop files from and to your PC
    ```{figure} ../pictures/lesson_1_5/cyberduck_4.png
    ```
:::
::::