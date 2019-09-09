# Homework 2: Pacman
Welcome to the Pacman portion of Homework 2! At the end of this portion of the assignment, you will get to see your search algorithms play out in front of you as Pacman searches for food.  Below are the installation instructions.  As always, please try to figure out problems you may have before bringing them to Piazza or office hours. If you're stuck, we're here to help.  You should have no problem getting the program working on CAEN.  However, because we understand that many students will prefer to do this project outside of the CAEN labs, we provide instructions below and the support for using an Ubuntu VM created in VirtualBox to develop for this project.  You are welcome to use another system to develop your code, but support will be offered only for CAEN and the Ubuntu VM we describe below.  If your program runs on one of these two systems, it will certainly run in our grading environment.

## Ubuntu VM Installation
Note: this process will take up to 20 minutes
Follow these [instructions](https://www.dev2qa.com/how-to-install-ubuntu-on-virtualbox-mac/) to get an Ubuntu VM running through virtualbox on your computer (note: the Ubuntu image download is ~2 GB.  If you have internet constraints at home, best to do this on MWireless).  It is recommended to download Ubuntu 18.04.3.

Note: you can "install ubuntu" or "try it".  Either will work for this assignment.  Installing Ubuntu is helpful if you plan on using this VM long term, or would like to make [copy paste](https://apple.stackexchange.com/questions/132233/copy-and-pasting-between-host-and-vm) available from your host system to your VM. Here are a few pointers if you would like to do this:
* Step 8: choose "Install Ubuntu"
* Step 10: choose "Minimal installation" - takes far less time, and for the purposes of this assignment you won't need the other programs included.
* Step 11: choose "Erase disk and install Ubuntu".  You will see a scary warning message saying it will delete all your files.  It is referring to the virtual drive you're  creating, not the host (your computer).    

## Downloading the repo and installing dependencies
```
sudo apt install git
git clone https://github.com/abwilf/HW2_Pacman.git
cd HW2_Pacman
sudo apt-get install python3-tk
sudo apt install python3-pip
```
Note: the staff has encountered some behavior where this last step fails.  If you see an error along the lines of `Unable to locate package python3-pip`, here is a [fix](https://askubuntu.com/questions/1061486/unable-to-locate-package-python-pip-when-trying-to-install-from-fresh-18-04-in).  Make sure to use `sudo apt install python3-pip` instead of `python-pip` as the fix recommends.

Then, 
```
pip3 install future
```
Note: if this last step fails, and you may need this [fix](https://askubuntu.com/questions/1061486/unable-to-locate-package-python-pip-when-trying-to-install-from-fresh-18-04-in).

To test that all the dependencies worked, run this command and play pacman.  If this works, you can get started coding and testing.
```
python3 pacman.py
```

## Testing Your Code
The staff has provided some test cases for you to test your code in `test.py`.  Run `python3 test.py` to test them.  Note that these are *not comprehensive*.  Your grade will be based partially on these test cases, but will also be based on a larger suite of hidden test cases.  For this reason, we strongly recommend that you write your own test cases.

## Credit
All credit for this portion of the homework goes to [UC Berkeley’s CS188](http://ai.berkeley.edu).