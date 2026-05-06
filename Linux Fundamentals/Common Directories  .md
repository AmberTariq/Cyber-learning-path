# Common Directories

## /etc

This root directory is one of the most important root directories on your system. The etc folder (short for etcetera) is a commonplace location to store system files that are used by your operating system.

For example, the sudoers file highlighted in the screenshot below contains a list of the users & groups that have permission to run sudo or a set of commands as the root user.

Also highlighted below are the “passwd” and “shadow” files. These two files are special for Linux as they show how your system stores the passwords for each user in encrypted formatting called sha512.

* Some notable contents of the /etc directory:

 <img width="415" height="92" alt="image" src="https://github.com/user-attachments/assets/e61bc7db-8739-4a76-9bef-12aa9109048f" />

 ## /var

The “/var” directory, with “var” being short for variable data, is one of the main root folders found on a Linux install. This folder stores data that is frequently accessed or written by services or applications running on the system. For example, log files from running services and applications are written here (/var/log), or other data that is not necessarily associated with a specific user (i.e., databases and the like).

* Some notable contents of the /var directory:

  <img width="415" height="93" alt="image" src="https://github.com/user-attachments/assets/d63d3ee6-4698-4979-8353-f77aaaa70f9b" />

##  /root

Unlike the /home directory, the /root folder is actually the home for the “root” system user. There isn’t anything more to this folder other than just understanding that this is the home directory for the “root” user. But, it is worth a mention as the logical presumption is that this user would have their data in a directory such as “/home/root” by default.

* Some notable contents of the /root directory:

  <img width="415" height="92" alt="image" src="https://github.com/user-attachments/assets/1b269b90-2be4-4926-a57b-459d481ccd78" />

 ## /tmp

This is a unique root directory found on a Linux install. Short for “temporary”, the /tmp directory is volatile and is used to store data that is only needed to be accessed once or twice. Similar to the memory on your computer, once the computer is restarted, the contents of this folder are cleared out.

What’s useful for us in pentesting is that any user can write to this folder by default. Meaning once we have access to a machine, it serves as a good place to store things like our enumeration scripts.

* Some notable contents of the /tmp directory:

  <img width="352" height="88" alt="image" src="https://github.com/user-attachments/assets/718e5586-5579-4bea-816c-7cf585c2444c" />

