# An Introduction to Shell Operators

Linux operators are a fantastic way to power up your knowledge of working with Linux. There are a few important operators that are worth noting. We'll cover the basics and break them down accordingly to bite-sized chunks.

At an overview, I'm going to be showcasing the following operators:
<img width="631" height="418" alt="image" src="https://github.com/user-attachments/assets/5331cfb8-ce32-40e8-a65d-a48d1ea1175a" />
## Operator "&"
This operator allows us to execute commands in the background. For example, let's say we want to copy a large file. This will obviously take quite a long time and will leave us unable to do anything else until the file successfully copies.

The "&" shell operator allows us to execute a command and have it run in the background (such as this file copy) allowing us to do other things!

## Operator ">"
This operator is what's known as an output redirector. What this essentially means is that we take the output from a command we run and send that output to somewhere else.

A great example of this is redirecting the output of the echo command that we learned in "Basic Commands". Of course, running something such as echo howdy will return "howdy" back to our terminal — that isn't super useful. What we can do instead, is redirect "howdy" to something such as a new file!

Let's say we wanted to create a file named "welcome" with the message "hey". We can run **echo hey > welcome** where we want the file created with the contents "hey" like so:
<img width="346" height="88" alt="image" src="https://github.com/user-attachments/assets/d7371490-971b-44e3-80d6-801f670be792" />

             *Note: If the file i.e. "welcome" already exists, the contents will be overwritten!*
