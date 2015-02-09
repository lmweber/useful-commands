Useful commands and shortcuts
=============================

A collection of useful commands and keyboard shortcuts for Mac OSX and Linux. Mostly for my own reference but might also be useful for others :)


#### screenshots (Mac OSX)

`command-shift-3` : full screen

`command-shift-4` : selectable area

`command-shift-4` then `space` : single window


#### run app downloaded from internet (Mac OSX)

`control-click` then select `Open`


#### connect to server

`ssh servername.uzh.ch` then enter password

`ssh -X servername.uzh.ch` if using GUI applications (then just launch apps as usual — requires XQuartz on Mac OSX)


#### check CPU cores

`sysctl hw.ncpu hw.physicalcpu hw.logicalcpu`


#### check Linux system/distribution info

`cat /etc/*-release`

`uname -a`

`free`

`top`

`cat /proc/meminfo`

`cat /proc/cpuinfo`


#### ls options

`ls -alh`


#### set path

`export PATH=~/custom_directory:$PATH` (paste in `.bash_profile` or `.bashrc` file; note order of terms matters — first has highest priority)


#### git/GitHub — set up a repository

`git init` to create local repository in a folder

manually create `README.md`, `.gitignore`, and `LICENSE` files

`git remote add origin ...` (paste address from GitHub)

`git add .` to add new files


#### git/GitHub — commit changes

`git add .` (if no new files can skip this and go straight to commit)

`git commit -am "commit message"` to commit

`git push -u origin master` to push to GitHub

