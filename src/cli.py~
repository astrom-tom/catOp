'''

catOp project 
-------------------
File: cli.py

This file configures the Command line interface 

@author: R. THOMAS
@year: 2018
@place:  ESO
@License: GPL v3.0 - see LICENCE.txt
'''

#### Python Libraries
import argparse

class CLI:
    """
    This Class defines the arguments to be calle to use SPARTAN
    For the help, you can use 'SPARTAN -h' or 'SPARTAN --help'
    """
    def __init__(self,):
        """
        Class constructor, defines the attributes of the class
        and run the argument section
        """
        self.args()

    def args(self,):
        """
        This function creates defines the 7 main arguments of SPARTAN using the argparse module
        """
        parser = argparse.ArgumentParser(description="catOp V1.0, R. Thomas, 2018, ESO, \
                This program comes with ABSOLUTELY NO WARRANTY; and is distributed under \
                the GPLv3.0 Licence terms.See the version of this Licence distributed along \
                this code for details.")

        parser.add_argument('catalog', help="Your first catalog of data to match this is mandatory (positionnal argument)")

        parser.add_argument('-n', choices = ['single', 'double'], help ='If you want to work on a single or double command, default=single', default = 'single')

        parser.add_argument('col', nargs='+', help ='Column name(s). If two columns are used, the format is- col1 col2 -')

        parser.add_argument('-o', '--operation', choices = ['m', 'a', 's', 'd'], help = 'If you use two column, the type of operation you want to perform:  m = multiplication; a = addition; s = subtraction; d = division')

        parser.add_argument('measurement', choices = ['mean', 'median'], help = 'Type of measurement you want to perform')
        
        parser.add_argument('error', choices = ['1s', 'MAD', 'Merr'], help = 'Type of error you want to compute')

        parser.add_argument('-t', '--threshold', nargs='+', help = 'Threshold to apply to the column values. You must enter vmin,vmax')

        parser.add_argument('-p', '--plot', action = 'store_true', help = 'if you want to plot the distribution at the end of the script. It will plot a simple histogram')

        ##### GET the Arguments for SPARTAN startup
        self.arguments = parser.parse_args()


