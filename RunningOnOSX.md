# Foo YC20 VST #

By far the easiest way to use the Foo YC20 organ is to use the included VST plugin. You can integrate the plugin into a host of your choosing and have the organ running in your sequencer etc.

However, due to the nature of the organ processing, it is worth noting that the VST plugin uses a lot of CPU power. This is regardless of whether it is playing sounds or not.

# The Jack application #

Foo YC20 for OS X also includes a standalone JACK application. JACK is a handy mechanism to route audio to and from applications. This allows patching together a virtual studio from separate audio programs.

# Installing JACK #

The easiest way to get JACK running on OS X is to install [JackPilot](http://www.jackosx.com/). Select the correct installer for your specific version of OS X. then follow the install instructions. Finally, the installer asks to restart your computer. After installation, you will find JackPilot in the Applications under a directory called Jack/.

# Running JACK #

When you start JackPilot, you will be presented with the main interface. The first time you start you will also see the preferences dialog. You can select a sampling rate, the audio device to use etc. The buffer size parameter is crucial as it defines the latency of the system. The lower the value, the faster response you will get at the expense of higher CPU load.

Before starting Foo YC20, you need to start jack using the main JackPilot interface.

# Making connections #

To control the organ and to hear the output, you need to do connections. These connections are kind of like connecting gear together using cables. However with JACK, these cables are virtual. You can open the routing dialog from the JackPilot main interface. There you can connect the output of the organ to your soundcard (or another program) and you can connect your MIDI keyboard to the organs MIDI input.


You can find more information in the documentation that is installed with JackPilot.

## Jack and MIDI ##

The Foo YC20 jack application uses Jack to route midi to it. As it stands, setting up MIDI support in Jack is quite difficult in OS X. This makes playing the standalone organ quite difficult and is a reason why at this point in time, the OS X release is still unannounced.


# FAQ #

**Q:** Why JACK?

**A:** Foo YC20 is developed on Linux. In the Linux audio ecosystem, JACK is the de-facto method of low-latency audio. The OS X release is done based on this work and thus this it inherits. More information on JACK can be found at http://jackaudio.org/

**Q:** I don't have a MIDI keyboard, but I'd like to try this.

**A:** You can try a virtual MIDI keyboard. One open source option is [vmpk](http://vmpk.sourceforge.net/).


---


_VST is © 2004, Steinberg Media Technologies, All Rights Reserved_