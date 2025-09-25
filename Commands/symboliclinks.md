# Commands

## linking files
This challenge required creating a symbolic link to "trick" a program into reading the flag. The program /challenge/catflag was hardcoded to read a specific file, so a symlink was used to redirect it.

### Solve
**Flag:** `pwn.college{kFZSL3S8ELVBbLmF6EeXyxrN05w.QX5ETN1wCO5EzNzEzW}`
The ln -s command was used to create a symbolic link named /home/hacker/not-the-flag that pointed to the actual flag file, /flag. The existing file with the same name was removed first to prevent an error. Running the /challenge/catflag program then followed the link and printed the flag.

```bash
rm /home/hacker/not-the-flag
ln -s /flag /home/hacker/not-the-flag
/challenge/catflag
```

### New Learnings
Symbolic links, or symlinks, are shortcuts to files or directories. They point to the location of the original file, much like a shortcut on a desktop.

The `ln -s` command creates a symbolic link. Its syntax is `ln -s <target> <link_name>`, where target is the original file and link_name is the new shortcut.

Hard links are a different type of link that directly reference the original data. They're like giving a file a second name. They are less common than symlinks and have some limitations, such as not being able to link across filesystems.
### References 

