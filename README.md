# passscript

My very first script, no Hello Worlds.

Last weekend my teacher installed a VNC server client (Epoptes) in my classroom computers. Feeling challenged, I wanted to try how 'strong' was the system, and after some minutes I managed to get rid of my teacher's control just by killing the process.

I went home, and I decided to improve the server security just by configurating a few options via a simple bash script, my very first script. As it was ridiculously easy to type the following command in order to kill the client:

    $ kill $(pidof epoptes-client)
    
My intention was to restrict access to commands kill, pkill and pidof so that they could only be used via sudo, and to configure the 'sudoers' file to ask for the root password I would have set previously. As a result, the user wouldn't be able to execute any sudo command without the root password (which would be supposed to be secret), being uncapable to kill their 'Big Brother'.
