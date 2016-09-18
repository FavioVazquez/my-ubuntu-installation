# My ubuntu installation

Commands and programs I use when installing a fresh Ubuntu version. This a very useful installation if you are a programmer, but you have to get use to i3, is a window manager that will make your life easier, but there is a learning curve. You can find the docs in http://i3wm.org/docs/. This has been tested for Ubuntu 14.04 and 16.04. 

# Update and upgrade Ubuntu repos and libraries

```
sudo apt-get install update
sudo apt-get install upgrade
```

# Git 

``` 
sudo apt-get install git
``` 

# Vim

## Download the last version

``` 
git clone https://github.com/vim/vim.git
``` 

## Build Vim

**Note**: You may need to install this before building:

``` 
sudo apt-get install libncurses5-dev
sudo apt-get install libtinfo-dev
``` 

Make sure to run `make distclean` if you build Vim before.

Then 

``` 
cd vim
git pull
cd src
make
sudo make install
```

# Google Chrome

https://www.google.com/chrome/browser/desktop/index.html

```
sudo apt-get install libappindicator1
sudo dpkg -i google-chrome-stable_current_amd64.deb
```

# i3-wm

```
sudo apt-get update
sudo apt-get install i3-wm
sudo apt-get install i3
```

Use *Alt* as window manipulator.

I have a custom configuration file with some addons for i3. You can find it in 

https://github.com/FavioVazquez/dotfiles-linux-configurations/blob/master/dotfiles/config

Please read the docs if you want to understand this configuration file. You can prettify and customize the looks of i3, and for me one of the best explained tutorials is the one by [Nikhil Kumar](http://kumarcode.com/). It is not that easy to follow, but if you do it with care you will have a beatiful and useful skin for your i3-wm. You can find the tutorial in 
http://kumarcode.com/Colorful-i3/.

# Ranger 

Ranger is a console file manager with VI key bindings. It provides a minimalistic and nice curses interface with a view on the directory hierarchy. It ships with "rifle", a file launcher that is good at automatically finding out which program to use for what file type.

```
git clone https://github.com/ranger/ranger.git
```

And then buil it:

```
cd ranger
sudo make install
```

# Kupfer 

Kupfer is an interface for quick and convenient access to applications and their documents.

To install:

```
sudo apt-get install kupfer
```

Open Kupfer from terminal, in general mark "Start automatically on login". In Keyboard change the Show Main Interface with whatever you want. I use *Alt*+*D*.

# Kile 

Kile is a user-friendly TeX/LaTeX editor for the KDE desktop environment. KDE is available for many architectures and operating systems such as PC, Mac, and BSD, including Linux and Microsoft Windows.

The main features are:

- Compile, convert and view your document with one click.
- Auto-completion of (La)TeX commands
- Templates and wizards make starting a new document very little work.
- Easy insertion of many standard tags and symbols and the option to define (an arbitrary number of) user defined tags.
- Inverse and forward search: click in the DVI viewer and jump to the corresponding LaTeX line in the editor, or jump from the editor to the corresponding page in the viewer.
- Finding chapter or sections is very easy, Kile constructs a list of all the chapter etc. in your document. You can use the list to jump to the corresponding section.
- Collect documents that belong together into a project.
- Easy insertion of citations and references when using projects.
- Flexible and smart build system to compile your LaTeX documents.
- QuickPreview, preview a selected part of your document.
- Easy access to various help sources.
- Advanced editing commands.

To install (it is a big package):

```
sudo apt-get install kile
```
