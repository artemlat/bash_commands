# Linux terminal (GitBash) commands
*Here I learned to use basic Linux terminal commands. I made some tasks to improve my practice skills. There are some of them:*
### 1. Check where I am: `pwd`
### 2. Create a folder: `mkdir linux_terminal`
### 3. Go to the created folder: `cd linux_terminal`
### 4. Make 3 new folders: mkdir `folder_1 folder_2 folder_3`
### 5. Go to any of these folders: `cd folder_1`
### 6. Create 5 files (3 x .txt, 2 x .json): `touch 1j.json  1t.txt  2j.json  2t.txt  3t.txt`
### 7. Create 3 folders: `mkdir first_folder second_folder third_folder`
### 8. Show folder content list: `ls -la`
### 9. Open some of created txt files: `cat >> 1t.txt`  
*Tip: Using `>>` with `cat` add new lines to the end of the file. Using `>` update information in the file. Using `cat` without any operator open the file.*
### 10. Write anything in this file  
*Input some lines:*  
`111111`  
`222222`  
`333333`  
`Press [Enter]`
### 11. Save and quit: `Ctrl+C`
### 12. Go to the directory located 1 level above: `cd ..`
### 13. Move any 2 files to any folder: `mv folder_1/1t.txt folder_1/1j.json folder_2`  
### 14. Copy any 2 files to any folder: `cp folder_1/2t.txt folder_1/2j.json folder_1/second_folder`
### 15. Find a file by name: `find . -name '2j*'`
### 16. Show file content in real time: `tail -f folder_2/1t.txt`  
*Tip: If we need to check updating of the line e.g. "line1" in the file we can use this command* `tail -f ./folder_2/1t.txt | grep "line1"`
### 17. Show several of the first lines from the text file: `head -n2 folder_2/1t.txt`
### 18. Show several of the last lines from the text file: `tail -n2 folder_2/1t.txt`
### 19. Show content of a large file: `less folder_1/2t.txt`
### 20. Show current date and time: `date`
### 21. Send http request to the server http://162.55.220.72:5005/terminal-hw-request:  
`curl http://162.55.220.72:5005/terminal-hw-request`
### 22. Write a bash script which does the steps # 3-8, # 13:  
`Create a folder "linux_terminal"`    
`vim script.sh`    
`Press [Enter]`  
`Press "i"`  
`#!/bin/bash`  
`cd linux_terminal`  
`mkdir script_folder1 script_folder2 script_folder3`  
`cd script_folder1`  
`touch script_file1.txt script_file2.txt script_file3.txt script_file4.json script_file5.json`  
`mkdir 1scripted 2scripted 3scripted`  
`ls -la`  
`mv /d/linux_terminal/script_folder1/script_file1.txt /d/linux_terminal/script_folder1/script_file5.json /d/linux_terminal/script_folder2`




