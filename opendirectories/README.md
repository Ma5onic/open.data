**Contents**
----------
This data repository includes an sqlite database which contains all the URLs of 
linked posts submitted to the subreddit https://www.reddit.com/r/opendirectories. 
The URLs also include various other forms of associated data, including but not 
limited to the post title, score and submit date.

For those people only wishing to use the URLs and/or do not want to use sqlite, 
a text file has also been included as a substitute. This file only includes the 
URLs and any other data would have to be retrieved from the database file and 
therefore require the use of sqlite (see below).

The graph below is derived from the data provided above. Each dot below
represents a linked post submission at the subreddit. The x axis represents the 
date and time of the post and the y axis represents the total score of the post 
(upvotes - downvotes).

![Submit Date (Timecode) VS Score](figs/TIME_GMT_vs_SCORE.png)

**Updates**
---------

This repository will be update on the first of every month, whereby all the 
associated data files will be updated with new data obtained from the previous 
month. ID order is not guaranteed to be preserved.


**Access**
---------
If you are unfamiliar with programming then it is advised that you simply try to 
use the text file provided. If you require any of the other data fields in text 
form please get in contact with me at my github emails address.

The database file 'opendirectories.db' requires the use of sqlite to manipulate,
if you wish to simply view the database, proceed to the section following this 
one. sqlite3 comes as standard with python3, and this is the recommended option 
for beginners. The documentation concerning this module can be found [here](https://docs.python.org/3.5/library/sqlite3.html). It is imported as follows.

    >>> import sqlite3

If you wish to simply to view the database sqlitebrowser can be used. More 
information about sqlitebrowser can be found [here](http://sqlitebrowser.org/).
A few examples of how to install it are given below.

**Debian/Ubuntu**

    sudo apt install sqlitebrowser

**FreeBSD**

    sudo pkg install sqlitebrowser

**Fedora**

    sudo dnf install sqlitebrowser

**Arch**

    sudo pacman install sqlitebrowser

**MacOS x**

    brew cask install sqlitebrowser

**Windows**

Windows binaries can be downloaded from here:
https://github.com/sqlitebrowser/sqlitebrowser/releases

**Authors**
----------

Reuben Thorpe


