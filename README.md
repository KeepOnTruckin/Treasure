# Treasure
A simple z/OS Mainframe game written in REXX.

Back in the early 1980s home computers were new and there were lots of different models available on the market. There was the ZX81, the Specturm 48K, the BBC Micro, the Electron, the VIC-20, the Commodore 64, the Atari 800, or how about lesser none ones such as the Jupiter Ace, Dragon 32 or even the derided Mattel Aquarius. What all these machines had in common was they came with a BASIC Interpreter. BASIC is a computer language that is virtually unheard of now, but back then it was as popular as, say Python is today.

Usborne Books published a series of books on home computing including several on how to program in BASIC (they even published one on coding in machine code). These proved very popular with a generation of young programmers. The book 'Practice Your Basic' featured details on how to write a simple text adventure game called 'Treasure Hunt'. 'Treasure' is based on 'Treasure Hunt'.

# Installation
Copy TREASURE into a dataset that is allocated to SYSEXEC. To find which datasets are allocated to SYSEXEC enter 'TSO ISRDDN' from the command line.  Input 'FIND SYSEXEC' which will list the datasets.                         

TREASURE requires three panels; GAME2, GAME4 and GAME5.  These need not be copied to a dataset allocated to ISPPLIB, because TREASURE does a LIBDEF is done to allocate the panel dataset:
  "LIBDEF ISPPLIB DATASET ID('Z01408.ISPF.PANELS')"
  
 Copy the panels to a dataset and change the LIBDEF to reference that dataset.
 
 
