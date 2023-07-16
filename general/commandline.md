# [Home](../README.md)

### Create Commandline Script
1. Create **test.sh** file
2. Make sh file executable `chmod +x test.sh`
3. run file `./test.sh`

### Read
```sh
# Display content 
cat [filename]

# Merge content 
cat info.txt info2.txt > mergedinfo.text
```

### Copy
```sh
# Duplicate file
cp myfile.txt myfile2.txt

# Copy file to folder
cp /home/hostinger/myfile.txt /home/etc/

# Copy folder recursively 
cp -R /home/hostinger/myfolder /home/etc/
``` 

### Move
Move file or folder 
```sh
mv [source] [destination]
```

### Find Content
```sh
# Find word in file
grep 'line' info.txt

# Find files ending with .zip
ls -l | grep .zip
```

### tar
```sh
# Create tar
tar -czvf file.tar.gz /directory_to_tar

# Unpack tar 
tar -xzvf file.tar.gz -C /target_dir/
```

### zip
Install `sudo apt install unzip` `sudo apt-get install zip`
```sh
# zip 
zip -r file.zip folder1 folder2

# unzip 
unzip sampleZipFile.zip

# unzip multiple 
unzip *.zip
```

### Get file size
```sh
# List all files with information
ls -h -l
```

### chmod
```sh
# Alle rechte rekursiv 
chmod -R 777 foldername

# Read only rekursiv
chmod -R a=r foldername
```

### pipe
```sh
# Pipe output to next command 
command with result | command expecting input
```