DirtyUnicorns For Xiaomi Redmi 2/Prime/Pro
======================================

Initializing:

First, create a folder to hold the source code: 

	mkdir ~/du

Next, naviate into that new directory via the terminal:

	cd ~/du

To initialize your local repository using the Turbo ROM trees, use this command:

	repo init -u http://github.com/DirtyUnicorns/android_manifest.git -b n7x-caf

Also add the local manifests:

	git clone https://github.com/Ayushd70/local_manifest -b android-7.1 .repo/local_manifests

Then sync up with this command:

	repo sync --force-sync
	
You can make the 4 higher depending on how fast your internet connection is. 

-------------
 
_Building from source_
---------------

First:

	cd ~/du

Second:

	$ echo "export USE_CCACHE=1" >> ~/.bashrc
	$ prebuilts/misc/linux-x86/ccache/ccache -M 50G

Third:

	. build/envsetup.sh
	brunch wt88047
