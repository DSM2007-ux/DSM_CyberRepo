# OverTheWire Bandit notes

Notes on what I learned. 

## Progress

| Level | Done | Main idea |
|---|---|---|
| 0-1 | Y | Print contents of readme |
|1-2| Y  | Print contents of file named -  |

## Commands I've learned

| Command | What it does | Example |
|---|---|---|
| ssh -p | Specifies a port other than the default port 22 | ssh -p 2220 |
| user@host | The username to log in as, and the server to connect to | ssh -p 2220 bandit0@bandit.labs.overthewire.org |
|ls|lists files in a specified directory, current directory if unspecified|ls -la|
|cat|displays contents of a file into the terminal|cat readme|
|./ prefix|Gives a file's path so a name like - isn't read as an option|cat ./-|

## Level notes

### Level 0 to 1
- **Goal:** Locate and print the contents of a readme file 
- **Commands used:** ls, cat
- **What I learned:** I learned how the ls command shows the files in the current directory by default, and how the cat command can be used to print the outputs of a specified file
- **Where I got stuck:** I was unsure of the syntax for the ls command


### Level 1 to 2
- **Goal:** Read the file called "-"
- **Commands used:** ls, cat
- **What I learned:** cat treats - as “read from the keyboard”, not as a file name. Writing ./- gives the file’s path, so cat reads the file.
- **Where I got stuck:** I was trying to enter the command "cat -" and left with a blank response. Research was needed to figure out how to indicate that I'm searching for a filename.


