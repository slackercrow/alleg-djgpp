Compile Allegro 4.2.3 from source with DJGPP for DOS on Windows XP
						(Whew what a title!)
====================================================================

I wanted to be able to compile the Allegro DOS library myself. These 
are the zips I used. These are old versions but they work for me to 
compile Allegro 4.2.3 on Windows XP SP3 for MS-DOS.

Just in case, I zipped allegro and djgpp as I have it.

1. Extract allegro-notclean.7z to c:\allegro 
2. Extract djgpp-for-alleg.7z to c:\djgpp
3. Setup environment variables for DJGPP as usual.
4. set LFN=n to compile allegro lib (or it gives an error at one point)
	NOTE: clear LFN before compiling an application (set LFN=)
5. I compiled thusly:
	a. make TARGET_ARCH_EXCL=i386 (TARGET_ARCH_EXCL=i386 is optional,
								   I just did this for a reason.)
	b. make install
	
This may not be ideal, but I have struggled to compile the DOS lib 
with what the djgpp zip picker gives me. This works for my purposes, 
good luck!

NOTE: dj-dl.7z is what I've downloaded from various places, but the zips 
outside of that 7z are the ones I used. I archived them just in case 
they disappear from the web, and if anyone wants to try their own
combination.

NOTE: The djgpp-for-alleg.7z already has a prebuilt working liballeg.lib. 
But I used "make lib" to only build the library. If you want the tools,
examples, and debug or profile builds, follow the instructions above.

DISCLAIMER: None of this is my software. I take no responsibility for
what it may do.

Yours truly,
Slacker Crow