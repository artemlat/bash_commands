# #1 Linux terminal (GitBash) commands
*Here I learned to use basic Linux terminal commands. I made some tasks to improve my practice skills. There are some of them:*
### 1. Check where I am:
```
artem@DESKTOP-4FHC137 MINGW64 /d/qa/34_group
$ pwd
/d/qa/34_group
```
### 2. Create a folder: 
```
artem@DESKTOP-4FHC137 MINGW64 /d/qa/34_group
$ mkdir linux_terminal
```
### 3. Go to the created folder: 
```
artem@DESKTOP-4FHC137 MINGW64 /d/qa/34_group
$ cd linux_terminal
```
### 4. Make 3 new folders:
```
artem@DESKTOP-4FHC137 MINGW64 /d/qa/34_group/linux_terminal
$ mkdir folder_1 folder_2 folder_3
```
### 5. Go to any of these folders:
```
artem@DESKTOP-4FHC137 MINGW64 /d/qa/34_group/linux_terminal
$ cd folder_1
```
### 6. Create 5 files (3 x .txt, 2 x .json):
```
artem@DESKTOP-4FHC137 MINGW64 /d/qa/34_group/linux_terminal/folder_1
$ touch 1j.json  1t.txt  2j.json  2t.txt  3t.txt
```

### 7. Create 3 folders:
```
artem@DESKTOP-4FHC137 MINGW64 /d/qa/34_group/linux_terminal/folder_1
$ mkdir first_folder second_folder third_folder
```

### 8. Show folder content list:
```
artem@DESKTOP-4FHC137 MINGW64 /d/qa/34_group/linux_terminal/folder_1
$ ls -la
total 4
drwxr-xr-x 1 artem 197609 0 Apr 28 19:50 ./
drwxr-xr-x 1 artem 197609 0 Apr 28 19:47 ../
-rw-r--r-- 1 artem 197609 0 Apr 28 19:50 1j.json
-rw-r--r-- 1 artem 197609 0 Apr 28 19:50 1t.txt
-rw-r--r-- 1 artem 197609 0 Apr 28 19:50 2j.json
-rw-r--r-- 1 artem 197609 0 Apr 28 19:50 2t.txt
-rw-r--r-- 1 artem 197609 0 Apr 28 19:50 3t.txt
drwxr-xr-x 1 artem 197609 0 Apr 28 19:50 first_folder/
drwxr-xr-x 1 artem 197609 0 Apr 28 19:50 second_folder/
drwxr-xr-x 1 artem 197609 0 Apr 28 19:50 third_folder/
```
### 9. Open some of created txt files:
*Tip: Using `>>` with `cat` add new lines to the end of the file. Using `>` update information in the file. Using `cat` without any operator open the file.*
```
cat >> 1t.txt
```

### 10. Write anything in this file  
*Input some lines:* 
```
111111  
222222 
333333
```
*Press `Enter`*

### 11. Save and quit: 
*Press `Ctrl+C`*

### 12. Go to the directory located 1 level above:
```
artem@DESKTOP-4FHC137 MINGW64 /d/qa/34_group/linux_terminal/folder_1
$ cd ..
```

### 13. Move any 2 files to any folder:
```
artem@DESKTOP-4FHC137 MINGW64 /d/qa/34_group/linux_terminal
$ mv folder_1/{1t.txt,1j.json} folder_2
```
### 14. Copy any 2 files to any folder:
```
artem@DESKTOP-4FHC137 MINGW64 /d/qa/34_group/linux_terminal
$ cp folder_1/2t.txt folder_1/2j.json folder_1/second_folder
```

### 15. Find a file by name:
```
artem@DESKTOP-4FHC137 MINGW64 /d/qa/34_group/linux_terminal
$ find . -name '2j.json'
./folder_1/2j.json
./folder_1/second_folder/2j.json
```

### 16. Show file content in real time: 
*Tip: If we need to check updating of the line e.g. "line1" in the file we can use this command*   
`tail -f ./folder_2/1t.txt | grep "line1"`

```
artem@DESKTOP-4FHC137 MINGW64 /d/qa/34_group/linux_terminal
$ tail -f folder_2/1t.txt
111111
222222
333333
444444
```
*Press `Ctrl+C` to quit the file*

