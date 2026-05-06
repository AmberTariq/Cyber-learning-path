## What is SSH & how Does it Work?
Secure Shell or SSH simply is a protocol between devices in an encrypted form. Using cryptography, any input we send in a human-readable format is encrypted
for travelling over a network -- where it is then unencrypted once it reaches the remote machine, such as in the diagram below.

<img width="466" height="129" alt="image" src="https://github.com/user-attachments/assets/69d94bcd-02b9-4a78-8ade-459e4667324a" />  


* SSH allows us to remotely execute commands on another device remotely.
* Any data sent between the devices is encrypted when it is sent over a network such as the Internet

## Introduction to Flags and Switches
A majority of commands allow for arguments to be provided. These 
arguments are identified by a hyphen and a certain keyword known as flags
or switches.  

When using a command, unless otherwise specified, it will perform its
default behaviour. For example, **ls** lists the contents of the working
directory. However, hidden files are not shown. We can use flags and
switches to extend the behaviour of commands.

Using our **ls** example, **ls** informs us that there is only one folder named
"folder1" as highlighted in the screenshot below.

<img width="550" height="100" alt="image" src="https://github.com/user-attachments/assets/a8610f60-6e46-4d37-ac2d-fc79beac96b6" />

However, after using the
**-a** argument (short for--all), we now suddenly have an output with a few more files and folders such as **".hiddenfolder"**. Files and folders with "." are hidden files.

<img width="594" height="63" alt="image" src="https://github.com/user-attachments/assets/327fbc98-f0eb-4fd7-9dbb-eaed28c97f2c" />
