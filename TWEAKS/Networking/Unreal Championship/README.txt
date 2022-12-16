Changes in the configuration file assume you at least 10mbit upload. 

	Purpose: Increase online performance with XBL.
		Unreal Championship was one of the first XBL games and due to this, it was very modestly tuned for the internet connections of 2002.  This game is a different build of Unreal 2k3, and therefore we can use the information the UT2k3 and UT2k4 modders have already learned and put it to use for Xbox.

	Details & Warnings:
		The primary items changed are listed below. Please note that Unreal Championship 2 uses a default value of ConfiguredInternetSpeed=10000, so that is a very safe value to use. But 10001 is required to have an "unlocked framerate" during online gaming.  You can further increase this value up to 20000 if your have ~20mbit upload available. However if you increase the value higher than you can sustain, you will create additional traffic and cause yourself issues. So be careful.

System\default.ini

[Engine.Player]
ConfiguredInternetSpeed=10001
;ConfiguredInternetSpeed=2400
;	 Default above ^^^^^=2400kbps UPLOAD
:	Unreal Championship 2 sets a default value of 10000. At 10001 it unlocks maximum framerate for online gaming.
; 	Set value between 2400 and 20000 based on your internet UPLOAD speed.
;		- DO NOT SET HIGHER THAN 20000 since that is the most servers can handle per client.
; 		- Info here - https://www.utzone.de/forum/showthread.php?t=4326
; 		- More Info here - https://wiki.unrealadmin.org/Netspeed_Tutorial_(UT)
ConfiguredLanSpeed=20000
; ConfiguredLanSpeed is only useful for local system link.
;	If you are on a 100mbit switch you should leave this value alone. 
;	If you are using a 1gbit switch, you can increase this value.
bMaxframespersecond=60
; bMaxframespersecond= is new setting added to this config.

[XboxDrv.XboxClient]
MinDesiredFrameRate=35.000000
; MinDesiredFrameRate=  This setting was not originally in this file
;	 When configured, the game will target a minimum desired framerate at the expense of graphics.
;		However, the xbox is already running Lower details on almost all settings. So the impact of this may be minimal.

[D3DDrv.D3DRenderDevice]
DetailTextures=True
HighDetailActors=False
;HighDetailActors=True
; Changed to False as an attempt to improve XBOX Live FPS at the expense of enemies are lower detail.
DesiredRefreshRate=60
; DesiredRefreshRate is linked to UseVSync setting. 
; 	On a real XBOX, you are limited to 60Hz with VSync enabled.

;--------
; If running a dedicated server, modify these options below
;--------

[Engine.GameReplicationInfo]
ServerName=SERVER NAME HERE
ShortName=SHORTNAME
AdminName=ADMINNAME
Region=0
; region list can be found here - https://wiki.unrealadmin.org/Tweaking_your_server_ini_(UT)
MOTDLine1=Hi!
MOTDLine2=Hi!
MOTDLine3=Hi!
; MOTDLineN= appear when CLIENTS connect to the SERVER