### 17. Show several of the first lines from the text file: 
```
artem@DESKTOP-4FHC137 MINGW64 /d/qa/34_group/linux_terminal
$ head -n2 folder_2/1t.txt
111111
222222
```
### 18. Show several of the last lines from the text file:
```
artem@DESKTOP-4FHC137 MINGW64 /d/qa/34_group/linux_terminal
$ tail -n2 folder_2/1t.txt
333333
444444
```

### 19. Show content of a large file: 
*Add large text to the file 2t.txt*
```
less folder_1/2t.txt
```
```
Древность

Устная передача — самый древний способ передачи знаний в истории человечества. После изобретения древними цивилизациями систем записи люди начали использовать для письма почти всё, на чём можно писать — глиняные таблички, кору дерева, листы металла и т. п.
Таблички
Шумерская глиняная табличка с клинописью

Табличку можно определить как физически прочный, надёжный носитель письменной информации, относительно удобный в повседневном использовании и транспортировке. Пишущим средством в этом случае, как правило, выступало стило. Можно выделить два основных типа табличек: глиняные (например, у населения долины между Тигром и Евфратом), которые часто использовались для письма клинописью[4], и восковые. Последние представляли собой дощечки, покрытые слоем воска, в то время как глиняные полностью состояли из глины и после нанесения надписей часто обжигались для придания им дополнительной прочности. После этой процедуры, соответственно, изменить текст было уже невозможно; напротив, записи на восковых табличках можно было стереть и использовать носитель повторно. В Древнем Риме дощечки часто скрепляли друг с другом. Известно, что существовали «диптихи», «триптихи» и «полиптихи» (соответственно две, три и много дощечек)[5], образуя тем самым своеобразный прототип современной книги — кодекс[6].
Свитки
folder_1/2t.txt
```

*Press `q` to quit the file*
### 20. Show current date and time: 
```
artem@DESKTOP-4FHC137 MINGW64 /d/qa/34_group/linux_terminal
$ date
Fri Apr 28 20:39:48     2023
```
### 21. Send http request to the server http://162.55.220.72:5005/terminal-hw-request:  
```
artem@DESKTOP-4FHC137 MINGW64 /d/qa/34_group/linux_terminal
$ curl http://162.55.220.72:5005/terminal-hw-request
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:--  0:00:02 --:--:--     0
curl: (7) Failed to connect to 162.55.220.72 port 5005 after 2212 ms: Connection refused
```

### 22. Write a bash script which does the steps # 3-8, # 13:  
*Create a folder "linux_terminal" and enter it. Then open bash console:*    
```
vim script.sh
```
*Press `Enter`*  
*Press `INS`* 
```
#!/bin/bash 
cd linux_terminal  
mkdir script_folder1 script_folder2 script_folder3 
cd script_folder1  
touch script_file1.txt script_file2.txt script_file3.txt script_file4.json script_file5.json 
mkdir 1scripted 2scripted 3scripted  
ls -la  
mv /d/linux_terminal/script_folder1/script_file1.txt /d/linux_terminal/script_folder1/script_file5.json /d/linux_terminal/script_folder2
```
*Press `Enter`*  
*Press `ESC`*  
*Input `:wq`*  
*Press `Enter`*  
*To run the script:*
```
artem@DESKTOP-4FHC137 MINGW64 /d
$ bash script.sh
total 4
drwxr-xr-x 1 artem 197609 0 Apr 28 20:51 .
drwxr-xr-x 1 artem 197609 0 Apr 28 20:51 ..
drwxr-xr-x 1 artem 197609 0 Apr 28 20:51 1scripted
drwxr-xr-x 1 artem 197609 0 Apr 28 20:51 2scripted
drwxr-xr-x 1 artem 197609 0 Apr 28 20:51 3scripted
-rw-r--r-- 1 artem 197609 0 Apr 28 20:51 script_file1.txt
-rw-r--r-- 1 artem 197609 0 Apr 28 20:51 script_file2.txt
-rw-r--r-- 1 artem 197609 0 Apr 28 20:51 script_file3.txt
-rw-r--r-- 1 artem 197609 0 Apr 28 20:51 script_file4.json
-rw-r--r-- 1 artem 197609 0 Apr 28 20:51 script_file5.json
```

