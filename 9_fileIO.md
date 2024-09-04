# File Input and Output

## Problem 1: writing and appending
Write a program that allows the user to enter any number of lines of text, and writes these lines to a file as they are entered. The user enters an empty string when finished. Here's an example terminal output

```
enter text: Dear diary,
enter text: COMP 1701 is my favorite class
enter text:
2 lines of text written to H:\1701\fileIO.txt
```

Now modify your program as follows:
- Alter your program so it does not overwrite the file(s) each time it runs. That is, each run of the program will append additional lines of text to the file(s).
- The program should insert some blank lines betwteen the text from different runs, to clearly seperate the text entries from different sessions. However, there should be no blank lines at the *beginning* or *end* of the file - only between entries. You will need to research some ways of doing this. Remember to cite your sources.

## Problem 2: reading and analyzing text
Download the file [import this.txt](/img/import_this.txt). Write a program that reads the file and reports the following:

- Total number of lines
- Total number of words
- Total number of words *not including* any words on the list of "stopwords" contained in [this file](/img/stopwords.txt) (your program should read that file too, to get the list of stopwords)

## Problem 3: transferring data from one file to another
Suppose your company stores its customers' usernames and passwords in [this file](/img/username_passwords.txt). You realize storing credentials in plain text may be a bad idea, so you decide to beef up security. 

- step 1: Write a program that reads the usernames and passwords from the original file, and creates a new file called `hashed.txt` containing the usernames with their *hashed* passwords. Hashing is a process that converts a value or string into another value - in this case, converting the password into an unintelligible series of digits. In Python, you can get a hash value for a string like this: `my_string.__hash__()`. 
   - Note you will also need to use the [.split()](https://www.w3schools.com/python/ref_string_split.asp) string method to separate usernames from passwords in the original file (what should you use as a separator?)
- step 2: Write a small, separate program that prompts the user for a username and password, and authenticates them by checking the hash of the entered password matches that user's hash in `hashed.txt`
- step 3: Now modify your original program so that it only writes usernames and hashes to `hashed.txt` if the password is at least 8 characters long. Otherwise the username/password combo is written to another file called `invalid_passwords.txt`
