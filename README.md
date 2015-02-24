Useful commands and shortcuts
=============================

A collection of useful commands and keyboard shortcuts for Mac OSX and Linux. Mostly for my own reference but might also be useful for others :)


#### screenshots (Mac OSX)

`command-shift-3` : full screen

`command-shift-4` : selectable area

`command-shift-4` then `space` : single window


#### em dash (Mac OSX)

`option-shift-dash`


#### run app downloaded from internet (Mac OSX)

`control-click` then select `Open`


#### go to folder (in Finder, Mac OSX)

`command-shift-G`


#### connect to server

`ssh servername.uzh.ch` then enter password

`ssh -X servername.uzh.ch` if using GUI applications (then just launch apps as usual — requires XQuartz on Mac OSX)


#### find out where R libraries are saved

run R command `.libPaths()`


#### check Linux system/distribution info

`cat /etc/*-release`, `uname -a`

`nproc`, `lscpu`

`free`, `top`, `df -H`

`cat /proc/meminfo`, `cat /proc/cpuinfo`


#### check CPU cores (Mac OSX)

`sysctl hw.ncpu hw.physicalcpu hw.logicalcpu`


#### ls options

`ls -alh` : list files — including hidden files and directories (-a), long format details (-l), and human readable file sizes (-h)


#### show disk usage of directories

`du -ahc --max-depth=1`


#### check file type

`file <filename>` : for example to check which type of compressed file


#### number of lines in a text file

`wc -l <filename>` : stands for word count, number of lines


#### create symbolic link

`ln -s <target> <name>` : creates a symbolic/soft link called `name` pointing to the file `target`


#### set path

`export PATH=~/new_directory:$PATH` (paste in `.bash_profile` or `.bashrc` file; note order of terms matters — first has highest priority)


#### install program in home directory (Linux)

`wget http://address.of.file/filename.tar.gz` : download .tar.gz source archive (run in `/home/username/src` folder to save it there)

`tar xfvz filename.tar.gz` : uncompress .tar.gz source archive (run in `home/username/src`)

`cd filename` : go to uncompressed source directory

`./configure --prefix=$HOME` : run configure script (performs installation checks and creates Makefile)

* **IMPORTANT**: include the option `--prefix=$HOME` to install the program in your home directory instead of the default Linux binary directories

`make` : run Makefile (compiles the program and creates executables)

`make install` : run install part of Makefile (copies executables into directories)


#### GNU screen

GNU screen is useful when working on a server, since programs running in a screen session will continue to run even if the server connection is interrupted.

`screen` or `screen -S <name>` : create new screen session (with optional name)

`screen -x` or `screen -r <name>` : attach to running screen session (with optional name)

`exit` : close session

`screen -ls` : list running screen sessions

full list of screen commands: http://aperiodic.net/screen/quick_reference


#### git/GitHub — set up a repository

`git init` to create local repository in a folder

manually create `README.md`, `.gitignore`, and `LICENSE` files

`git remote add origin https://github.com/user/repository-name.git` (paste repository address from GitHub)

`git add .` to add new files


#### git/GitHub — commit changes

`git add .` (if no new files can skip this and go straight to commit)

`git commit -am "commit message"` to commit

`git push -u origin master` to push to GitHub


#### git/GitHub — pull changes

`git pull origin` (merges into local repository)


#### git/GitHub — undo commit

`git reset --soft HEAD^` : Use this to undo the previous commit if it hasn't been pushed to GitHub yet, for example if you have added the wrong files or want to change the commit message.

