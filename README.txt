-------------
What is this
-------------

This is a collection of the DEFAULT plaintext files of interest from various Xbox games. It is not a list of ALL games with plaintext files of interest, nor is it a list of ALL plaintext files that could be modified to do interesting things.

-------------
Why did I do it
-------------

With the return of Xbox live (https://insignia.live) as well as improvements in capabilities of Xbox emulators, I thought it would be interesting to see what more the Xbox could do.  Creating this GitHub repository is a way to increase community awareness and to increase community participation in the effort to improve the Xbox experience for: Online gaming, Systems with 128mb RAM, Systems with overclocked or upgraded CPUs, xEMU and CXBX playback. Additionally, it may open up the doors to additional modifications such as Fan Translations into additional languages, new maps, new skins, new functionality, or porting features from PC games into Xbox. There may be additional opportunities as well and the more eyes we have the more we might be able to do.

-------------
What can you actually do with these files
-------------
There are already a few things you might gather just from the "Why did you do it" above. Of course not all games have any capabilities to make modifications, and ones which do support varying level of modifications.
But here are some examples of what is possible:
 - Increase Graphical details (such as for emulators or systems with added memory or cpu resources)
 - Decrease Graphical details (for instance to increase FPS)
 - Modifying advanced keybindings not avialable in game
 - Increase available memory to games (systems with 128mb or emulators that can handle additional RAM)
 - Localization / Language translations
 - Skip intros or re-order games
 - Swap audio, video, textures, etc.
 - Enable debug features
 - Enable hidden functionality
 - Increase available bandwidth for servers and clients for online gaming
 - Add ability for clients to get game updates from dedicated servers (such as map packs)
 - Add / remove content from games (such as porting new maps or levels from PC versions)
 - .....
 - .....
 - many more

-------------
Content Layout
-------------

\GAMES\Game Name\
	Description: Contains cleartext files of interest from the game disks. Nested folder structures represent actual file paths.
		Modification of these files requires the use of a modified console.

\UDATA\########
	Description: Contains cleartext files of interest from the E:\UDATA\ directory on the xbox.
		Modification of these files does not require a modified console.
		You just need a way to transfer the files to the system such as using a USB->Xbox controller port adapter and using a Flash drive as your memory card and copying them to the system.
			**Some files can run from memory card while others must be installed to the HDD

\TWEAKS\
	Description: Will contain various catagories of tweaks for various games

\TWEAKS\Networking\
	Description: Contains list of modifications intended to increase network performance.