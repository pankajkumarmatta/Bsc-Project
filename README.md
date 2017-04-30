### Bsc-Project

### Introduction 

The purpose of makes this report to increase and demonstrate understanding of the use the different part of this project like virtual Box Software, Development of webserver, Apache webserver and hosting a website on your server. This is also  help us to familiarity with developer with cloud tools. It is also help us to increase the knowledge of Ubuntu server OS, connection with virtual box machine and Ubuntu sever.  After completing the process how to make a page on Github, as usally we know Github is a distributed version control system written by the creator of Linux, Linus Torvalds, this is a server which control system such as CVS. With the help of it we can commit and tag all our local machine without interacting with a server at all. Github also stores a copy of your project’s repository just like any other developer. This is help us to create own repository. 

Virtualisation(Virtual Box)    
 Virtual Box is a strong x86 and AMD64/Intel64 virtualization product for enterprise as well as home use. No doubt it has many rich feature but it is also very high performance product as well. This is just one and only available open source Software which comes under the terms of GNU General Public Licence. It has one specific speciality it runs with windows Linux, Macintosh and solaris hosts, and it supprt a large number of guest  operating system  but not limited to Windows (NT 4.0, 2000, XP, Server 2003, Vista, Windows 7, Windows 8, Windows 10), DOS/Windows 3.x, Linux (2.4, 2.6, 3.x and 4.x), Solaris and OpenSolaris, OS/2, and OpenBSD.
Virtual Box is being actively developed with frequent releases and has an ever growing list of features, supported guest operating system and platforms to runs on . 

Configuration and Deployment of the Virtual Machine:- 

First of all download the Ubuntu software, we can download it online which is very easy to download but in class we install through Pen Drive which was Provide by Conor it takes a 5 to 10 Minutes to whole process. Most notable thing we use Ubuntu Server OS 16.04 as this is an up to date and long term support version of Ubuntu. Wecan download it online direct from the Browser http://releases.ubuntu.com/16.04/. Scroll down and download the 32-bit pc(i386) server install imagelink. But we will use this file later when we install our virtual machine setup. 
Secondely install Virtual Machine to host Ubuntu server. We can install Virtual Machine our guest OS. VM Virtual Box mainly use for hosting our 32 Bit Ubuntu Linux server.  It has some steps. First of all we need to select the size and type of drive which we are going to use as well as memory which we are going to use for Machine. 

## It has some recommend settings: 
Memory Size : 2048mb 
Virtual Hard Disk: VDI, dynamically allocated 20GB 

### We need to mount the.iso image (Ubuntu Install File) which we downloaded/ copied earlier and proceed. We can access the virtual Cd drive by accessing the setting for the Virtual Machine and looking the storage settings.  After we have mounted the iso power on our virtual machine and the ubuntu install file will boot up. Select english has the language and continue to install ubuntu server. Continue through the setup selecting and appropriate settings. Not detect the keyboard leyout but to select it from the list instead. After setup has configured we can enter the host name for our computer . I suggest calling it web-server but any single world will do.  After that follow the screen instructions. Write them settings we enter  here we will need them later. Make sure whatever password we used remember that, and it should be a t least 7 charcters long and mix of numbers, symbols, upper and lower cases letters.  Choose a guided partition and volume of the entire disk . Confirm changes to the disk  this may take ten to fifteen minutes to whole process. Do not setup a proxy and choose automatic security updates and then we can install a base package as we will manually install the software we need in the next tutorials. Install the GRUB  boot loader and finish the installation. The machine will reboot when finished prompting for the login details we entered earlier, then we have successfully deployed the ubuntu server
While the install is running go to the Github.com and create a free account. Well you make the account on Github.com and complete the HELLO WORLD to act your introduction to Github. 	

### Create a Virtual Machine:  
### In the Virtual Box Manager window, Click on the “New” button( a blue spiky circle) 
After that process the first screen asks for Name and Operating system then Enter and we can give it any name like our own name or Ubuntu-1 etc. In second option it asked about Type which has to chose Linux, Version 32Bit( Uubuntu) and then click next and select the size of memory which is by default 512Mb, we can change it later. After that it will ask for Hard Drive Select “ Create a Virtual hard drive” and click “Create”.  Select the default VDI(Virtual Box Disk Image) and click next. After those steps choose “Dynamically allocated” and click next.(This option allocates disk space only when the guest OS writes to the Virtual disk). Increase the size of it 10GB but it does not mean it will actually use 10GB straight away on your Laptop or Computer,but will allow it to grow up to 10GB and then click create. After finished all those steps we will see VM created but the “Power Off”. 
Inserting a Virtual CD 
When we start a VM first time, Virtual Box automatically prompt us for a CD-ROM image. However we are going to it in manual way so that you learn your way around the settings. 
Before starting the Vm click on the “Settings” button (an Orange sprocket) after that click on Storage and chose Controller:IDE 
                                                                  ......... Empty (with Cd Icon)  
                                                                             Controller SATA 
                                                 ...........Ubuntu -1.vdi( Or whatever you chose Name)
                                                                       
