# ORCA Installation Steps
First, we need to download ORCA source file from [ORCA offical page](https://orcaforum.kofo.mpg.de/app.php/portal). For HPC with command line interface, we can use [lynx](https://en.wikipedia.org/wiki/Lynx_(web_browser)) to download the source files.

First we make a directory dedicated to ORCA.
```shell
mkdir orca
```
Then, we install lynx
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
After download ORCA_Linux_Part_1,2,3 , then use tar -xvf to extract
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
Transfer all file from extracted tar-xvf directory to orca directory
```shell
mv /home/m_2554324/orca_5_0_4_linux_x86-64_openmpi411_part1/* /home/m_2554324/orca
```
```shell
mv /home/m_2554324/orca_5_0_4_linux_x86-64_openmpi411_part2/* /home/m_2554324/orca
```
```shell
mv /home/m_2554324/orca_5_0_4_linux_x86-64_openmpi411_part3/* /home/m_2554324/orca
```
