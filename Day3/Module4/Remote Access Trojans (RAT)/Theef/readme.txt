Downloaded from Hacking Library
http://www.library.2ya.com

-


##############################
#  Theef v.2.10 01/Nov/2004  #
#   http://theef.4-all.org   #
#  tt - theef3000@yahoo.com  #
##############################

Changes;
~~~~~~~~

[2.10]
 + New; Recent folder menu in file manager
 + New; Favourites menu in registry editor
 + New; Automatically remove finished transfers
 + New; Improved password security, using MD5 hashes
 + New; Improved, full remote command shell
 + Fix; Manually removing finished transfers mid-way through other transfers
 + Fix; Manually entering folder path that's already been viewed
 + Fix; Decimal separator difference bug between client/server
 + Fix; Access errors on 'download dir' when local dir already exists
 + Fix; Connection statistics transfer sent/received count
 + Fix; Small bug in network drive options popup
 + Fix; Retrieves full path of processes on NT systems
 + Drag & drop between file manager and transfer window
 + DiskInfo on a network drive shows network path
 + Seperated filename/path in process viewer
 + Improved network browser at both client and server side
 + Changed transfer window's file list
 + Redesigned connection statistics window
 + Redesigned file search result list
 + Improved ListDrive info, no strange characters on removable drives
 + Improved IE Favourite listing

[2.02]
 + Fix; Tiny file <1kb transfer bug
 + Fix; Drive info icon
 + Improved country/language info
 + Improved command data transfer

[2.01]
 + New; Keylog parser 
 + New; Detailed drive info 
 + Editserver; meltserver and new keylogger settings 
 + Improved file transfer window view (time taken/remaining, etc) 
 + Fix; multiple (+10) local filename download bug 
 + Fix; upload transfer speed recording 
 + Fix; event manager OnInstall event should work better 
 + Improved event manager classes 
 + Client layout tweaks

Readme;
~~~~~~~

 + Compatibility; server should work on all Windows OS's

 + File caching; improves speed of file browser by only re-requesting the contents
   of a directory if it has actually changed, saving time and bandwidth

 + Hugely improved file management system, as well as file caching, there's local 
   icon caching, network browsing, integration with search/edit/transfer, fast
   access straight to common folders (desktop / documents)

 + Event manager; schedule events to happen at certain times, allowing you to
   automate server actions without needing to be connected to it

 + Plugin manager; extend the functionality of the server by creating/installing 
   plugins, which can also be used alongside the event manager

 + Keylogger; write all keys that are typed into specific window to a seperate file
   for easy password lookup

 + ... and too much more to write about!

Plugins;
~~~~~~~~

There are a few plugins included; Password retreiver, IP Scanner and Zip add-ons.

There's a tutorial on the Theef homepage showing you how to install and use plugins,
and the Zip plugin is open-source.

Notes;
~~~~~~

Included in this package is UPX, use this to compress your servers after you have 
edited them; it will reduce the size of the server down to around 268kb. Use from 
the command prompt like so: 

    UPX --best Server210.exe

And to decompress: 

    UPX -d Server210.exe

You can configure the editserver to automatically compress your servers, with the packer
of your choice, when you are finished editing them.

Contact;
~~~~~~~~

    http://theef.4-all.org
 
    theef3000@yahoo.com

Please visit the forums (link on homepage) for any questions, comments, bug reports
you want to post.

Cheers!

That's it, thanks for downloading :)

tt