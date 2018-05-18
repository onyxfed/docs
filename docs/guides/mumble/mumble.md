# Mumble

Mumble is a third-party VOIP (Voice Over Internet Protocol) application that allows people to communicate verbally both in- and out-of-game.

Mumble is mostly used in two situations: PvP and Alerts. In PvP, it is most useful because; for example, it is faster to call out a primary target than to type it, especially with PvP related to lag. Alert wise, mumble can be used to provide a quick and efficient response to those in distress.

## Mumble Quick Connect Guide
---

The set-up instructions are as follows:

Download Mumble from [http://wiki.mumble.info](http://wiki.mumble.info). Versions for many different operating systems are available.

   1. Install and set it up - starting Mumble for the first time will start two wizards, for certificates and audio tuning. See the [FAQ](https://wiki.mumble.info/wiki/FAQ) if you have any issues.
   2. You must set a push-to-talk key - do not use voice activation.
   3. Click on Server > Connect > Add New... and create a server using the details below:

<center>

|            |                                                                                  |
|:----------:|:--------------------------------------------------------------------------------:|
| Servername | Onyx Federation                                                                  |
| Address    | voice.onyxfed.space                                                              |
| Port       | 64738 (default)                                                                  |
| Username   | *<Your username that was generated for you on the auth site. [mumble service]\>* |
| Password   | *<Your password that was generated for you on the auth site. [mumble service]\>* |

</center>

A more detailed guide to set-up and troubleshooting is below, along with how to get the overlay to work.

## Setting Up Mumble
---

### Audio Tuning Wizard

When you run Mumble the first time, an Audio Tuning Wizard is presented to you. If you skip or miss it on the first run you can retake the wizard by clicking Configure > Audio Wizard. It is recommended you go through it carefully, since setting up Mumble correctly will make your and everyone else's life much easier (going through the Audio Tuning Wizard properly will also normalise everyone's voices, such that everyone will sound the same volume regardless of how they have their microphone set up).  However there are two things to pay close attention to:

#### Push-to-talk

![Imgur](https://i.imgur.com/myVt34M.png)

When you reach a screen that looks like the one above select the top radio button, click on the box on the same line and press the key you you want to use as the push-to-talk key.This is your normal push-to-talk key; for certain Fleet roles you may need more than one (see the comments in the Fleet channels), but for general ONY activity one is sufficient.

#### Text-to-Speech
![Imgur](https://i.imgur.com/uQZIRy1.png)

When you reach a screen that looks like the one above, it is recommended that you disable the text to speech notifications.

### Connecting to the Onyx Federation Server 

Once Mumble is all set up and you have run through the Audio Tuning Wizard, you will want to connect to the Onyx Federation server.  

   1. Go to Server in the toolbar --> Connect.
   2. Click the Add New... button in the bottom right.
   3. Put anything you like in the Label box ("Onyx Federation" seems sensible), the Address box needs to be voice.onyxfed.org and the Port needs to be left as default (64738).
   4. The Username box needs to be the exact username generated for you on the auth site, which also happens to be your exact character name with spaces replaced by underscores.
   5. Click the Connect button.
   6. The server will reject your connection, and prompt you with a Wrong Password box.  You need to use the password that was generated for you on the auth site or the one you changed it to, in the box, then click OK.

#### Speaker and Microphone Choices

When you went through the wizard set-up, you may have left the microphone and speaker choices on "default." This is a normal thing to do, and it means that mumble will send sound out through your normal speaker, and listen on your normal microphone. For many players this will work fine.

If the sound is coming from the wrong speaker, though, like for example your computer speaker instead of your headphones; or if your voice is not coming through clear and strong when you do the microphone check, you may want to change those default settings.

  * First open Mumble Preferences.
  * To change microphones, click on Audio Input. This is the first item in the Preferences, and is also the page where you set the Push-To-Talk key. At the top of the page is the word "Device" and next to it is a menu list of all the audio input devices connected to your computer. These may have strange names ... mine are things like "USB Audio CODEC" and "Mic 96K" ... so you may just have to click each one and do the microphone check to pick the one that works best.
  * To change speakers, click on Audio Output. Again it says "Device" at the top and there is a menu list. There should be at least two devices on this list: your computer's speakers, and your headphones. If you're not sure which is which, try each one with a microphone check until the sound comes out where you want it to.
     
Note: if you want to listen to Mumble through your computer speakers, the slider labeled "Attenuate Applications By..." will reduce the sound of the EVE game (and any other apps that might be running) by the percentage you choose - but only when Mumble is active. This lets Mumble talk stand out from the sounds of combat and such.

## Using the Onyx Federation Mumble
---

### Notificiations

In the Configure --> Settings screen you can find Advanced settings checkbox in the bottom left corner. With it checked you can access the Messages settings. From there you can disable popup and sound notifications about events you don't care about.  By default Mumble makes a loud PING and gives you a notification popup for almost any event on the server - this gets annoying pretty fast.

Mac version: From the Mumble --> Preferences window (make sure the 'Advanced' checkbox in the upper right is checked), select the 'Messages' tab. The only way to eliminate audio notifications is to uncheck items in the 'Soundfile' column.

## Mumble Overlay
---

Mumble provides a very handy and customizable overlay. To configure it go to Configure --> Settings --> Overlay option.

Mumble, being the awesome program that it is, shows in this window an example of what the overlay will look like on your current desktop, as well as instructions on how to alter it.  One position that works very well is just to the right of the current location name, like the screenshot on the right.  You could even put it above the current location, but then - for me at least - it's too small to see easily.

The default setting is for the Overlay to display the name of everyone currently in the channel.  As you can imagine, this gets unwieldy very quickly.  To change this, right-click on the small example overlay in the window, choose Filter >, and tick Only talking.  Also untick Always show yourself, otherwise your name will constantly be displayed on the overlay.

The Edit... option on the right-click menu produces a detailed configuration screen where you can change pretty much anything you like about the overlay: colours, sizes, backgrounds, avatars, etc.

If your overlay is not showing up, it might be because you started Mumble whilst EVE was already running. If necessary simply restart EVE. If the overlay is still not showing, check the troubleshooting section below.

![Imgur](https://i.imgur.com/0NwbQLb.png)

### Overlay on Windows 10

The Mumble Overlay often doesn’t work on the EVE client with Windows 10 without some additional work. Many of the usual work-arounds won’t fix the problem. A reliable fix that is compatible with DirectX 11 can be done with the following two steps.

   1. Download and install the current Mumble Snapshot from [http://wiki.mumble.info/](http://wiki.mumble.info/). Use the Development Snapshot version instead of the Stable Release version and use the first listed (“Windows” -- Do Not use the “Windows x64” version). You can install the Snapshot version over your current version of Mumble. You don’t have uninstall the current version first.
   2. Next, put the location of the EVE client, “exefile.exe”, into the Mumble Overlay Whitelist. To find the Whitelist, open the Mumble Configuration (Menu: Configure/Settings or the Gear icon). Then select Overlay on the left side menu. Next select the Overlay exceptions and click on the Whitelist. Use the Add button at the bottom to add the location of your exefile.exe. The familiar Open File window will allow you to find the path, select the file, and add it to the Whitelist.

<img align="right" src="https://i.imgur.com/vcWSAhc.jpg">

If you don’t know where your "exefile.exe" file is located, go to the EVE Launcher, open the dropdown menu from the top right corner, and select the Shared Cache option. The pop-up window will show the full path of the Shared Cache folder and the Tranquility exefile.exe will be located in the "\SharedCache\tq\bin folder". 

The file might be located in the "ProgramData" folder which is a hidden folder. You might have to unhide it using File Explorer. If you want to add the path for the Singularity or Duality test servers, add the path that contains “\SharedCache\sisi\bin\exefile.exe” or “\SharedCache\duality\bin\exefile.exe” instead of "\SharedCache\tq\bin\exefile.exe".

### Overlay on Linux

To actually display the overlay over EVE in Linux after you've enabled it in Mumble's settings you need to have Mumble launched first and then run mumble-overlay in front of the wine command that you use to launch EVE. For example:

mumble-overlay wine explorer /desktop=EVE,1600x1200 "C:\Program Files\CCP\EVE\eve.exe"

If you use a WINEPREFIX, then you would insert it after the WINEPREFIX variable like so:

WINEPREFIX=/home/username/bin/wine/wine-eve/ mumble-overlay wine explorer /desktop=EVE,3200x1180 "C:\Program Files\CCP\EVE\eve.exe"

### Overlay on Mac

The overlay in the 1.2.3a stable release works with Mac OS X 10.7 (Lion), but not with Mac OS X 10.6 (Snow Leopard). You'll need to install the developer snapshot from [http://mumble.sourceforge.net/](http://mumble.sourceforge.net/) to get a working overlay in Snow Leopard.

In all cases, it is essential that Mumble be running before the EVE client is started for the overlay to work in EVE.

#### Version 1.2.3.a

#### Installing the Overlay

   1. After downloading and mounting the Mumble install dmg, drag and drop the Mumble application into the folder of your choice.
   2. Launch Mumble.
   3. Click Mumble -> Preferences… and go to the Overlay section in the Preferences window that opens.
   4. Click the [Install Mumble Overlay] button. If prompted, authenticate using an account with Admin rights.
     * The window will update once the overlay is installed.
   5. Tick the [Enable Overlay] checkbox if it's not already ticked.
   6. Click [OK] to close the Preferences window.

Congratulations, you now have a working overlay! Well, kind of. You'll probably want to make some configuration changes.

### Configuring Overlay

   1. With the Mumble application still running, launch EVE.
   2. If you run EVE in full-screen mode, press the [Command]+[Enter] keys to put it into windowed mode.
   3. Switch to Mumble and click Mumble -> Preferences… and go back to the Overlay section.
   4. In the Layout tab in the bottom half of the window, use the screen preview to:
      1. Move the red dot to anchor the overlay where you want it.
      2. Hover the mouse over the overlay and scroll in/out to increase/decrease the size of the overlay.
      3. Right-click the overlay and in the Filter menu check [Only Talking] (or [Talking and recently active]) and uncheck [Always show yourself].
      4. Adjust other settings as desired. Right-click the overly and select Edit to customise the look of the overlay (e.g., background and font colour for the talk/shout/whisper).
   5. Click Ok to save the changes.
   6. With Mumble running in the background, you can now switch back to EVE. Press [Command]+[Enter] if you want to put EVE in full-screen mode.
   7. 
Your overlay is now setup and you are ready to go!

Again - be sure to start Mumble first before EVE from here on out.

"In the EVE settings make sure that you have checked "Use Multithreaded OpenGL"'. Without it the overlay will not work in EVE and will crash the client on startup.

## Troubleshooting
---

The Mumble FAQ on the Mumble homepage - [http://mumble.sourceforge.net/FAQ](http://mumble.sourceforge.net/FAQ) - has a lot of useful information, and also has a section on Common Problems and Resolutions which may be helpful.

### I can login to other servers but not the ONY server!

The Mumble download comes with a "backwards-compatible" version.  That program won't work with our server.  Use the up-to-date version. 

### "Server connection failed: The remote host closed the connection."

Third-party certificates (for example the free one from [https://www.startssl.com]([https://www.startssl.com) that Mumble suggests using) do not work with the Onyx Federation Mumble server. Create a new certificate from within Mumble and you should be properly prompted for your password when initially connecting.

### I continue getting the message "Server connection failed: The remote host closed the connection."

Click on the Mumble menu: Configure/Settings and a popup window appears. Click on Network and be sure to UNcheck the [ ] Use Quality of Service (QoS) box. Now click Apply at the bottom right then click OK. The window will close and you will be connected to your server.

## Fallback to Discord, should Mumble go down
---

Not required, just recommended.

Sometimes Mumble goes down, and sometimes ONY is at war (when anyone undocked should be capable of at least listening in Mumble), or you might be in the middle of a fleet op in null-sec. To prepare for the eventuality that they happen at once, it would make sense to prepare by setting up your Discord account on the auth site and configuring your Discord properly.