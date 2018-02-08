'''
The catOp Project
-------------------
This file configures the messages passed to the user


@author: R. THOMAS
@year: 2018
@place: ESO
@License: GPL v3.0 - see LICENCE.txt
'''


####Python Libs
import os

def Error(message, toline):
    """
    This function display an error message. After such a message
    SpArtan must quit

    Paramters:
    ---------
    message:    str,Message to be displayed
    toline:     str,Carriage return or not before the message(Yes or No)

    Returns:
    -------

    """
    if toline == 'Yes':
        print('\n'+ '\033[1m' + '[ERROR]:   ' + message + '\033[0m')
    else:
        print('\033[1m' + '[ERROR]:\t' + message + '\033[0m')

def Warning(message, toline):
    """
    This function display an warning message.
    This message does not lead to the end of SPARTAN

    Paramters:
    ---------
    message:    str,Message to be displayed
    toline:     str,Carriage return or not before the message(Yes or No)

    Returns:
    -------

    """

    if toline == 'Yes':
        print('\n'+ '\033[1m' + '[WAR]:\t' + message + '\033[0m')
    else:
        print('\033[1m' + '[WAR]:\t' + message + '\033[0m')

def Info(message, toline):
    """
    This function display an information message.

    Paramters:
    ---------
    message:    str,Message to be displayed
    toline:     str,Carriage return or not before the message(Yes or No)

    Returns:
    -------

    """
    if toline == 'Yes':
        print('\n'+ '\033[1m' + '[INF]:\t' + message + '\033[0m')
    else:
        print('\033[1m' + '[INF]:\t' + message + '\033[0m')
