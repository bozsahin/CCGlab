# <code>CCGlab</code> in Windows10 as a native linux app.

This guide is prepared by Efecan Yilmaz. It gives you first a linux as W10 app, then ccglab. 
=======
This guide was first prepared by Efecan Yilmaz. It gives you first a linux as W10 app, then <code>ccglab.</code> 

No partitions, no virtualbox. Thanks Efe.

-----------------------------

- You need to be on version 1909 of Windows10, build 18363.476 or later. 

- To find out your Windows 10 build, use Windows Search at bottom-left for 'Settings' and look at 'About' in settings somewhere at the bottom.

- Similarly, to locate <code>Powershell</code>, use Windows Search at bottom-left and search for 'Powershell'.


This document is based on: <a href="https://docs.microsoft.com/en-us/windows/wsl/install-win10">WSL</a> (windows subsystem for linux)

You can try the newer and easier version of steps 1-2 at <a href="https://towardsdatascience.com/dual-boot-is-dead-windows-and-linux-are-now-one-27555902a128">WSL2</a>.

1. Open a Powershell window *with administrator rights* and execute the following command:

	<code>Enable-WindowsOptionalFeature -Online -FeatureName Microsoft-Windows-Subsystem-Linux</code>

	(This will ask at the end your computer to be restarted; say YES)

2. Go to Windows Store (search for "store" in Windows Search), and search for "Linux" in the store.
	- Download your preferred distribution (our guide is for Ubuntu, which requires the least amount of effort in configuration.)
	- When the download and installation finishes, click on "Launch" in the Store window for the first time installation to take place.
	- Please note your username and password at the end of the installation. 


3. Assuming you are in the terminal app that Ubuntu opened for you when asking for userid, do: 

<code>cd ~</code>

(This is your home in linux app of w10, wherever windows created it.)

4. do: 

<code>git clone https://github.com/bozsahin/ccglab </code>

5. Proceed with  <a href="https://github.com/bozsahin/ccglab/blob/master/README.md">ccglab installation guide</a>.

You are ready to go. You can close the linux app when you are done without loss of work. 

To run again, locate ubuntu app from windows left corner button and run; once in ubuntu, just call <code>ccglab</code>. 

