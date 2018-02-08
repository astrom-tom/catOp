# catOp
This tool is a very simple way to make operation between different columns in a given catalog and give very basic statistic about the columns.


The help of the program will help you to get started 
```
#########################################
##  catOp: Quick Catalog Manipulation  ##
##        and basic statistics         ##
##        Astrom-tom @ GitHub          ##
##           2018 @ Paranal            ##
#########################################

usage: catOp [-h] [-n {single,double}] [-o {m,a,s,d}]
             [-t THRESHOLD [THRESHOLD ...]] [-p]
             catalog col [col ...] {mean,median} {1s,MAD,Merr}

catOp V1.0, R. Thomas, 2018, ESO, This program comes with ABSOLUTELY NO
WARRANTY; and is distributed under the GPLv3.0 Licence terms.See the version
of this Licence distributed along this code for details.

positional arguments:
  catalog               Your first catalog of data to match this is mandatory
                        (positionnal argument)
                        
  col                   Column name(s). If two columns are used, the format
                        is- col1 col2 -
                        
  {mean,median}         Type of measurement you want to perform
  
  {1s,MAD,Merr}         Type of error you want to compute

optional arguments:
  -h, --help            show this help message and exit
  
  -n {single,double}    If you want to work on a single or double command,
                        default=single
                        
  -o {m,a,s,d}, --operation {m,a,s,d}
                        If you use two columns, the type of operation you want
                        to perform: m = multiplication; a = addition; s =
                        subtraction; d = division, it will to 
                        --col1 operation col2--
                     
  -t THRESHOLD [THRESHOLD ...], --threshold THRESHOLD [THRESHOLD ...]
                        Threshold to apply to the column values. You must
                        enter vmin,vmax
                        
  -p, --plot            if you want to plot the distribution at the end of the
                        script. It will plot a simple histogram


```

An example of command:
```
catOp cat.txt -n double NUV-GALEX_Abs MNUV median MAD -o s -t -10 10
```
