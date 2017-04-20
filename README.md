# SilentUninstall
Silently Uninstall Software manually or by GPO using this batch file as a script in Windows.

**In order to uninstall software, you must edit the batch file after download. I will attach a few batch file examples to aid, but please do not run them unless you want the program uninstalled. Just right click on the file and click edit. 
Additionally, please see screenshots that I have attached to help.

*I cannot guarantee that this will work for every program, and you will have to have some level of command prompt skill and know your way around program files on Windows to edit the batch files.


   # x64 version
      "C:\Program Files\Program\Program\program.exe" /Appmode=Setup /uninstall /uilevel=Silent /dontrestart
      Where "\Program\Program\Program.exe" are, place the corresponding program files in place. For instance, for Adobe Photoshop, I would
      put the following...see below
      "C:\Program Files\Adobe\Adobe Photoshop CC 2017\Photoshop.exe" /Appmode=Setup /uninstall /uilevel=Silent /dontrestart
      You will need to find the files accordingly, as each program will have different file structures.
      
   # x86 version
      "C:\Program Files (x86)\Program\Program\progm.exe" /Appmode=Setup /uninstall /uilevel=Silent /dontrestart
      The only differnce is adding (x86), which is used when you are running 64bit architecture. Same thing applies as x64 version.
      See below for example in use with Evernote...
      "C:\Program Files (x86)\Evernote\Evernote\Evernote.exe" /Appmode=Setup /uninstall /uilevel=Silent /dontrestart
      
