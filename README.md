# ORCA Installation Steps
First, we need to download ORCA source file from [ORCA offical page](https://orcaforum.kofo.mpg.de/app.php/portal). For HPC with command line interface, we can use [lynx](https://en.wikipedia.org/wiki/Lynx_(web_browser)) to download the ORCA source file.

First, we install lynx
```shell
sudo apt update
```
```shell
sudo apt install lynx
```
```shell
lynx "https://orcaforum.kofo.mpg.de/app.php/dlext/?view=detail&df_id=190"
```

## Step 1
After download ORCA_Linux_Part_1,2,3 then use tar -xvf to extract
```shell
tar -xvf '*=UTF-8--orca_5_0_4_linux_x86-64_openmpi411_part1.tar.xz'
```
```shell
tar -xvf '*=UTF-8--orca_5_0_4_linux_x86-64_openmpi411_part2.tar.xz'
```
```shell
tar -xvf '*=UTF-8--orca_5_0_4_linux_x86-64_openmpi411_part3.tar.xz'
```

## Step 2
Create a directory dedicated to ORCA, such as `orca`.
```shell
mkdir orca
```

Transfer ORCA_Linux_Part_1,2,3 files from the extracted tar -xvf directory to `orca` directory just created.
```shell
mv /home/directory1/orca_5_0_4_linux_x86-64_openmpi411_part1/* /home/directory1/orca
```
```shell
mv /home/directory1/orca_5_0_4_linux_x86-64_openmpi411_part2/* /homedirectory1/orca
```
```shell
mv /home/directory1/orca_5_0_4_linux_x86-64_openmpi411_part3/* /home/directory1/orca
```

## Step 3
Add the correct `orca` running path in the `bashrc` file.
```shell
nano .bashrc
```

Note: Add the following line at the end of `bashrc` file
```shell
alias orca='/home/directory1/orca/orca'
```

Source the `bashrc` file to allow the changes take place.
```shell
source .bashrc
```

## Step 4
Download open-mpi shared library
```shell
sudo apt install libopenmpi-dev
```

## Run ORCA !
Hooray! ORCA is installed and setup correctly. Now, try to do test run.
```shell
orca $INPUT
```
