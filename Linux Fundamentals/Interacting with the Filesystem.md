# Interacting With the Filesystem
 As I previously stated, being able to navigate the machine that you are logged into without relying on a desktop environment is pretty important. After all, what's the point of logging in if we can't go anywhere?
<img width="450" height="300" alt="image" src="https://github.com/user-attachments/assets/eb5c2055-2fe1-4a58-b381-2f29f3f287c7" />
## Listing Files in Our Current Directory (ls)
 Before we can do anything such as finding out the contents of any files or folders, we need to know what exists in the first place. This can be done using the "ls" command (short for listing)
 <img width="531" height="108" alt="image" src="https://github.com/user-attachments/assets/f16bcd05-ad6e-4dbb-b885-d67c4b9c322d" />

*Pro tip: You can list the contents of a directory without having to navigate to it by using ls and the name of the directory. I.e. **ls Pictures***

## Changing Our Current Directory (cd)
Now that we know what folders exist, we need to use the "cd" command (short for change directory) to change to that directory. Say if I wanted to open the "Pictures" directory - I'd do "cd Pictures". Where again, we want to find out the contents of this "Pictures" directory and to do so, we'd use "ls" again:
<img width="531" height="106" alt="image" src="https://github.com/user-attachments/assets/5370b981-786f-47cd-b21f-d91b5defb12a" />
In this case, it looks like there are 4 pictures of dogs!

## Outputting the Contents of a File (cat)
Whilst knowing about the existence of files is great — it's not all that useful unless we're able to view the contents of them. we're going to talk about simply seeing the contents of text files using a command called "cat".  
"Cat" is short for concatenating & is a fantastic way for us to output the contents of files (not just text files!).
In the screenshot below, you can see how I have combined the use of "ls" to list the files within a directory called "Documents":
<img width="531" height="146" alt="image" src="https://github.com/user-attachments/assets/8bd3b735-76ce-4126-9447-489faea8eda6" />

We've applied some knowledge from earlier in this task to do the following:

* Used "ls" to let us know what files are available in the "Documents" folder of this machine. In this case, it is called "todo.txt".
* We have then used cat todo.txt to concatenate/output the contents of this "todo.txt" file, where the contents are "Here's something important for me to do later!"

   *Pro tip: You can use cat to output the contents of a file within directories without having to navigate to it by using cat and the name of the directory. **I.e. cat /home/ubuntu/Documents/todo.txt***

 Sometimes things like usernames, passwords, flags or configuration settings are stored within files where "cat" can be used to retrieve these.

## Finding out the full Path to our Current Working Directory (pwd)
It's easy to lose track of where we are on the filesystem exactly, which is why I want to introduce "pwd". This stands for **p**rint **w**orking **d**irectory.  
Using the example machine from before, we are currently in the "Documents" folder — but where is this exactly on the Linux machine's filesystem? We can find this out using this "pwd" command like within the screenshot below:  
<img width="475" height="127" alt="image" src="https://github.com/user-attachments/assets/75aa513c-6776-4757-8dca-6ec1760e7136" />

