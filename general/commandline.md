# [Home](../README.md)

### Create Commandline Script
1. Create **test.sh** file
2. Make sh file executable `chmod +x test.sh`
3. run file `./test.sh`

### Read
- Display content `cat [filename]`
- Merge content `cat info.txt info2.txt > mergedinfo.text`

### Copy
- duplicate file `cp myfile.txt myfile2.txt`
- copy file to folder `cp /home/hostinger/myfile.txt /home/etc/`
- copy folder recursively `cp -R /home/hostinger/myfolder /home/etc/` 

### Move
- Move file or folder `mv [source] [destination]`

### Find Content
- Find word in file `grep 'line' info.txt`
- Find files ending with .zip `ls -l | grep .zip`

### tar
- create tar `tar -czvf file.tar.gz /directory_to_tar`
- unpack tar `tar -xzvf file.tar.gz -C /target_dir/`

### zip
- install `sudo apt install unzip` `sudo apt-get install zip`
- zip `zip -r file.zip folder1 folder2` 
- unzip `unzip sampleZipFile.zip`
- unzip multiple `unzip *.zip`s

### Get file size
- `ls -l`

### chmod
- alle rechte rekursiv `chmod -R 777 foldername`
- read only rekursiv `chmod -R a=r foldername`

### pipe
- pipe output to next command `command with result | command expecting input`