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
|ls|lists files in a specified directory, current directory if unspecified|
|cat|displays contents of a file into the terminal|cat readme|

## Level notes

### Level 0 to 1
- **Goal:** Locate and print the output of a readme file 
- **Commands used:** ls, cat
- **What I learned:** I learned how the ls command shows the files in the current directory by default, and how the cat command can be used to print the outputs of a specified file
- **Where I got stuck:** I was unsure of the syntax for the ls command

Password found: 6y2kwnwK6grgvwvpvLaa2T1cpFEKOhNR

### Level 1 to 2
- **Goal:** Read the file called "-"
- **Commands used:** ls, cat
- **What I learned:** Files named "-" cant be directly read from the terminal as when the - character is used, cat waits for the user to type into the terminal rather than it look for a file. The fix is to input ./ before the character, this tells the OS that it needs to look for a filename.
- **Where I got stuck:** I was trying to enter the command "cat -" and left with a blank response. Research was needed to figure out how to indicate that im searching for a filename.

Password found: PK8fYLZg2hnHSz83plBL1iEPKdD3QToB

