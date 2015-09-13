# simple-update

### Inroduction

simple-update is simple bash script that uses 'apt' to update your system, it even removes redundant packages! All you do is execute it as root and it runs the following commands;

* apt-get updates
* apt-get upgrade
* apt-get dist-upgrade

and lastly, with your permission,

* apt-get autoremove
* apt-get autoclean

### Why did I make this?

My younger sister is now a Linux user but she's not too tech savvy, as a result, she is unable to use the terminal fluently. I made this script and placed in her `/bin` folder so that to update and maintain her system, she only has to run `sudo simple-update`. It also makes my life a little easier too as it runs 5 commands, saving typing time.

### How can you trust me?

You have full access to the source code, comments and files. This allows you to read exactly what it does, allowing full transparency. I made this for my ease, I shared it because I'm nice.

### How do I install the script?

To install the script, you must simply download the file, from here you just run it. Putting it into a `/bin` folder will allow you to execute it by simply using `sudo simple-update` in a terminal, otherwise you have to navigate to it in the terminal and execute `sudo ./simple-update`. I'm going to explain how you install it into any folder, a `/bin` would be best for ease of execution.

1. Navigate to to the folder of your choicein the terminal, here is a list of the best `/bin` folders to use;

  * `/bin`
  * `/usr/bin`
  * `/usr/local/bin`

  `/bin` folders install the script system wide (for all other users), other than your `~/bin` folder or custom folders that are specific to your user.

2. Download the file using the `wget` command like so:

  `sudo wget https://raw.githubusercontent.com/JetLaggedEgg/simple-update/master/simple-update`

  You may have to be root to do so.

3. Correct the permissions for the script using `sudo chmod 755 simple-update`. You'll have to be in the directory the script is, otherwise point to the file where the file name is. i.e `sudo chmod 755 /point/to/file/simple-update`. This has to be done as you'll be running it as root.
