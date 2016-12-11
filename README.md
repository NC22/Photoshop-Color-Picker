# Photoshop-Color-Picker
Simple HSV color picker for Photoshop. Based on my <a href="https://github.com/NC22/HTML5-Color-Picker">HTML5 widget</a>

<img src="https://raw.githubusercontent.com/NC22/Photoshop-Color-Picker/master/widget.png">

Some notices about how to compile the extension :

To compile the extension for install throw Photoshop Extension Manager (also any way you will need to create sertificate to use extension without debug mode, even if you install it manually)

1. Install Eclipse
2. Install Adobe Extension Builder 3
3. Open project throw Eclipse
4. Go to File -> Export -> choose Adobe Extension Builder 3 -> Application Extension -> Next -> Create sertificate and choose Export directory 

To run Photoshop in debug mode in Windows

1. run regedit.exe
2. go to brunch HKEY_CURRENT_USER -> Software -> Adobe -> CSXS.4 (or CSXS.6 .. etc depends on Photoshop version) -> create register option "PlayerDebugMode" = 1

Installed extensions in Photoshop stored in (by default)

Photoshop 2015 and newer

C:\Program Files (x86)\Common Files\Adobe\CEP\extensions

for old versions

C:\Program Files (x86)\Common Files\Adobe\CEPServiceManager4\extensions

<b>Warning</b>

By default Adobe Extension Builder 3 sets in the manifest file of extension incorrect version of Photoshop, you must check it manually in file "manifest.xml" check values in HostList section. Verion must be setted to Version="[14.0,99.9]"
