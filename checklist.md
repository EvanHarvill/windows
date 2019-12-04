<pre>
2019 Cyber installation checklist - start with a VM (Wamware)

#WINDDOWS VM CHECKLIST (VIRTUAL BOX or VMWARE)
TRY TO USE 64 BIT APPLICATIONS
_____ Set VM to bridge.
_____ Set Static ip : Control Panel\Network and Internet\Network Connections
        AM 10.183.3.# / 16  PM 10.183.4.# / 16
_____ Create a "windows" repo in your github account.
_____ Add the following directories: screenshots and docs. 
        Etxra direcotories{system, security}
_____ Install Python 64 bit.  Test with yourt turtle graphics.
_____ Process explorer - upload text output to docs
_____ Install and run tcpview - upload text output to the windows repository
_____ Change the name of your computer (hostname)
_____ Install 2 pdf viewers (Adobe Acrobat Reader  and your choice)
_____ Install firefox and chrome
_____ Install and run Packettracer
_____ Install and use git ( https://git-scm.com/downloads)
        Make git usable with PowerShell ISE
_____ Install and use atom.io (optional)
_____ Install Audacity (optional)
_____ Install and use putty (64bit)
_____ Install and use cygwin
_____ Configure Cygwin for ssh gcc, g++ and ssh)
_____ Configure Cygwin to compile c code.
_____ Compile and C code using Powershell ISE
_____ Install JDK from Oracle (Java Platform JDK 13  Date:191119)
_____  Configure classpath for JDK. (Caution)
_____  Compile and run JAVA,
_____  Enable GOD MODE 
_____  Install gpg4win and send an encrypted textfile to  . . .
Look at the following using file explorer: %appdata%  and %localappdata%
_____ Upload a screenshots of the result of %appdata% to github
_____ Upload a screenshots of the result of %localappdata% to github
_____ compmgmt.msc (Screenshot compmgmt.msc showing users and a custom group.)
_____ mmc (Screenshot host mmc with 3 windows users with one user in a custom group.)
_____ Create folder on your desktop and share it.  Hvae someone add files to that folder.
_____  Install BGInfo.zip and appy the settings to your desktop.
_____ Enable OpenSSH and OpenSSH Server 
          Windows-Settings>Apps>
           Manage optional features
           +Add a feature
            (Add OpenSSH Client and OpenSSH Server)
############################################################################
Server client process:
_____ Install fileZilla and connect to an ftp server.
        Probably 10.183.1.30
        Download irfanview (iview.7z) and install it.
Server side processes:
_____ Install one copy of Nginx.  Install the package at c:\nginx
_____ Add a custom html to Nginx document root.
_____ Start a python webserver at ip:8000
_____ Place text and images in a directory "web/files"
        Notes for python webserver.  Create a directory in the same folder named "web"
        Run the following script:
        import http.server
        import socketserver
        import os

        PORT = 8000

        web_dir = os.path.join(os.path.dirname(__file__), 'web')
        os.chdir(web_dir)

        Handler = http.server.SimpleHTTPRequestHandler
        httpd = socketserver.TCPServer(("", PORT), Handler)
        print("serving at port", PORT)
        httpd.serve_forever()
</pre>