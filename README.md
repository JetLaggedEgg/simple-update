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

My younger sister is now a Linux user but she's not too tech savvy, as a result, she is unable to use the terminal fluently. I made this script and placed in her `/bin` folder so that to update and maintain her system, she only has to run `sudo simple-update`.

### How can you trust me?

You have full access to the source code, comments and files. This allows you to read exactly what it does, allowing full transparency. I made this for my ease, I shared it because I'm nice.

### How do I install the script?

All you need to do is download the `simple-update` file and place it in your `/bin` folder. In order to do so, you will have to be root or use `sudo`.

1. Download the file. Download the script from this repository.

2. Moving it. Move the file if needed, putting it the `/bin` folder allows to you most simply execute it using the following command: `sudo simple-update`. Use the following command to move the file, replacing the caps text and square brackets with the directory path you downloaded it to. You could also change the `/bin/` to your own new location if you want.
`sudo mv /[DIRECTORY THE FILE IS IN]/simple-update /bin/`

3. Preparing it. Once it's in a location of your choice, you will have to set the file's permissions to allow it to execute. You can do this with the following command: `sudo chmod 755 /bin/simple-update`. Change the path to your custom location if you had one.

4. Running it. If the file in your `/bin`, just run `sudo simple-update`, if it is in a custom directory, either change directory to it and run `./simple-update` or just run `./[DIRECTORY-PATH]/simple-update`, changing the caps text and square brackets to the path you saved the file at.

5. Optionally, you can install figlet to make it look nicer. I use a figlet logo if you have it installed but you don't have to. You can install figlet by running `sudo apt-get install figlet`.
