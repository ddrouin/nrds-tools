nrds-tools
==========

A library and a user-interface (called 'KosLookup') that will provide the ability to
check if a pilot in EVE is 'kill on sight' in Providence or not.

Simply type 'xxx' and drag and drop a pilot's name into a chat window that this tool
is monitoring, and the pilot will be looked up on http://kos.cva-eve.org/ to see if
they're Kill on Site or not.

Release version:
https://github.com/downloads/eve-val/nrds-tools/KosLookup-0.6.zip

Jerub's Beta version:
http://www.nrds.eu/downloads/KosLookup.exe

Dave Drouin's fork of Jerub's Beta version that supports running on Linux with 
sounds.  Additional requirements for playing sounds on Linux (installing audiolab):

sudo apt-get install libsndfile-dev python-numpy cython
git clone https://github.com/cournape/audiolab.git
cd audiolab
python setup.py install --user

Then run KosLookupExe.py providing the location for the chat logs and a sound to 
play when a KOS player is present.

python KosLookupExe.py -c ~/EVE/logs/Chatlogs/ -s /usr/share/sounds/gnome/default/alerts/bark.ogg

