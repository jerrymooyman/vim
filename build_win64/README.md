# These are my custom build instructions for a windows x64 version.

I followed the instructions found [here](https://mgiuffrida.github.io/2015/06/27/building-vim-on-windows.html).    
I build from source for my personal environment:  
 * win10 (x64)  
 * python2.7 (x64)  

I use visual studio 2014, but had to install Win7 SDK to get nmake. 

# Convenience Scripts  
provided are the following scripts:  
 * config.cmd - contains build configurations, such as GUI, architecture, etc.  
 * build.cmd - contains the build commands  
 * copy-vim.cmd - copies the result into vim74 directory, which can then be
   copied to the default install location.  

# Building from Source  
 1. create a directory, doesn't matter where or what.  
 2. clone the git repo  
```sh
git clone https://github.com/jerrymooyman/vim.git  
```
 3. cd to build_win64  
 4. run config  
```sh
config.cmd  
```
 5. run build  
```sh
build.cmd  
```
 6. run copy-vim  
```sh
copy-vim.cmd  
```

If there are no errors, then you should end up with a vim74 directory in the
current directory.  

# gvim  
There is a custom gvimrc file (_gvimrc_example.jam).  
Rename this to _gvimrc and place in your home directory. It has the following basic settings:  
 * consolas font  
 * menus disabled  
 * scrollbars disabled   
 * annoying bell disabled  
 * jellybean color scheme (dark theme)  

