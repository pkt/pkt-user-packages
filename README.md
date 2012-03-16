pkt-user-packages -- Debian packages to manage the lifecycle of user accounts
=============================================================================

These are debian packages that cause a certain user to be created
when they are installed and cause the user to be removed when they
are removed.

NB: WHEN THE USER IS REMOVED, IT'S HOME DIRECTORY GOES BYE-BYE TOO!!
(AS IN RM -RF). DON'T USE THESE PACKAGES IF YOU DON'T KNOW WHAT YOU
ARE DOING!!!

Also, this method should NOT be used for:

    * Users that own *any* file outside their home directory, so
      most likely not for your primary user.

    * System accounts (e.g., www-data)

An example for how this method can be useful is "shuser" a shared
user whose home directory is set to 1777 to allow anyone in the
local machine to write in it (for easy access to remote backups
and things that are shared among computers).

The best way to reuse this project is to fork and adapt to your own needs.
All files in this project should be covered by 3-clause BSD license.
