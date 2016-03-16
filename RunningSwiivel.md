# Introduction #

This page should contain a step-by-step guide for installing and running swiivel.

# Details #

Requirements:
  * python-pygame
  * python-bluez
  * N wiimotes.  Currently N should be less than 5.  If N=0, you can only play one player (with keyboard and mouse).
  * ceil(N/4) bluetooth dongles.
  * If N>0, you need a Sensor Bar.  This can be any two sources of infrared light (tea candles work well), positioned a foot or so apart in front of your screen.
  * subversion

Steps:
  * svn checkout http://swiivel.googlecode.com/svn/trunk/ swiivel-read-only
  * cd swiivel-read-only
  * ./swiivel.py
  * To connect a wiimote, type its bluetooth address and hit enter; on the wiimote, hold the 1 and 2 buttons to put it into discoverable mode.  If you'd rather not type the address each time, you can enter it in KNOWN\_WIIMOTES under wmd/Config.py.
  * Console controls: mouse to aim, cursor keys to move, space to fire
  * Wiimote controls: point to aim, D-pad to move, A to fire
  * Escape quits the game