### Table of Contents
[Home](README.md)
[Reading Day 2](day2.md)

This is where I document my reading for this lab.

#### Choosing a Text Editor

- We'll be writing a lot of code, a good text editor will be invaluable
- Text editor is entirely a personal choice, they're all pretty similar
  -  As long as the text editor you choose can complete a website to your liking
- **What is a text editor?**
  -  A piece of software that lives online, allowing you to write and edit text and build a website
  -  Super important for people learning to create websites
- Some important features:
  - Code completion
    -  Like predictive text and autocorrect on your phone, but with code
  - Syntax highlighting
    - Important elements are color-coded to make writing code simpler
    - Makes code easier to read, and helps you find what you're looking for
  - Variety of themes
    - Some themes (darker ones especially) can reduce eye strain
  - Extension choice
    - Adds functionality as you learn more coding techniques
- Always code in **plain text**. Your text editor shouldn't allow you to change font sizes, add italics, etc.
- Use proper file extension names
  - .html for HTML files
  - .css for CSS files
- **Third party text editors**
  - Notepad++
    - Windows only
    - Free
  - TextWrangler/BB Edit
    - Mac only
    - TextWrangler is defunct, BB Edit costs money ($50)
  - Visual Studio Code
    - Windows, Mac, and Linux compatible
    - Free
  - Atom
    - Windows, Mac, and Linux compatible
    - Free
    - Created by GitHub
  - Brackets
    - Windows, Mac, and Linux compatible
    - Free
    - Created by Adobe
  - Sublime Text
    - $70 for full version 
- Integrated Development Environment (IDE)
  - Combines features like these:
    - Text editing
    - File Management
    - Compiling
    - Debugging
  - Microsoft Outlook is a good example 

# Cheat Sheet for Terminal Use

- `pwd` shows you your current directory
- `ls` shows you what files are in your current directory
  - `ls [options] [location]` is how it is usually formatted
- `ls -l` shows a long listing
- `ls /etc` shows directory's *contents*
- `ls -l /etc` shows both a command line option and argument
- `~` is a shortcut to your home directory
- `.` references your current directory
- `..` references parent directory
- `cd [location]` changes your directory
- `file [path]` shows what type of file something is
- `ls -a` shows hidden files

# Other Notes

#### The Command Line

- A command is usually the first thing you type
- `echo` displays a system variable
- You can navigate and edit previous commands using the arrow keys

#### Basic Navigation

Paths
- A path is a means to get to a particular file or directory on the system 
- Absolute paths
  - Show location in relation to root directory
  - Start with a forward slash (/)
- Relative
  - Specify a location relative to where you are in the system
  - Do not begin with a slash

- Tab completion is a form of autocorrect. Can be invoked by pressing **tab**

#### About Files
- A computer sees **everything** as a file
- Case sensitivity **matters**
- If moving a file into a folder that contains a space (e.g., "Honeymoon Pics"), make sure to put that directory in single quotes
  - Otherwise the space is seen as a separate command
  - An "escape character" (\) works as well
    - This would appear as "Honeymoon\ Pics"
  - Tab completion does this for you!
