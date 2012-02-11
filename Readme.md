MySqueakQl
=============

History
-------
This project is more of a 'demonstration of the possible' rather than an actively supported project.  I had need to access a MySQL server from an iOS device, but discovered that Oracle's dual licence requirements of their client driver (libmysql) effectively precluded the sale of any app that linked to their client libraries (unless you purchased a commercial license, a request that oracle did not respond to.) or the GPL'ing of my code :(

So this is a *VERY* basic and *VERY* rough minimal Objective-C implementation of a mysql client driver that does the minimum I need to solve my requirements.

As such I have no intention to support this code, but have licensed it as MiT so that others could use it or build upon it.  

It was developed in a clean room fashion based solely on the documentation found at http://forge.mysql.com/wiki/MySQL_Internals_ClientServer_Protocol and from diagnostic information gleaned with WireShark which means there should be no GPL infected code present.

As a side note, ObjectiveC is not a language I'm overly familiar with, so this code is of pretty poor quality but may help others access MySQL effectively from their devices.

Dependencies
------------
The only non iOS dependency currently is I'm using the sha functions in libcrypto, but I'll move that to use the commoncrypto library shortly.

License
-------
MIT licensed, but be aware this code is *not* production ready, probably has memory leaks and should be considered to be purely a 'safe' (non GPL'd) example to base your own implementation on :)