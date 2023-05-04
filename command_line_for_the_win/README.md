      ### command_line_for_the_win ###
Level 1 : print "hello world"
  ✔ echo "hello world" 
Level 2 : Print the current working directory.
  ✔ pwd
Level 3 : List names of all the files in the current directory, one file per line.
  ✔ ls
Level 4 : There is a file named access.log in the current directory. Print the contents.
  ✔ cat access.log
Level 5 : Print the last 5 lines of "access.log".
  ✔ cat access.log | tail -5   
Level 6 : Create an empty file named take-the-command-challenge in the current working directory.
  ✔ touch take-the-command-challenge  
Level 7 : Create a directory named tmp/files in the current working directory
      Hint: The directory "tmp/" doesn't exist, with one command you need to create both "tmp/" and "tmp/files"
  ✔ mkdir tmp ; cd tmp ; mkdir files 
Level 8 : Copy the file named take-the-command-challenge to the directory tmp/files
  ✔ cp take-the-command-challenge tmp/files  
Level 9 : Move the file named take-the-command-challenge to the directory tmp/files
  ✔ mv take-the-command-challenge tmp/files  
Level 10 : A symbolic link is a type of file that is a reference to another file.
   Create a symbolic link named take-the-command-challenge that points to the file tmp/files/take-the-command-challenge.
  ✔ ln -s tmp/files/take-the-command-challenge take-the-command-challenge  
Level 11 : Delete all of the files in this challenge directory including all subdirectories and their contents.
      Hint: There are files and directories that start with a dot ".", "rm -rf *" won't work here!
  ✔ rm -r * .*  
Level 12 : There are files in this challenge with different file extensions. Remove all files with the .doc extension recursively in the current working directory.
  ✔ rm **/*.doc  
Level 13 : There is a file named access.log in the current working directory. Print all lines in this file that contains the string "GET".
  ✔ cat access.log | grep -e "GET"   
Level 14 : Print all files in the current directory, one per line (not the path, just the filename) that contain the string "500".
  ✔ ls | grep -lR 500  
Level 15 : Print the relative file paths, one path per line for all filenames that start with "access.log" in the current directory.
  ✔ ls -r access.log*  
Level 16 : Print all matching lines (without the filename or the file path) in all files under the current directory that start with "access.log" that contain the string "500". Note that there are no files named access.log in the current directory, you will need to search recursively.
  ✔ ls | grep -rh 500  
Level 17 : Extract all IP addresses from files that start with "access.log" printing one IP address per line.
  ✔ grep -ro ^[0-9.]*  
  
  
