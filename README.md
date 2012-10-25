surfno is actually a suite of tools:

* surfno - blocks sites (via /etc/hosts)
* surfon - unblocks sites (restores /etc/hosts)
* surfstat [-v] - utility used to determin surfno state

The main reason I created surfstat is so I could use it to set my shell
prompt. For example, I place this in my ~/.bashrc:

    PS1='[\u@\h \W$(surfstat -v " (%s)")]\$ '

If in a surfno state, I get a red colored status that says "surfNO", if
in surfon, it is a green colored "surfON".

Super simple, but I banged this out because I needed something like this
and there was nothing out there that satisfied me.
