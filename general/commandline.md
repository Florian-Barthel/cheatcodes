# [Home](../README.md)

### Create Commandline Script
1. Create **test.sh** file
2. Make sh file executable `chmod +x test.sh`
3. run file `./test.sh`

### Read
Display content 
```sh
 cat [filename]
 ```
Merge content 
```sh
cat info.txt info2.txt > mergedinfo.text
```

### Copy
Duplicate file
```sh
cp myfile.txt myfile2.txt
```
Copy file to folder
```sh
cp /home/hostinger/myfile.txt /home/etc/
```
Copy folder recursively 
```sh
cp -R /home/hostinger/myfolder /home/etc/
``` 

### Move
Move file or folder 
```sh
mv [source] [destination]
```

### Find Content
Find word in file
```sh
grep 'line' info.txt
```
Find files ending with .zip
```sh
ls -l | grep .zip
```

### tar
Create tar
```sh
tar -czvf file.tar.gz /directory_to_tar
```

Unpack tar 
```sh
tar -xzvf file.tar.gz -C /target_dir/
```

### zip
Install `sudo apt install unzip` `sudo apt-get install zip`
zip 
```sh
zip -r file.zip folder1 folder2
```

unzip 
```sh
unzip sampleZipFile.zip
```
unzip multiple 
```sh
unzip *.zip
```

### Get file size
List all files with information
```sh
ls -l
```

### chmod
Alle rechte rekursiv 
```sh
chmod -R 777 foldername
```
Read only rekursiv
```sh
chmod -R a=r foldername
```

### pipe
Pipe output to next command 
```sh
command with result | command expecting input
```