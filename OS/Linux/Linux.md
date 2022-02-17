# Linux

## Directories
- `/bin`: The bin folder contains binaries (also known as executables) that are essential to the system

- `/sbin`: This folder is almost the same as the `/bin` folder, but it contains only binaries that are accessible to the superuser (root).

- `/lib`: This folder is for libraries. Here there is mostly code that is shared between binaries.

- `/usr`: This folder is for binaries that are not essential to the system. Think of binaries of applications for the end-user.

	- `/bin`: This folder is for the binaries that are not essential for the system and are meant for the end-user.

	- `/local`: This folder is used for binaries that the user compiles themself it is in a separate folder than the `/bin` folder above so that the binaries that applications install won't conflict with the user's own binaries.
	
- `/etc`: This folder stands for "Editable Text Config". This folder is mostly used for config files that can be edited here.

- `/home`: This folder contains folders named after every user registered in the system. It contains the files, configuration, and software for that user. You can only modify it if you are logged in as that user or a superuser.

- `/boot`: It contains all the files needed to boot the system.

- `/dev`: It stands for "Device Files". Here you can interface with hardware or drivers like they are regular files. You can also make petition files here.

- `/opt`: This folder contains optional or add-on software.

- `/var`:  This folder contains variable files that change when the system is being used most of the times things like logs and cache files are stored here.

- `/tmp`: Everything in this folder is temporary. It will get wiped after a reboot.

- `/proc`: This folder does not exist on the hard disk but is instead made in memory so that the system can keep track of running processes.