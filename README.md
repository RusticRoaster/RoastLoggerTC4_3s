RoastLoggerTC4_3s
=================

Modification to RoastLoggerTC4 sketch to work with SainSmart lcd Shield

Requires the following modification to the sainsmart shield
you want all functionality of the TC4.

Cut or remove D9 and D10 from the Sainsmart LCD shield

Add a jumper wire from D9 pad to D11 pad on SainSmart shield

Add a jumper wire from D10 pad to D12 pad on SainSmart shield


If you just want to monitor temps and dont plan to use the
OT pins no modifications to the shield are needed.

change this line in RoastLoggerTC4_3s.ino

HIDbase hid(8, 11, 4, 5, 6, 7); // interface

to

HIDbase hid(8, 9, 4, 5, 6, 7); // interface


sbuttons files could be moved to a user library directory, they were placed in the working directory
for ease of downloading.
