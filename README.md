# Lab-4
summarize about shell commands

## Shell commands
### meaning
**Shell**: Interface that allows users to communicate with (\*)kernel/ Users runs applications and give commands throgh shell
\* kernel: Core of OS that cntrols and communicates with hardware resource  

### languages  
**\*pwd**: shows the current path in a hierarchical directory  
**\*cd**: change directory
**\*ls**: list files and directories
 *arguments*
  1. '/': root
  2. '.': current directory
  3. '..': upper-level directory
  4. '~': home of current user
  5. '/[directory name]': absolute path
  6. './[directory name]':relative path
  7. '../[directory name]': relative path
  
  *options*
  1. '-l': show detailed information(long format)
  2. '-lh': show detaield information(size in units)
  
  *methods for using (possible to mix two or more)*
  1. 'ls': list the files in the working
  2. 'ls/bin': list the files in the '/bin(directory name)' directory (or any other directory we care to specify)
  3. 'ls -l': listh the files in the working directory in long format
  4. 'ls -l /etc /bin': list the files in the '/bing' directory and the '/etc' directory in long format (show information about bin&etc in long format)
  5. 'ls -la ..': list all files in the parent of the working directory in long format 

**\*clear**
 input "clear" -> delete files and directories
 *Warnings: Make sure to backup important contents*
 
 **\*cp**
  : copy files and directories
 1. cp file1 file2: copies the contents of file1 into file2 (if file2 does not exist, it is created)
 2. cp -i file1 file2: like above however, since the "-i"(interactive) opton is specified
 3. cp file1 dir1: copy the contents of file1 inside of directory dir1
 4. cp -R dir1 dir2: copy the contents of the directory dir1 (if directory dir2 does not exist, it is created)
 
**\*mv**
  : move files and directories or rename them
  1. mv file1 file2: If file2 does not exist, then file1 is renamed filew
  2. mv -i file1 file2: Like above however, since the "-i"(interactive) option is specified
  3. mv file file2 dir1: the files file1 and file2 are moved to directory dir1
  4. mv dir1 dir2: if dir2 does not exist, then dir1 is renamed dir2.
  
**\*rm**
   : \delete files and directories permantely and irreversevley
   1. rm file1 file2: delete fiel1 and file2
   2. rm -i file1 file2: like above however, since the "-i"(interactive) option is specified
   3. rm -r dir1 dir2: directions dir1 and dir2 are deleted along with all of their contents
   
**\*mkdir**
    : make a new directory
    
**\*Wildcards**
  : specify multiple files at once
  1. *: all filenames
  2. g*: all filenames that begin with the character "g"
  3. b*.txt: all filenames that begin with the character "b" and end with the characters ".txt"
  4. Data???: any filenme that begns with the characters "Data" followed by exactly 3 more characters
  5. cp *.txt text_files: copy all files in the current working directory with names ending with the characters ".txt" to an existing director named text_files
  6. mv dir1 ../*bak dir2: move the subdirectory dir1 and all the fiels ending in ".bak" in the current working directory's parent directoy to an existing directory named dir2.
  7. rm *~: delete all files in the current working directory that end with the character "~".
  
**\*man**
: help command

**\*exit**
: exiting terminal
 

***Tip***
   1. autocompletion 
      ex) neuralintlab : n -> press "tab" key -> neuralintlab
                         if, 'neauralintlab' and 'nauralintlab' present in one folder: ne -> press "tab" key -> neuralintlab
                         
   2. past commands
      : press "up arrow" key -> show past commands($ ls ~)
