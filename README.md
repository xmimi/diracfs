This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY.

Author :  Xiabo Li <li.xiabo@gmail.com>

-----------------------
version : 2.1
DIRAC release : v6r12p16
Date : 27 Jan 2015

correction double / of pathname in old DIRAC

------------------------
version : 2.0
DIRAC release : v6r11p6
Date : 15 Jul 2014

global temporary file handler change to dict()
do not delele-recreate remote file if there is no modification
  (cat, more, less, tail)
added mount option : -o SE=<dirac storage element>
file/directory access permission sync

commands compatibility:
  mv : - globaly works for files, for directory better to copy to local then
         copy to remote path and delete local copy (fuse/fuse-python bug?)
       - cannot overwrite existing file in same directory : dirac GUID
  vi(vim, gvim) : work although better to set swap file/directory to local path
  emacs : work as vi
  cp [-r]
  stat
  chmod [-R]

------------------------
version 1.1
DIRAC release : v6r11p6
Date : 25 Jun 2014

Commands compatible/tested/working with this version :
  mkdir [-p]
  rmdir
  rm [-rf]
  cp
  ls [-lha -R]
  cat
  less
  more
  tail
  echo >  >>
  nano
  du [-sh]
  find -name -print
  xpdf
  eog
  tar [tzf] [tjf]

