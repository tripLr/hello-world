# project learn to install and use Linux  

newest posts at top 

<meta name="keywords" content="linux,mint,ubuntu,how-to,how to,install,server,destktop,fedora,redhat"> 

update 3-28-18
    Ok, here is what you need to know about high end servers.
    Stability and dependancies. to achive this, Linux achieves this in several ways.
    1. Debian only uses open source for all its programs and kernel install. DO not install downloads, or your going to
         get dependancies that are inconsistant. cleaning a linux system is hard. installing PPA is really difficult.
    2. Ubuntu allows "PPA" installs , but that is another way to get your binaries out of sync
    3. Red-hat and its sibling, Fedora are a little/lot more hardened for having needed stabile software
   4. Dell makes open source all its drivers. really really nice . 
   
3-18-18
   its been a while. i have been cramming nights on building linux for my older laptop in prelude to building a server. 
   i have one thing to say about any ubuntu distro.  find a desktop that you like, the core is all the same.
   i am running linux Mint, based on ubuntu. it has a excellent software center and the desktop you see is what you like, not really the programs annd core. those all come from canonical servers ( ubuntu )
   
   linux mint is based on the "Mate" desktop . most all desktops are based on the opendesktop.org environment. this is a standard to do the same things
   
   this is called the "display manager" or the desktop environment. 
   
   so LXDE is the desktop environment that lxle.net is based off, with ubuntu core programs, however, if one is downloading programs, and the program comes with a PPE distrobution rather than the official Ubuntu sources, one can quickly install binaries that are NOT compatable with released stable binaries. i found out the hard way. ( format-reload )
   
   so ubuntu comes with an lxde flavor (distro)
   a mate ( linux mint desktop) flavor but is NOT linux mint.
   a KDE distro.. etc, you get the drift..
   
   each sub distro of Ubuntu has some basic support BUT it makes it easy to get lost in the usage of what the core system does
   
   Ubuntu trys to make a official distrobution, that you can have paid for support for servers and such
   so does redHat linux, which as a linux distrobution has quote " official distrobutions for paid for support"
   
   redhat has a free side called Fedora, which has a desktop and server flavor.
   
   so which to choose? what do you want to do with linux ?
   if you truly understand linux, it won't matter.
   its about resources and scaleability.
   
   linux is open source at its heart.
   what that means is anyone can read it, use it and modify it, but they cant charge for it.
   at the core of linux is the kernel,
   www.kernel.org
   
   all the changes edits, and release come from a guy called Linus Torvaldas, he deserves the Nobel Peace Prize.
   he has a team of people, that mostly work for free or are supported by the linux foundation to write the kernel and the
   drivers for hardware.
   
   linux, stands for linus torvaldis Unix operating system
   google unix history and you will find out that really big corps sold UNIX as a stable version of an operating system for 
   Corporations and the guvmint. 
   Universities used a custom UNIX called BSD, written by students, ( berkley science division ), but
   is still a licence to use it.  
   its free, but not "free", truly open source.
   google open source, and freeware
   
   so an open source version was created.. open BSD, which battled FreeBSD . 
   Enter Linus Torvaldus about the time Microsoft bought Windows to battle Apple, both running propritary desktop operating 
   systems to compete in the desktop computer market.
   
   IBM and Solaris and a couple other companies were selling the Backbone of the internet at the time, Servers that cost 
   hundreds of thousands, and Cisco sold switches and routers that expanded the internet.
   
   enter Linus, who coded in the C programming language the ability of an IBM 386 $6000 POS desktop system to run a WEB server!
   boom, he kept at it, kept writing a kernel that most unix software could run on, or be patched to run on, and now everything
   runs core Linux, including, Apple, Google, Microsoft and all your cell phones, your internet of things, your game camera, 
   you name it linux is a part of it
   
   Linux can run on a 386, or 64 CPU with multi core server or a supercluster supercomputer, and your smart wristwatch. 
   all Linux, Oh, dont forget Bitcoin.
   
   So, get out that older laptop, and wipe out the windows 98 or older, and load Linux Mint, or lxle.net on it.
   update the drivers
   compile the kernel ( www.kernel.org )
   to the newest version that will load your drivers
   
   grab that old tower PC and make a home web and video server
   
   Buy a used Dell Proliant or HP server on ebay and load up Ubuntu, Fedora, or if you really want a challenge, Debian or Arch
   
   be prepared to stare at an old style CRT monitor and run text only commmands to make it Scream !, desktops are great,
   Terminal commands are where its at. 
   
   Oh, which Linux Desktop I hate ? Ubuntu ! the Gnome destop sucks. I am a windows dude, so LXDE or Mate rocks
   
   full disclosure, i built a router/mailserver for a internet company in 2001 or so,
   and because i didnt read the security updates for the
   remote management, it was hacked in about a month turning it into a DOS attack machine. 
   
   The guy who ran a dial up service i used , went to give me about 30 1.44 mb floppies with Linux on it. i said no. my bad
   
   thanks
   written on a HP dv9810us dual Athalon dual CPU 4GB laptop with Nvidia Chipset and video, 
   runnining Linux Mint
   on kernel versions
   4.13.0-36-generic ( stock upgrade )
   4.14.27-HP-tripLr ( custom latest stable long term release)
   4.15.8-HP-tripLr  
   4.16.0-rc5-HP-tripLr ( linux custom release canidate )
   and building
   4.15.11-HP-tripLr
   4.16.0-rc6-HP-tripLr
   
   tripLr.dev@gmail.com
   m.rrrogers@gmail.com
   
