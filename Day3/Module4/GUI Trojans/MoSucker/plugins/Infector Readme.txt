
 +------------------------------------+
 +-----------[ SuperClicks ]----------+
 +------------------------------------+

 Plugin written by Superchachi
 Homepage: www.mosucker.tk

 ******* Category: Fun *********

 Plugin file:          infector.msp
 Plugin size:          19.5 KB

 ------------------ Description of the features: ----------------------

Some trojans or viruses may include a wormlike feature that will drop a server into a common fileshaing folder. MoSucker's INFECTOR plugin takes filesharing infections to the next level. By packaging the infector plugin with your MoSucker 3.0 servers, your servers will bind itself to every .exe file in any folder that you specify. Infecting multiple folders is supported.
There are a few steps you need to take when editing your server to take advantage of this feature.

Goto the Plugins page of the edit server and add the infector.msp file to your server.

Goto the options page and check "Drop full server into %windir%". Specify a filename.

Goto the Events page and start a new "on startup" -> "Execute Plugin" Event.



Your "Execute Plugin" event requires a little bit of scripting. This gives you the power to specify order, folders, and other options. Scripting for this plugin follows this format:

infector @@@{01}folderpath1{02}filename.exe{03}

filename.exe is the name you specified in step 2.

folderpath1 is the path to the folder that contains the .exe's you want your MoSucker server to bind itself to. You may specify multiple folders, separating each with a "#".

Example event:

infector @@@{01}C:\Program Files\Morpheus\My Shared Folder\#C:\Program Files\Kazaa\My Shared Folder\#C:\Program Files\Bearshare\Shared\#C:\Program Files\Edonkey2000\Incoming\#C:\Program Files\KaZaA Lite\My Shared Folder\{02}server.exe{03}

The INFECTOR plugin is able to detect which files have already been infected to avoid re-infection. Using the example script above, your plugin will search each specified folders every time the server starts and infects any new files that have been added. By added the word "kill" at the end of your script, the plugin will only infect all files on the first startup rather than each start-up. It is recommended that you use this kill command. 

Example event with kill command:

Same as above ...... d Folder\{02}server.exe{03}kill

The Windows and System/32 folders have been blocked. Infecting these folders will cause endless errors. However ... paths to popular anti-virus software have not been blocked from infection. Use your imagination. MoSucker 3.0 has multi-infection protection, so multiple servers running is not an issue.



 How to use:
 Copy the files "Infector.gui" and "infector.msp" to your
 MoSucker\plugins directory.
 Start the client, select "Plugins" in the "Misc stuff"-menu
 and doubleclick the "Infector".