# Opening CLI



* **MacOS** -> open spotlight search (default way to do this is by hitting command and the space bar) and type in “terminal”. Select the application called terminal and press the return key. This should open up an app with a black background. When you see your username followed by a dollar sign, you’re ready to start using command line.
* **Linux** -> You can open Terminal by directly pressing \[+ALT+T] or you can search it up by clicking the “dash” icon, typing in “terminal” in the search box, and opening the Terminal application. Again, this should open up an app with a black background. When you see your username followed by a dollar sign, you’re ready to start using command line.
* **Windows** -> On Windows 10, open the start menu and go to the shortcuts folder called “Windows System”. Pressing the dropdown menu should reveal a shortcut to open the Command Prompt application. Right click on the shortcut, press “more”, and press “run as administrator”.
*   **Accessing Servers** -> If you run code on a server (e.g. a GPU cluster or something like Amazon Web Services), you need to be able to access the server. The best method to do this through Secure Shell (ssh), which lets you securely control and modify your server using the Internet. You can do this by typing in the following:

    ssh username@host\_server

    Where username is the account name of your account on the server, and host\_server is the host (e.g. GPU cluster’s name). If you have a password to access your account on the server, command line will prompt you to enter that in. If it’s your first time accessing that particular server, your computer may also ask you if it can remember the authenticity key — type in ‘yes’ or the corresponding phrase so that your computer doesn’t ask you this every time. When you’re linked up to the server, you should see that the command line starts with a green header with some kind of username@host format. Use this as an indicator that you’re really connected to the server
