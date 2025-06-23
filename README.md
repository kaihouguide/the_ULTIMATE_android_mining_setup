This guide was written by @1selxo , you can reach me on discord if you have better tools or improvements<br>  
this is not a new or made by me tools but i have not seen a comprehensive android-only guide for japnese language immersion before so i thought i'd share my setup with some hacks and tricks i use <br> 
## Installing all of this guide will need quite a bit of space, i reccomened you have a 128/256GB phone at least before attempting to install all of this <br> 
# ANKI WITH ADDONS ON ANDROID 
THIS DOESN'T TAKE PLAC OF ANKIDROID AND IT'S REALLY UNCOMFORTABLE TO ACTUALLY DO REVIEWS ON, I RECCOMENED THIS ONLY FOR PLUGINS THEN SYNC AND USE ON ANKIDROID
first of all you will need some requiruments to use this 
first you will need to get [termux](https://github.com/termux/termux-app)
[RealVNC](https://play.google.com/store/apps/details?id=com.realvnc.viewer.android&hl=en)
in termux run in order
 <pre> pkg upgrade  </pre> 
 <pre> proot-distro install debian  </pre> 
 <pre> proot-distro login debian  </pre> 
 <pre> apt update && apt upgrade </pre> 
  <pre> apt install sudo </pre> 
   <pre> adduser (your username) </pre> 
   <pre> nano /etc/sudoers </pre> 
   scroll down till you find root and in the line right under it add your user like this 
User ALL=(ALL:ALL) ALL
![Screenshot](./Screenshot%202025-06-23%20121624.png)

now technically the linux installation is done but we need to access it so 