Click on the Cd icon by “Empty”. To the right we will see: 
Attribute: CD/DVD Drive: IDE Secondery Masterand another Cd icon Click on this other CD icon From the menu which appears, select choose a Virtual CD/DVD Disk File. Browse to the Directory where you copied the Ubuntu server ISO Image and select it 
And then we will see Controller:IDE, Ubuntu-12.04-3 server-i386, Controller SATA....Ubuntu-1.vdi. 
Click Ok Start the VM 
Select the Vm and click the green start arrowand the Vm will start. After this whole procees some warning will show on Computer Screen like “ You have auto capture Keyboard option turned on you can press the host key at any time to uncapture the keyboard and Mouse and then return them to normal way The host key is currently defined as Right Ctrl” 
After that Have a look at the bottom right hand corner of the window. It should show a reminder of what the host key is currently is set to, next to a small download arrow. The Ubuntu installer should start. Click inside the window. Note that you may have to press the host key to get your mouse out again. After thatselect your Language like Select Englis(UK) and  press F3 if youwant to select a non US Keyboard layout. Next press F4 and install minimal virtual machine. This selects the minimum number of the package to get a very basic sytem Use whatevr Hostname, Username and Password you like. This is our own Virtual Machine. 

Strongly Recomended settings: 
Encrypt your home directory? No 
Partitioning method: Guided-Use entire Disk. It’s mean it will use entire disk sda, which is about 8.6GB and is an “ATA Virtual Box Hard Disk” . Allow it to write changes to the disk.Remember , this is safe- we are not  overwriting on our real hard drive it is going to writing into the virtual disk file which we created before. 
Select none for HTTP proxy 
Select automatic updates 
When you get to “Choose  software to install” move to Open SSH Server and hit space to select it, but leave everything else unselected. Install GRUB boot loader to the master boot record? Yes 
Restart  Once the installation is complete, you will be prompted to restart. If the Machine starts up with the virtual CD-ROM will attached, we may need to remove it. Go to settings> storage as before, click to the Cd icon under Controller IDE click on the second Icon CD select remove disk fro virtual drive then restart the VM again. After few seconds we get login Ubuntu prompt and then Login with the username and password which we created before.   
                                                                                                    
Explanation of web server : Web server is kind of computers that deliver web pages. Like we know every web server has IP Address and their domain name . For Instance: If we enter the URL http://www. Wikipedia.com/index.html in our Browser this sends to a request to web server who domain name is wikipedia.com. We can any computer move into web server with help of installing  software and connecting the machine to the internet. There are many web server and software applications including public domains and commercial packages.  While Apache Web Server software commonly reffered  to as just “Apache”, It is technically called “ Apache HTTP Server” , since the software serves  webpages over the HTTP protocol. When apache is running it’s process name is short for ” HTTP Daemon”. Apache is a one of the most popular software web server. It enables to computer to host one or more websites that can be accessed over the internet using a web browser The one of the most interesting thing in Apache it is open source and free to use, therefore web hosting companies  offer  Apache based web hosting  solutions at minimul costs Other server such as window server requires a commertial licence . Apache also supports multiple platforms including Linux,  windows and Macintosh operating systems. Apache can  host static websites as well as dynamic websites that use server side scriping  languages such as Php Python or Perl. Apache is also support to others modules which offers advance security options like file file management tools and another features. Install Apache Web Server: 
WE are going to install the Apache Web server. Log into your VM( if updates available you can install them with sudo apt-get upgrade command). 
Enter the command below to install apache2 apache2-utils 
We want to change our setting so the Apache2 web server will start up at system boot to do this enter the systemctl enable command. Type the following: 
Sudo systemctl start apache2 lets check our Apache sever is up and runing. First we will need to make sure that our network adapter setting make ourVM visible from our host. Wewill need to shut down our VM and change the setting our virtual network adapter. By default our adapter is configured as Network Address translation. We can set up port forwarding with our host to make it accessible from the host. These setting can be accessed through the settings-Network-Advanced-port Forwarding 


Port Forwarding Rule
Name     Prrotocol      Host IP       Host Port       Guest IP      Guest Port
Apache     TCP                                      80                                            80 


2. Install My SQL
Sudo apt-get install mysql-client mysql-server 

Sudo mysql_secure_installation ( Strong password is required ).

Install PHP and Modules 

Sudo apt-get install php7.0 php 7.0-mysql libapache2-mod-php7.0 php7.0-cli php7.0-cgi php7.0-gd
When the command is finished running we need to test that PHP working. We will do this creating a info.php file in our /var/www/html directory

Type the command 
Sudo vi /var/www/html/info.php

This will open a new file called info.php. Press the i key to enter insert mode and then type the following php code in: 
<?php
phpinfo(); 
?> 
Press ESC when you are done entering text then enter the command :wq to save your file and close with Vi
Open your web browser in your host computer and go to the addresss localhost/info.php then you will see a page containing configuration information.

Reflection: Well everything was ok i had not any hurdle because i had the full data of install all the process but there was two problem happen with me Firstly this is very sensitive work therefore everything should be a perfect the problem i faced sometimes i put wrong comand  which creates a error because if there is one step is wrong while installing it stops the whole procees. Secondly i had problem with password the password should be strong and always notice it otherwise if we forget the password or username then we have need to whole procees again 

Conclusion: Over the years I’ve used many version control systems, and many backup schemes. They all have facilities for retrieving the past contents of a file. Most of them have ways to show how a file has differed over time. Many permit you to go back in time, begin a divergent line of reasoning, and then later bring these new thoughts back to the present. Still fewer offer fine-grained control over that process, allowing you to collect your thoughts however you feel best to present your ideas to the public. Git lets you do all these things, and with relative ease — once you understand its fundamentals. It’s not the only system with this kind of power, nor does it always employ the best interface to its concepts. What it does have, however, is a solid base to work from. In the future, I imagine many new methods will be devised to take advantage of the flexibilities Git allows. Most other systems have led me to believe they’ve reached their conceptual plateau — that all else from now will be only a slow refinement of what I’ve seen before. Git gives me the opposite impression, however. I feel we’ve only begun to see the potential its deceptively simple design promises.




