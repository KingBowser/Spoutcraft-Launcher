This is a modified tekkit launcher that supports a sort of "Ignore Incongruous MD5 Sum(s) Feature".
It was made in response to the obscenely odd MD5 mismatches occurring due to what appears to mod repository negligence.

------------------

Technic Launcher (based off SpoutCraft Installer)

The goal of this launcher is to provide a one-click method to switch modpacks and versions in as simple a manner as possible for the end user!

-------------------

Main Technic site is here: http://technicpack.net/

and the forums are here: http://technicpack.net/forums/

-------------------

A personal note to the spout and technic devs:
I highly suggest that you read the java code conventions. Your code is embarrassingly messy, and pretty much implementation-specific where it should be implementation-inspecific (ie: NOT having methods to describe individual properties in SettingsUtil.java).
I assume that your poor idea of code quality originates from that of decompiled minecraft, and the minecraft launcher. Whilst I do not mean this offensively (I learned java that way too, however I then learned the standards), it can do some disgusting things to the code that you produce should you not catch up on the standards from sun/oracle.
Nonetheless, I don't blame you for the horrible UI syntax, swing nearly violates all of the code conventions laid down by it's very creators.

Futhermore, you need to look in to singletons instead of creating massive files ful of static members, it's really quite awful.
Static members are mean to be in files that will also have individual instances with instance-members.
