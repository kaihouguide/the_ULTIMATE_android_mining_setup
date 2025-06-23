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
   <pre> sudo apt install xfce4 tigervnc-standalone-server dbus-x11</pre>
   <pre> adduser (your username) </pre> 
   <pre> nano /etc/sudoers </pre> 
   scroll down till you find root and in the line right under it add your user like this 
User ALL=(ALL:ALL) ALL
![Screenshot](./Screenshot%202025-06-23%20121624.png)
   <pre> su (youruser) </pre>
   <pre>vncserver -xstartup /usr/bin/startxfce4 -localhost no <pre>
now technically the linux installation is done but we need to access it so we'll do so through a VNC
    you can access this from a password or on android using RealVNC eitherway, now you should be booted into a linux enviroment
in the terminal of LINUX in the VNC copy and paste the following in order to run anki
    <pre>    sudo apt install python3-pyqt6.qt{quick,webengine,multimedia} python3-venv   <pre> 
    <pre>   python3 -m venv --system-site-packages pyenv <pre> 
  <pre>  pyenv/bin/pip install --upgrade pip  <pre> 
   <pre> pyenv/bin/pip install --upgrade --pre aqt <pre> 
 <pre>    pyenv/bin/anki <pre> 
 <pre>  apt-mark hold libpci3 <pre> 
 <pre>  echo software > ~/.local/share/Anki2/gldriver6 <pre> 
  and finally to run anki ! 
<pre>QTWEBENGINE_CHROMIUM_FLAGS="--disable-seccomp-filter-sandbox" pyenv/bin/anki<pre>
every time to run anki just rerun 
<pre>QTWEBENGINE_CHROMIUM_FLAGS="--disable-seccomp-filter-sandbox" pyenv/bin/anki<pre>
i reccomened you just make this an excutable to just be able to double click it
