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

# Searching for files
## Using Find
The find command is fantastic in the sense that it can be used both very simply or rather complex depending upon what it is you want to do exactly. However, let's stick to the fundamentals first.
Take the snippet below; we can see a list of directories available to us:
<img width="510" height="121" alt="image" src="https://github.com/user-attachments/assets/0569a6c8-97d4-4463-9ec7-1f257c263f60" />

Now, of course, directories can contain even more directories within themselves. It becomes a headache when we're having to look through every single one just to try and look for specific files. We can use **find** to do just this for us!  
There are two cases:
* We know the exact file name we're looking for. Let's say in this case, we're looking for "passwords.txt". We can simply use **find -name passwords.txt** where the command will look through every folder in our current directory for that specific file like so:
  <img width="510" height="144" alt="image" src="https://github.com/user-attachments/assets/76c497e9-772c-485d-b17d-380d75cc23e6" />

* We don't remember the exact file name but we know its format. Let's say we're looking for a *.txt* file. We can simply use what's known as a wildcard (*) to search for anything that has .txt at the end. In our case, we want to find every .txt file that's in our current directory. We will construct a command such as **find -name *.txt*** . Where "Find" has been able to find every .txt file and has then given us the location of each one:
<img width="510" height="146" alt="image" src="https://github.com/user-attachments/assets/77eeb0f8-cb7e-404d-ba32-95c715102d9c" />

## Using Grep
Another great utility that is a great one to learn about is the use of *grep*. The grep command allows us to search the contents of files for specific values that we are looking for.

Take for example, the access log of a web server. In this case, the access.log of a web server has 244 entries.
<img width="510" height="129" alt="image" src="https://github.com/user-attachments/assets/3051bfdb-cc99-48a1-a812-19cdf1303d50" />
Using a command like cat isn't going to cut it too well here. Let's say for example if we wanted to search this log file to see the things that a certain user/IP address visited? Looking through 244 entries isn't all that efficient considering we want to find a specific value.

We can use grep to search the entire contents of this file for any entries of the value that we are searching for. Going with the example of a web server's access log, we want to see everything that the IP address "81.143.211.90" has visited (note that this is fictional)
<img width="1200" height="119" alt="image" src="https://github.com/user-attachments/assets/3112b0c3-fece-4b45-8ce5-a8a6d4d8457c" />
"Grep" has searched through this file and has shown us any entries of what we've provided and that is contained within this log file for the IP.
## Searching Recursively with grep
Sometimes, the information we are looking for is spread across multiple files inside a directory. Instead of checking each file individually, we can tell grep to search recursively through all files and subdirectories.

To do this, we use the -R (recursive) option.
For example, to search for a variable across all files in the current directory and its subfolders, we can run:
<img width="294" height="46" alt="image" src="https://github.com/user-attachments/assets/0f15c463-f14b-453d-b87e-215ea15065f8" />
This will:

* Search every file in the current directory
* Search all subdirectories
* Show where the PRETTY_NAME appears

**Example output:**
<img width="389" height="85" alt="image" src="https://github.com/user-attachments/assets/e060dd89-21b2-4b0a-bafc-304a8a81b9a6" />
The file path is shown before the matching line, making it easy to identify where the result was found.

## Creating Files and Folders (touch, mkdir):

Creating files and folders on Linux is a simple process. First, we’ll cover creating a file. The touch command takes exactly one argument — the name we want to give the file we create. For example, we can create the file “note” by using touch note. It's worth noting that touch simply creates a blank file. You would need to use commands like echo or text editors such as nano to add content to the blank file.

### Using touch to create a new file:
<img width="395" height="93" alt="image" src="https://github.com/user-attachments/assets/6ec88865-9328-4f68-8ffd-17d73e1de899" />

This is a similar process for making a folder, which just involves using the mkdir command and again providing the name that we want to assign to the directory. For example, creating the directory "mydirectory" using mkdir mydirectory.

### Creating a new directory with mkdir:
<img width="353" height="114" alt="image" src="https://github.com/user-attachments/assets/84879808-f53a-4252-a067-2cd92396e367" />

## Removing Files and Folders (rm):

rm is extraordinary out of the commands that we've covered so far. You can simply remove files by using rm. However, you need to provide the -R switch alongside the name of the directory you wish to remove.

### Using rm to remove a file
<img width="353" height="94" alt="image" src="https://github.com/user-attachments/assets/bec319b2-cf6a-4822-ac28-ddbb6e267990" />

### Using rm recursively to remove a directory
<img width="353" height="104" alt="image" src="https://github.com/user-attachments/assets/fd5d127b-3608-4ae5-af95-4dd9816886ea" />

## Copying and Moving Files and Folders (cp, mv):

Copying and moving files is an important functionality on a Linux machine. Starting with cp, this command takes two arguments:

    1.  the name of the existing file

    2. the name we wish to assign to the new file when copying

cp copies the entire contents of the existing file into the new file. In the screenshot below, we are copying "note" to "note2".

### Using cp to copy a file
<img width="353" height="97" alt="image" src="https://github.com/user-attachments/assets/af51f2bd-c961-4058-9ff2-a5405a24999a" />

Moving a file takes two arguments, just like the cp command. However, rather than copying and/or creating a new file, mv will merge or modify the second file that we provide as an argument. Not only can you use mv to move a file to a new folder, but you can also use mv to rename a file or folder. For example, in the screenshot below, we are renaming the file "note2" to be named "note3". "note3" will now have the contents of "note2".

### Using mv to move a file
<img width="353" height="105" alt="image" src="https://github.com/user-attachments/assets/590d71fd-52da-47eb-92f8-731e3f7f20db" />  

## Determining File Type

What is often misleading and often catches people out is making presumptions from files as to what their purpose or contents may be. Files usually have what’s known as an extension to make this easier. For example, text files usually have an extension of “.txt”. But this is not necessary.

So far, the files we have used in our examples haven’t had an extension. Without knowing the context of why the file is there — we don’t really know its purpose. Enter the **file** command. This command takes one argument. For example, we'll use **file** to confirm whether or not the "note" file in our examples is indeed a text file, like so **file note**.

### Using file to determine the contents of a file
<img width="353" height="90" alt="image" src="https://github.com/user-attachments/assets/7ec14e07-3bab-4c00-90e6-f04f2d55a915" />








