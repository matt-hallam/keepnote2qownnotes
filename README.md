# keepnote2qownnotes

## Description
Script to convert a [keepnote](http://keepnote.org/) directory structure to one suitable for [QOwnNotes](https://www.qownnotes.org)

With keepnote sadly no longer maintained, and increasingly difficult to install on modern distros, I decided to move to QOwnNotes. I created this simple script to port my existing notes over

## Prerequisites
- Python 3
- html2text utility (or some equivalent, edit the script as necessary)

## Usage
No installation is necessary. This is a standalone script, just download and run it in your keepnote notes directory.

Make a backup of your keepnote notes - This process is not reversible. It will convert the directory tree in place.

Change into your keepnote directory and run the script: `keepnote2qownnotes`

After conversion, add the directory to QOwnNotes:

- Note > Setup Note Folders > Add folder
- Point the folder path to your directory 
- Make sure "Use note subfolders" is checked

## Formatting
The main goal of this script is to convert the directory structure of a keepnote note directory into something suitable for QOwnNotes to use. 

html2text is used to convert those notes themselves.   
Whilst it does preserve some of the formatting in markdown, not all is.  

Since the formatting available within keepnote is very limited anyway, this wasn't an issue for me and html2text was chosen as it is a widely available tool. You may wish to investigate more dedicated converters like html2markdown. 
