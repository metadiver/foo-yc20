# Foo YC20 VST #

By far the easiest way to use the Foo YC20 organ is to use the included VST instrument plugin. You can integrate the plugin into a host of your choosing and have the organ running in your sequencer etc.

However, due to the nature of the organ processing, it is worth noting that the VST plugin uses a lot of CPU power. This is regardless of whether it is playing sounds or not.


# Standalone JACK version #

To use the standalone version, you must first install jack and then have it running before starting the application. You need a bit of dedication to take this route, so **it is not recommended for the faint of heart**.

The release also contains a JACK application. JACK is a handy mechanism to route audio to and from applications. This allows patching together a virtual studio from separate audio programs. The standalone application also contains a GUI which imitates the (red) Yamaha YC20.

![http://foo-yc20.googlecode.com/svn/trunk/graphics/screenshot-800.png](http://foo-yc20.googlecode.com/svn/trunk/graphics/screenshot-800.png)

Note: There is a headless command line version for those who do not want or need the GUI.


## Installing JACK ##

Jack is available to download at [the jack website](http://jackaudio.org/download). The _tgz_ file is a package which contains an installer in the bin/windows directory. That will install jack and a graphical user interface you can use to control and set up jack (Jack Control). Using the control panel included in the 1.9.6 release is a bit tricky but later versions should make it easier.

A tutorial on how to set up jack in Windows is greatly appreciated.

## Jack and MIDI ##

The Foo YC20 jack application uses Jack to route midi to it. To get your MIDI devices to appear in the Jack Control connections dialog, you need to add "-X winmme" (without the quotes) in the setup page in the _Server Path_.



---


_VST is © 2004, Steinberg Media Technologies, All Rights Reserved_