1-8.to.1-13-18 
        So i have a second drive on my HP laptop installed with www.lxle.net a linux distribition based on www.ubuntu.com
        
  If your running windows, you will have to have a usb iso installer . multibootusb can install multiple iso's on a single
        usb drive, use the same program to install a single iso onto a single usb drive
        
   www.lxle.net  I learned a lot with this install because its user friendly
        If you have an older computer with old drivers or first time linux users to install this distribution
        i have installed the partitions as / 'root' 25 gb, /var 25 gb, swap 25 gb, /tmp 25 gb, /home remainder of drive 500+ gb
            this is because the drives will be really busy while compiling, and this is the server scheme. normal swap files are 
            usually 1.5 times usable memory. use more for stability. /var and /tmp are where the system unpacks files and
            uses temp cache for web and other processes. everything the all users installs should be in /home
            so lets say you upgrade or build your own kernel. the grub bootloader is installed in the boot partition of the 
            drive(0) , Grub allows you to boot from multiple OS and multiple Kernels . cool
   
   Warning, this and other distros make you the super user,so you can put in your password to root. if your connected
        to the internet this is a bad idea. 
           fix.. when your up and running, open a terminal window and type
           >sudo passwd<  put in your user password to get sup privlage, then put in the system password.
           dont know why they do this but its stupid
   Driver install and upgrades. Super Easy. click the driver manager, and install your non free ( manufacturer ) drivers. 
           pay attention to the driver names, export the driver names to a thumbdrive
        
   www.debian.org  I have also finally figured out how to install Debian. ( read, read, do and try )
        
   Debian is the ULTIMATE top level distro of linux. any kernel changes are made here by linus torvaldis himself
        see www.kernel.org
        
   My hdd(0) has 2 partitions, windows 10 ( finally got enough updates to work. rinning 64 bit version with windows 7 64 bit
        drivers from HP. from 2008.  buwahaa. that took a while to get stable.
        So with the second partition, i just installed debian in the whole partition and used hdd(1) swap sector
        www.debian.org  follow the download and install instructions.
        warning , read up on command lines in terminal , u will have to use them.
        i reccomend downloading a linux textbook to your Kindle 
        and the step by step guides 
        https://www.debian.org/releases/stable/installmanual
        https://www.debian.org/doc/
        My Install
        I finally did an install without the graphical interface provided
        its similar to other distributions 
        
   When you get to the selection of which desktop to use ONLY SELECT ONE. I am a software collector so I like it all. not 
   good idea in linux ( i tried installing this about 10 times before i got it right.
   You will be asked for system password ( su - superuser ) and a login. this is for u not to screw up to easy.
   
   I select LXE desktop because it uses a whole lot less resources on my older laptop. See above. its the same desktops , 
   icons and similar programs
   to the lxle.net distro. lxle has a very stable and editable menus and icons
   
   Boot to screen. look at your driver names on your thumb drive and install them using the synaptic package manager. 
   This program is common on all distributions of Linux. its ALL the software that can run on your device. 
   note, u have to configure the repositaries. they tell the manager where to look for your software.
   You need to disable the CDrom repo or every time u use this it will ask you for your thumb drive or cd. click the toolbar 
   see the repos and scroll to the one that has the cd listed, and deselect it.
   
   debian only points to debian servers
   lxle points to ubuntu servers and others, because its a port of ubuntu
   synaptic package manager is a window version of git
   
   you are going to learn git, and github where you are if you build anything. its how EVERYTHING gets programmed and
   tested that is open source ( free ) INCLUDING Android.
   
   Thats IT folks. I finally have a working stable install with all drivers of www.debian.org and www.lxle.net and poor old 
        microsoft windows 10.
   
   So now i am learning to build, modify , test and install progams, kernels, android distrbutions and whatever i want !
   
   www.kernel.org walks you thru on how to build, install, and test a linux kernel. if you mess up you can boot to the old one
   easy. see older posts.
   www.xda-developers.com is a huge resource to learn to develop custom android. it primary drive is to root older devices
   and install newer versions of android on them, do to manufacturers stop supporting devices
   i have a galaxy note 4 verizon ( sm-t910v ), and its running android 7, and samsung stopped at 6 search @tripLr in the forums, 
   and you will see my posts ( 
   i also was gifted an expensive (300 buck) samsung galaxy sm-t710, and have had it rooted and runnning Posiedon rom, and now 
      LineageOS. search those names to find those devices
      
THANK YOU ALL. on to my next project
   
   
1-7-18  updated partitions . again. Reinstall again. For /var only had 25 mb instead of GB
.
1-6-18  todo list
               resize partitions, especially for swap area. swap area crucial for builds
               update crypto so i can sign my distros, and download them cant update laptop drivers with out correct keys
               update drivers
               install drivers and software 
               install android build software

1-6-18 spent a lot of time in the config files for security becuse updates were not completing due to security signing. 
         root root..crashed some extensive note because i forgot to save. oh weell
         command line relearing linux
            just to update drivers
            then the security in debiian is so strong, i have to say good, but makes it hard to install programs and drivers 
            not in their release files. but i have to learn because it will make it next to impossible to install development 
            software
            
1-5-18 i compiled a kernel, and it updated to debian desktop with all my old ldlx files. interesting
        so i reloaded full debian. debian is the developers dream. getting used to it is not for noobs, 
        but a good excersize in installing for a server and such
            
12-2-18 i learned if you use command line git, u better be in the folder u want to download everything 
        using this guide, https://kernelnewbies.org/KernelBuild which is similar to the process of building a kernel 
            in FreeBSD. working on my config file...to build
        why build your kernel ? beause of the unneeded code in your distrobution especially for your drivers its for stability.
        
12-2-18 created directory on ldlx linux laptop for repos, finished laptop install working on continuing education in linux builds



12-1- 18 My first github
my first edit and commit

Welcome to my first github 
I will be using this forum to make and build ROMs for my tablet and phone using sources posted in XDA forums
my new hobby and hands on learning for skills

made a change going to merge fork and delete fork
