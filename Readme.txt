This code is free to use/modify/distribute.
I do not provide warranty for this code. it is open and free. Period.

thanks.

Notice:
This was created for and tested on Ubuntu 14.04 server 64bit with screen.
Although it should work on most if not all newer Linux 64bit debain based distros with screen.
If you don’t know what screen is… you probably shouldn’t be reading this. :)
But if you don’t, just make sure you have it installed.
Or install it with:

sudo apt install screen
 
Or my favorite, Byobu which includes screen and is much better (in my opinion):
 
sudo apt install byobu

Also, have McMyAdmin working before using this, this is for autorun and control of McMyAdmin from the command line and/or ssh.
 
Use your favorite editor (I prefer nano) to create file called "mcma" in /etc/init.d/

cd /etc/init.d
sudo nano mcma

and paste the code in that file.

Edit the USERNAME=minecraft variable according to your setup.
(Replace "minecraft" with your username.)

Make sure the newly created file has the required permissions.

sudo chmod a+x /etc/init.d/mcma

then install the script with:

sudo update-rc.d mcma defaults 99 01
 
if you need to remove the script use:

sudo update-rc.d -f mcma remove



PS: this assumes a default install of mcmyadmin using their directions. If you made any changes then this may not work. 
But if you did make changes, then you should know how to make this work anyway.... right?  :)
Enjoy.

