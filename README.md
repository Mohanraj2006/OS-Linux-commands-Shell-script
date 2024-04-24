# OS-Linux-commands-Shell-scripting
Operating systems Lab exercise
# Linux commands-Shell scripting
Linux commands-Shell scripting

# AIM:
To practice Linux Commands and Shell Scripting

# DESIGN STEPS:

### Step 1:

Navigate to any Linux environment installed on the system or installed inside a virtual environment like virtual box/vmware or online linux JSLinux (https://bellard.org/jslinux/vm.html?url=alpine-x86.cfg&mem=192) or docker.

### Step 2:

Execute the following commands

### Step 3:

Testing the commands for the desired output. 

# COMMANDS:
### Create the following files file1, file2 as follows:
cat > file1
```
chanchal singhvi
c.k. shukla
s.n. dasgupta
sumit chakrobarty
^d
```
![s1](https://github.com/Mohanraj2006/OS-Linux-commands-Shell-script/assets/152195759/34526ad5-3634-4a1a-b9eb-15445c2a2958)

cat > file2
```
anil aggarwal
barun sengupta
c.k. shukla
lalit chowdury
s.n. dasgupta
^d
```

![s2](https://github.com/Mohanraj2006/OS-Linux-commands-Shell-script/assets/152195759/967217d2-7987-4fc5-a9ec-1c44a995063f)

### Display the content of the files
cat < file1
## OUTPUT

![s3](https://github.com/Mohanraj2006/OS-Linux-commands-Shell-script/assets/152195759/8a3db055-61fa-4751-b62c-33846c1a922e)


cat < file2
## OUTPUT

![s4](https://github.com/Mohanraj2006/OS-Linux-commands-Shell-script/assets/152195759/b20edecc-9035-4fd4-aaf3-d89beb186b87)

# Comparing Files
cmp file1 file2
## OUTPUT
 
 ![s5](https://github.com/Mohanraj2006/OS-Linux-commands-Shell-script/assets/152195759/ac4faabf-3cdd-403b-81f5-1508010df70e)

comm file1 file2
 ## OUTPUT

 ![s6](https://github.com/Mohanraj2006/OS-Linux-commands-Shell-script/assets/152195759/fb13a598-97b1-4a1c-9c3f-3f32e4f34134)

diff file1 file2
## OUTPUT

![s7](https://github.com/Mohanraj2006/OS-Linux-commands-Shell-script/assets/152195759/9c1a0f8d-838d-41b4-aa10-bf849795db0a)

#Filters

### Create the following files file11, file22 as follows:

cat > file11
```
Hello world
This is my world
^d
```
![s8](https://github.com/Mohanraj2006/OS-Linux-commands-Shell-script/assets/152195759/c7dfb6da-73bd-4af6-bd11-2177901d5bcd)

cat > file22
```
1001 | Ram | 10000 | HR
1002 | tom |  5000 | Admin
1003 | Joe |  7000 | Developer
^d
```

![s9](https://github.com/Mohanraj2006/OS-Linux-commands-Shell-script/assets/152195759/18709008-75a1-4596-827f-b0d3f18be189)

cut -c1-3 file11
## OUTPUT

![s10](https://github.com/Mohanraj2006/OS-Linux-commands-Shell-script/assets/152195759/ce42ea13-a4f3-4200-a6e1-0ccc7cf77ab3)

cut -d "|" -f 1 file22
## OUTPUT

![s11](https://github.com/Mohanraj2006/OS-Linux-commands-Shell-script/assets/152195759/fda638c7-b9cc-4f83-ad5d-9b6ba57cc7e5)


cut -d "|" -f 2 file22
## OUTPUT

![s12](https://github.com/Mohanraj2006/OS-Linux-commands-Shell-script/assets/152195759/8692bf3f-948c-471b-a59f-54a89159d291)

cat < newfile 
```
Hello world
hello world
^d
````
![s13](https://github.com/Mohanraj2006/OS-Linux-commands-Shell-script/assets/152195759/d0fb4349-528a-49f8-9b9a-e93a2552129f)

cat > newfile 
Hello world
hello world

 ![s14](https://github.com/Mohanraj2006/OS-Linux-commands-Shell-script/assets/152195759/f9642bfd-59be-4792-b65a-9bed1c3e3c7c)

grep Hello newfile 
## OUTPUT

![s15](https://github.com/Mohanraj2006/OS-Linux-commands-Shell-script/assets/152195759/190c2e24-3656-409e-823c-5770b2772cee)


grep hello newfile 
## OUTPUT
grep -v hello newfile 

![s16](https://github.com/Mohanraj2006/OS-Linux-commands-Shell-script/assets/152195759/5b49ad0a-027e-473c-8be6-41d2ba040d38)


## OUTPUT
cat newfile | grep -i "hello"

![s17](https://github.com/Mohanraj2006/OS-Linux-commands-Shell-script/assets/152195759/8d93a070-1417-4057-a634-169e66afc8b3)


## OUTPUT
cat newfile | grep -i -c "hello"

![s18](https://github.com/Mohanraj2006/OS-Linux-commands-Shell-script/assets/152195759/842e4c38-1f44-4b78-ac40-28a5949c5b03)

## OUTPUT


![s19](https://github.com/Mohanraj2006/OS-Linux-commands-Shell-script/assets/152195759/32665990-0b6a-426d-9fc5-d347a1c8190b)


grep -R ubuntu /etc
## OUTPUT

![s20](https://github.com/Mohanraj2006/OS-Linux-commands-Shell-script/assets/152195759/810860fd-2352-4920-b66a-b50e7ed8cc45)


grep -w -n world newfile   
## OUTPUT


cat < newfile 
```
Hello world
hello world
Linux is world number 1
Unix is predecessor
Linux is best in this World
^d
```
![s21](https://github.com/Mohanraj2006/OS-Linux-commands-Shell-script/assets/152195759/43fda45c-690d-4906-b295-0cdefb3333a1)


cat > newfile
```
Hello world
hello world
Linux is world number 1
Unix is predecessor
Linux is best in this World
^d
 ```

![s22](https://github.com/Mohanraj2006/OS-Linux-commands-Shell-script/assets/152195759/81a69ed1-30f7-4170-83cb-d23646d68b63)


egrep -w 'Hello|hello' newfile 
## OUTPUT

![s23](https://github.com/Mohanraj2006/OS-Linux-commands-Shell-script/assets/152195759/66cf3c2e-0828-4ea9-ac05-3026e584fb2f)


egrep -w '(H|h)ello' newfile 
## OUTPUT

![s24](https://github.com/Mohanraj2006/OS-Linux-commands-Shell-script/assets/152195759/47b87ad3-d606-4c2e-99fb-9e725cdfa242)


egrep -w '(H|h)ell[a-z]' newfile 
## OUTPUT

![s26](https://github.com/Mohanraj2006/OS-Linux-commands-Shell-script/assets/152195759/459ad898-177b-4086-b6c0-f521bf4594df)



egrep '(^hello)' newfile 
## OUTPUT

![s27](https://github.com/Mohanraj2006/OS-Linux-commands-Shell-script/assets/152195759/a24fbd2d-84b5-41f8-8a72-27bb0b9141c8)


egrep '(world$)' newfile 
## OUTPUT

![s28](https://github.com/Mohanraj2006/OS-Linux-commands-Shell-script/assets/152195759/96da7aef-cae2-4492-ba7e-d8107c53592f)


egrep '(World$)' newfile 
## OUTPUT

![s29](https://github.com/Mohanraj2006/OS-Linux-commands-Shell-script/assets/152195759/d6a20110-8c79-4d79-92cb-2bf2570ae741)

egrep '((W|w)orld$)' newfile 
## OUTPUT

![s30](https://github.com/Mohanraj2006/OS-Linux-commands-Shell-script/assets/152195759/8d44c99c-cd98-48e4-bfbc-4e9194ead99d)


egrep '[1-9]' newfile 
## OUTPUT



egrep 'Linux.*world' newfile 
## OUTPUT


egrep 'Linux.*World' newfile 
## OUTPUT

![s31](https://github.com/Mohanraj2006/OS-Linux-commands-Shell-script/assets/152195759/79ae8a42-7f89-4c36-b3a2-b61621098e6d)

egrep l{2} newfile
## OUTPUT

![s32](https://github.com/Mohanraj2006/OS-Linux-commands-Shell-script/assets/152195759/7c8892f1-3c41-46d6-95a4-d0c90efcaf16)


egrep 's{1,2}' newfile
## OUTPUT 


cat > file23
```
1001 | Ram | 10000 | HR
1001 | Ram | 10000 | HR
1002 | tom |  5000 | Admin
1003 | Joe |  7000 | Developer
1005 | Sam |  5000 | HR
1004 | Sit |  7000 | Dev
1003 | Joe |  7000 | Developer
1001 | Ram | 10000 | HR
^d
```

![s33](https://github.com/Mohanraj2006/OS-Linux-commands-Shell-script/assets/152195759/292b0270-59b3-4774-8b12-52e74951b71a)


sed -n -e '3p' file23

![s34](https://github.com/Mohanraj2006/OS-Linux-commands-Shell-script/assets/152195759/473c0bce-a536-4051-8adc-2813f1b6c8e9)

## OUTPUT

![s35](https://github.com/Mohanraj2006/OS-Linux-commands-Shell-script/assets/152195759/ddcba002-e5a3-42fe-8e22-ca92196d0780)


sed -n -e '$p' file23
## OUTPUT

![s36](https://github.com/Mohanraj2006/OS-Linux-commands-Shell-script/assets/152195759/25f46729-86e4-43bd-bd69-a347cb64be6d)


sed  -e 's/Ram/Sita/' file23
## OUTPUT

![s37](https://github.com/Mohanraj2006/OS-Linux-commands-Shell-script/assets/152195759/e1ad1fbc-5b7b-4ca8-8294-569a0c00780c)


sed  -e '2s/Ram/Sita/' file23
## OUTPUT

![s38](https://github.com/Mohanraj2006/OS-Linux-commands-Shell-script/assets/152195759/82dc5df8-ca7b-4529-90e3-54a14610bda5)


sed  '/tom/s/5000/6000/' file23
## OUTPUT

![s39](https://github.com/Mohanraj2006/OS-Linux-commands-Shell-script/assets/152195759/b766e4b5-ec15-453e-bebf-8ebc5b0694f4)


sed -n -e '1,5p' file23
## OUTPUT


![s40](https://github.com/Mohanraj2006/OS-Linux-commands-Shell-script/assets/152195759/fa1ee142-b25d-4870-824d-f19cb67541d2)

sed -n -e '2,/Joe/p' file23
## OUTPUT

![s41](https://github.com/Mohanraj2006/OS-Linux-commands-Shell-script/assets/152195759/e21fe06d-6be4-4b5a-a06c-f41261b45792)



sed -n -e '/tom/,/Joe/p' file23
## OUTPUT

![s42](https://github.com/Mohanraj2006/OS-Linux-commands-Shell-script/assets/152195759/cae7b3e7-7cea-4bd5-b605-d87a81fc4927)


seq 10 
## OUTPUT

![s43](https://github.com/Mohanraj2006/OS-Linux-commands-Shell-script/assets/152195759/fa78bdff-acb8-49e7-ae1e-aee97daa38cb)


seq 10 | sed -n '4,6p'
## OUTPUT

![s44](https://github.com/Mohanraj2006/OS-Linux-commands-Shell-script/assets/152195759/15ce1cf2-1755-447a-b351-541342c27154)


seq 10 | sed -n '2,~4p'
## OUTPUT

![s45](https://github.com/Mohanraj2006/OS-Linux-commands-Shell-script/assets/152195759/378880ad-bebb-4aae-a722-86fd5fd58053)


seq 3 | sed '2a hello'
## OUTPUT

![s46](https://github.com/Mohanraj2006/OS-Linux-commands-Shell-script/assets/152195759/e982993f-1d80-47dc-a7a7-a39ae4782769)


seq 2 | sed '2i hello'
## OUTPUT

![s47](https://github.com/Mohanraj2006/OS-Linux-commands-Shell-script/assets/152195759/e1b47dc2-0c74-4b93-983d-184d22a9322b)

seq 10 | sed '2,9c hello'
## OUTPUT

![s48](https://github.com/Mohanraj2006/OS-Linux-commands-Shell-script/assets/152195759/50e77941-f804-4060-932f-f0deba56e779)

sed -n '2,4{s/^/$/;p}' file23
## OUTPUT

![s49](https://github.com/Mohanraj2006/OS-Linux-commands-Shell-script/assets/152195759/a8b39126-7d80-4240-ba76-df77fad8733d)


sed -n '2,4{s/$/*/;p}' file23


#Sorting File content
cat > file21
```
1001 | Ram | 10000 | HR
1002 | tom |  5000 | Admin
1003 | Joe |  7000 | Developer
1005 | Sam |  5000 | HR
1004 | Sit |  7000 | Dev
``` 
sort file21

![s50](https://github.com/Mohanraj2006/OS-Linux-commands-Shell-script/assets/152195759/6cf61fa7-ac25-40bb-8097-895fc0a499e7)

## OUTPUT


cat > file22
```
1001 | Ram | 10000 | HR
1001 | Ram | 10000 | HR
1002 | tom |  5000 | Admin
1003 | Joe |  7000 | Developer
1005 | Sam |  5000 | HR
1004 | Sit |  7000 | Dev
```

![s51](https://github.com/Mohanraj2006/OS-Linux-commands-Shell-script/assets/152195759/a8afb99d-a98d-4514-9600-1702f6453d46)

uniq file22

![s52](https://github.com/Mohanraj2006/OS-Linux-commands-Shell-script/assets/152195759/02dc7f22-1d08-44e8-8cbc-e93358dd5c0d)


## OUTPUT



#Using tr command

cat file23 | tr [:lower:] [:upper:]
![s53](https://github.com/Mohanraj2006/OS-Linux-commands-Shell-script/assets/152195759/0404d3ae-44f1-4e62-ac51-0d40b7d180b4)


## OUTPUT

cat < urllist.txt
```
www. yahoo. com
www. google. com
www. mrcet.... com
^d
 ```

![s54](https://github.com/Mohanraj2006/OS-Linux-commands-Shell-script/assets/152195759/90a2e0c9-16f2-4e7e-b792-8852e161fd6b)

cat > urllist.txt
```
www. yahoo. com
www. google. com
www. mrcet.... com
 ```

![s55](https://github.com/Mohanraj2006/OS-Linux-commands-Shell-script/assets/152195759/1f370493-97eb-4d78-931b-8b3e5371a2b9)

cat urllist.txt | tr -d ' '

![s56](https://github.com/Mohanraj2006/OS-Linux-commands-Shell-script/assets/152195759/f8cd87d2-e8d3-48d5-b045-b4b4c1c4e208)

 ## OUTPUT


 ![s57](https://github.com/Mohanraj2006/OS-Linux-commands-Shell-script/assets/152195759/1d84b067-f3ee-4974-8db9-c03d3000cedb)

cat urllist.txt | tr -d ' ' | tr -s '.'
## OUTPUT
#Backup commands
tar -cvf backup.tar *

![s58](https://github.com/Mohanraj2006/OS-Linux-commands-Shell-script/assets/152195759/39578207-2bec-477d-8333-fe09d72c5778)

 
## OUTPUT


mkdir backupdir
 
mv backup.tar backupdir

 ![s59](https://github.com/Mohanraj2006/OS-Linux-commands-Shell-script/assets/152195759/58ae0a86-6ec4-4ca4-b4f7-61cf3e4ecfe6)

tar -tvf backup.tar

![s60](https://github.com/Mohanraj2006/OS-Linux-commands-Shell-script/assets/152195759/cac87890-023d-4fd2-a0af-2da24d34f272)

## OUTPUT

![s61](https://github.com/Mohanraj2006/OS-Linux-commands-Shell-script/assets/152195759/1d8a581f-d32f-4811-9730-18649f554953)

tar -xvf backup.tar
## OUTPUT

gzip backup.tar

ls .gz

![s62](https://github.com/Mohanraj2006/OS-Linux-commands-Shell-script/assets/152195759/e66d8ad0-e3c0-4cde-a6f8-f6dc57bce07f)

## OUTPUT
 
gunzip backup.tar.gz

![s63](https://github.com/Mohanraj2006/OS-Linux-commands-Shell-script/assets/152195759/18b711dd-e509-4beb-a0be-84b90feae194)

## OUTPUT

 
# Shell Script
```
echo '#!/bin/sh' > my-script.sh
echo 'echo Hello World‘; exit 0 >> my-script.sh
```

![s64](https://github.com/Mohanraj2006/OS-Linux-commands-Shell-script/assets/152195759/e5afb1e0-1de8-4216-b2c5-6ce22b51da60)

chmod 755 my-script.sh
./my-script.sh

![s65](https://github.com/Mohanraj2006/OS-Linux-commands-Shell-script/assets/152195759/d0ad45a8-5939-41b8-8ced-8eba227f2d97)

## OUTPUT

 
cat << stop > herecheck.txt
```
hello in this world
i cant stop
for this non stop movement
stop
```

![s66](https://github.com/Mohanraj2006/OS-Linux-commands-Shell-script/assets/152195759/00f030ed-0819-4fc5-858f-3a09703abc62)


cat herecheck.txt

![s67](https://github.com/Mohanraj2006/OS-Linux-commands-Shell-script/assets/152195759/47f26053-1822-4b71-ab28-78110fb370d6)

## OUTPUT


cat < scriptest.sh 
```bash
\#!/bin/sh
echo “File name is $0 ”
echo "File name is " `basename $0`
echo “First arg. is ” $1
echo “Second arg. is ” $2
echo “Third arg. is ” $3
echo “Fourth arg. is ” $4
echo 'The $@ is ' $@
echo 'The $\# is ' $1#
echo 'The $$ is ' $$
ps
^d
 ```

![s68](https://github.com/Mohanraj2006/OS-Linux-commands-Shell-script/assets/152195759/8e4ec488-d505-43e5-b760-b9f9b92d8cc1)

cat scriptest.sh 
```bash
\#!/bin/sh
echo “File name is $0 ”
echo "File name is " `basename $0`
echo “First arg. is ” $1
echo “Second arg. is ” $2
echo “Third arg. is ” $3
echo “Fourth arg. is ” $4
echo 'The $@ is ' $@
echo 'The $\# is ' $\#
echo 'The $$ is ' $$
ps
```
 
 ![s69](https://github.com/Mohanraj2006/OS-Linux-commands-Shell-script/assets/152195759/f4931d74-0580-42ba-9c8c-b8a9b2d4a820)

chmod 777 scriptest.sh
 
./scriptest.sh 1 2 3

![s70](https://github.com/Mohanraj2006/OS-Linux-commands-Shell-script/assets/152195759/01f4d50a-933b-4c03-a792-34714a58458a)

## OUTPUT

 
ls file1
 ![s71](https://github.com/Mohanraj2006/OS-Linux-commands-Shell-script/assets/152195759/4e0473d3-e91a-4e74-af7d-dbd91b23a344)

## OUTPUT

echo $?

![s72](https://github.com/Mohanraj2006/OS-Linux-commands-Shell-script/assets/152195759/5b319444-b545-4918-808d-7ca07598d5bc)

## OUTPUT 
./one
bash: ./one: Permission denied
 
echo $?

![s73](https://github.com/Mohanraj2006/OS-Linux-commands-Shell-script/assets/152195759/951012f7-f28a-4ddf-bf42-8602e275059b)

## OUTPUT 
 
abcd
 
echo $?

![s74](https://github.com/Mohanraj2006/OS-Linux-commands-Shell-script/assets/152195759/fc793256-7668-4c28-94f7-8d567254b8a7)

 ## OUTPUT


 
# mis-using string comparisons

cat < strcomp.sh 
```bash
\#!/bin/bash
val1=baseball
val2=hockey
if [ $val1 \> $val2 ]
then
echo "$val1 is greater than $val2"
else
echo "$val1 is less than $val2"
fi
^d
```

cat strcomp.sh 
```bash
\#!/bin/bash
val1=baseball
val2=hockey
if [ $val1 \> $val2 ]
then
echo "$val1 is greater than $val2"
else
echo "$val1 is less than $val2"
fi
```

![s76](https://github.com/Mohanraj2006/OS-Linux-commands-Shell-script/assets/152195759/4013ee60-d534-47fc-9cc9-e14a12bece34)

##OUTPUT



chmod 755 strcomp.sh
 
./strcomp.sh 

![s77](https://github.com/Mohanraj2006/OS-Linux-commands-Shell-script/assets/152195759/638ae967-2c12-4a73-95e0-0dc04b31899a)

## OUTPUT


# check file ownership
cat < psswdperm.sh 
```bash
\#!/bin/bash
if [ -O /etc/passwd ]
then
echo “You are the owner of the /etc/passwd file”
else
echo “Sorry, you are not the owner of the /etc/passwd file”
fi
^d
```

cat psswdperm.sh 
```bash
/#!/bin/bash
if [ -O /etc/passwd ]
then
echo “You are the owner of the /etc/passwd file”
else
echo “Sorry, you are not the owner of the /etc/passwd file”
fi
 ```

![s78](https://github.com/Mohanraj2006/OS-Linux-commands-Shell-script/assets/152195759/62173aa6-46e8-4b3c-9229-7d1ddd70a63a)


./psswdperm.sh

![s79](https://github.com/Mohanraj2006/OS-Linux-commands-Shell-script/assets/152195759/56da2453-f1ff-4873-9405-93d5fe4507d0)

## OUTPUT

# check if with file location
cat>ifnested.sh 
```bash
\#!/bin/bash
if [ -e $HOME ]
then
echo “$HOME The object exists, is it a file?”
if [ -f $HOME ]
then
echo “Yes,$HOME it is a file!”
else
echo “No,$HOME it is not a file!”
if [ -f $HOME/.bash_history ]
then
echo “But $HOME/.bash_history is a file!”
fi
fi
else
echo “Sorry, the object does not exist”
fi
^d
```
cat ifnested.sh 
```
\#!/bin/bash
if [ -e $HOME ]
then
echo “$HOME The object exists, is it a file?”
if [ -f $HOME ]
then
echo “Yes,$HOME it is a file!”
else
echo “No,$HOME it is not a file!”
if [ -f $HOME/.bash_history ]
then
echo “But $HOME/.bash_history is a file!”
fi
fi
else
echo “Sorry, the object does not exist”
fi
```

![s81](https://github.com/Mohanraj2006/OS-Linux-commands-Shell-script/assets/152195759/7f5aa713-3a88-48b3-920c-6a7f97ba1167)



./ifnested.sh 

![s80](https://github.com/Mohanraj2006/OS-Linux-commands-Shell-script/assets/152195759/901dbf16-2456-4d04-aef1-ca970b6d756a)


## OUTPUT



# using numeric test comparisons
cat > iftest.sh 
```bash
\#!/bin/bash
val1=10
val2=11
if [ $val1 -gt 5 ]
then
echo “The test value $val1 is greater than 5”
fi
if [ $val1 -eq $val2 ]
then
echo “The values are equal”
else
echo “The values are different”
fi
^d
```


cat iftest.sh 
```bash
\#!/bin/bash
val1=10
val2=11
if [ $val1 -gt 5 ]
then
echo “The test value $val1 is greater than 5”
fi
if [ $val1 -eq $val2 ]
then
echo “The values are equal”
else
echo “The values are different”
fi
```

![s82](https://github.com/Mohanraj2006/OS-Linux-commands-Shell-script/assets/152195759/51c67a42-b3ff-40cb-8886-57e0ab4b7707)


$ chmod 755 iftest.sh
 
$ ./iftest.sh

![s83](https://github.com/Mohanraj2006/OS-Linux-commands-Shell-script/assets/152195759/51d92eb7-f021-4aff-a3ce-57fd86423ca4)

##OUTPUT

# check if a file
cat > ifnested.sh 
```bash
\#!/bin/bash
if [ -e $HOME ]
then
echo “$HOME The object exists, is it a file?”
if [ -f $HOME ]
then
echo “Yes,$HOME it is a file!”
else
echo “No,$HOME it is not a file!”
if [ -f $HOME/.bash_history ]
then
echo “But $HOME/.bash_history is a file!”
fi
fi
else
echo “Sorry, the object does not exist”
fi
^d
```

cat ifnested.sh 
```bash
\#!/bin/bash
if [ -e $HOME ]
then
echo “$HOME The object exists, is it a file?”
if [ -f $HOME ]
then
echo “Yes,$HOME it is a file!”
else
echo “No,$HOME it is not a file!”
if [ -f $HOME/.bash_history ]
then
echo “But $HOME/.bash_history is a file!”
fi
fi
else
echo “Sorry, the object does not exist”
fi
```

![s84](https://github.com/Mohanraj2006/OS-Linux-commands-Shell-script/assets/152195759/ba7914fd-04e0-4c19-94c8-320cf2c670b2)


$ chmod 755 ifnested.sh
 
$ ./ifnested.sh 

![s85](https://github.com/Mohanraj2006/OS-Linux-commands-Shell-script/assets/152195759/584bcea0-0906-4c3a-9958-90ec4377cbe7)

##OUTPUT

# looking for a possible value using elif
cat elifcheck.sh 
```bash
\#!/bin/bash
if [ $USER = Ram ]
then
echo "Welcome $USER"
echo "Please enjoy your visit"
elif [ $USER = Rahim ]
then
echo "Welcome $USER"
echo "Please enjoy your visit"
elif [ $USER = Robert ]
then
echo "Special testing account"
elif [ $USER = gganesh ]
then
echo "$USER, Do not forget to logout when you're done"
else
echo "Sorry, you are not allowed here"
fi
```

![s86](https://github.com/Mohanraj2006/OS-Linux-commands-Shell-script/assets/152195759/11e2b753-b457-4f39-a785-71959352695c)


$ chmod 755 elifcheck.sh
 
$ ./elifcheck.sh 

![s87](https://github.com/Mohanraj2006/OS-Linux-commands-Shell-script/assets/152195759/58c80893-7b16-4924-936b-9ab284c8637c)

## OUTPUT


# testing compound comparisons
cat> ifcompound.sh 
```bash
\#!/bin/bash
if [ -d $HOME ] && [ -w $HOME ]
then
echo "The file exists and you can write to it"
else
echo "I cannot write to the file"
fi
```
$ chmod 755 ifcompound.sh
$ ./ifcompound.sh 

![s88](https://github.com/Mohanraj2006/OS-Linux-commands-Shell-script/assets/152195759/d7efda70-b0ab-4ea2-ba55-2a5774daeffb)

## OUTPUT

# using the case command
cat >casecheck.sh 
```bash
case $USER in
Ram | Robert)
echo "Welcome, $USER"
echo "Please enjoy your visit";;
Rahim)
echo "Special testing account";;
gganesh)
echo "$USER, Do not forget to log off when you're done";;
*)
echo "Sorry, you are not allowed here";;
esac
```
$ chmod 755 casecheck.sh 
 
$ ./casecheck.sh 

 ![s89](https://github.com/Mohanraj2006/OS-Linux-commands-Shell-script/assets/152195759/13fc6b99-1d09-45ee-92dc-086ea2cb400d)

cat > whiletest
```bash
#!/bin/bash
#while command test
var1=10
while [ $var1 -gt 0 ]
do
echo $var1
var1=$[ $var1 - 1 ]
done
```
$ chmod 755 whiletest.sh
 
$ ./whiletest.sh
 
 ![s90](https://github.com/Mohanraj2006/OS-Linux-commands-Shell-script/assets/152195759/c4c44973-cf00-458b-b1f4-d5de08446b3a)

cat untiltest.sh 
```bash
\#using the until command
var1=100
until [ $var1 -eq 0 ]
do
echo $var1
var1=$[ $var1 - 25 ]
done
``` 
$ chmod 755 untiltest.sh
 
 ![s91](https://github.com/Mohanraj2006/OS-Linux-commands-Shell-script/assets/152195759/70c8542e-bccf-4c6b-9cc7-cbf454ee0027)

 
cat forin1.sh 
```bash
\#!/bin/bash
\#basic for command
for test in Alabama Alaska Arizona Arkansas California Colorado
do
echo The next state is $test
done
 ```

 ![s92](https://github.com/Mohanraj2006/OS-Linux-commands-Shell-script/assets/152195759/a88fd622-f1c7-4b94-8321-58c9d3dbed6f)

$ chmod 755 forin1.sh
 
 ![s93](https://github.com/Mohanraj2006/OS-Linux-commands-Shell-script/assets/152195759/7e93a73c-bf24-4ae0-8385-c00683194f16)


cat forin2.sh 
```bash
\#!/bin/bash
\# another example of how not to use the for command
for test in I don't know if this'll work
do
echo “word:$test”
done
```
$ chmod 755 forin2.sh
 
$ ./forin2.sh 

 ![s94](https://github.com/Mohanraj2006/OS-Linux-commands-Shell-script/assets/152195759/3144e35c-1267-4519-8a7d-d7598d8cc78e)

cat forin3.sh 
```bash
\#!/bin/bash
\# another example of how not to use the for command
for test in I don\'t know if "this'll" work
do
echo "word:$test"
done
```
$ chmod 755 forin1.sh
$ ./forin3.sh 

![s95](https://github.com/Mohanraj2006/OS-Linux-commands-Shell-script/assets/152195759/9ea3333d-e4e7-4c5a-af26-c1b4df6496f1) 

## OUTPUT
cat forinfile.sh 
```bash
#!/bin/bash
# reading values from a file
file="cities"
for state in `cat $file`
do
echo "Visit beautiful $file“
done
```
$ chmod 777 forinfile.sh
$ cat cities
Hyderabad
Alampur
Basara
Warangal
Adilabad
Bhadrachalam
Khammam

![s97](https://github.com/Mohanraj2006/OS-Linux-commands-Shell-script/assets/152195759/feae16ca-e20d-418b-8ddb-5610dd568a22)

![s96](https://github.com/Mohanraj2006/OS-Linux-commands-Shell-script/assets/152195759/0d72d45f-44d3-4ab7-b89c-8fd5ffe9600a)

## OUTPUT


cat forctype.sh 
```bash
#!/bin/bash
# testing the C-style for loop
for (( i=1; i <= 5; i++ ))
do
echo "The value of i is $i"
done
````
$ chmod 755 forctype.sh
$ ./forctype.sh

![s98](https://github.com/Mohanraj2006/OS-Linux-commands-Shell-script/assets/152195759/b7095457-e620-40ad-86f0-725886f37f3d)

 
## OUTPUT

cat forctype1.sh 
```bash
#!/bin/bash
# multiple variables
for (( a=1, b=5; a <= 5; a++, b-- ))
do
echo "$a - $b"
done
```
$ chmod 755 forctype.sh
$ ./forctype1.sh 

![s99](https://github.com/Mohanraj2006/OS-Linux-commands-Shell-script/assets/152195759/2f5702d2-736c-4305-a503-e54657e6848c)

## OUTPUT

cat fornested1.sh 
```bash
#!/bin/bash
# nesting for loops
for (( a = 1; a <= 3; a++ ))
do
echo "Starting loop $a:"
for (( b = 1; b <= 3; b++ ))
do
echo " Inside loop: $b"
done
done
```
$ chmod 755 fornested1.sh
 
$ ./fornested1.sh 


## OUTPUT

 
cat forbreak.sh 
```bash
#!/bin/bash
# breaking out of a for loop
for var1 in 1 2 3 4 5
do
if [ $var1 -eq 3 ]
then
break
fi
echo "Iteration number: $var1"
done
echo "The for loop is completed“
```
## OUTPUT

$ chmod 755 forbreak.sh
 
$ ./forbreak.sh 


 
cat forbreak.sh 
```bash
#!/bin/bash
# breaking out of a for loop
for var1 in 1 2 3 4 5
do
if [ $var1 -eq 3 ]
then
continue
fi
echo "Iteration number: $var1"
done
echo "The for loop is completed“
```

 
$ chmod 755 forcontinue.sh
 
$ ./forcontinue.sh 
## OUTPUT
 
cat exread.sh 
```bash
#!/bin/bash
# testing the read command
echo -n "Enter your name: "
read name
echo "Hello $name, welcome to my program. "
 ```
 
$ chmod 755 exread.sh 
 
$ ./exread.sh 
## OUTPUT


 cat exread1.sh
```bash
#!/bin/bash
# testing the read command
read -p "Enter your name: " name
echo "Hello $name, welcome to my program. “
``` 
$ chmod 755 exread1.sh 

## OUTPUT



$ ./exread1.sh 
 
cat funcex.sh
```bash
#!/bin/bash
# trying to access script parameters inside a function
function func {
echo $[ $1 * $2 ]
}
if [ $# -eq 2 ]
then
value=`func $1 $2`
echo "The result is $value"
else
echo "Usage: badtest1 a b"
fi
```
## OUTPUT
 ./funcex.sh 

 
 ./funcex.sh 1 2

 
cat argshift.sh
```bash
#!/bin/bash 
 while (( "$#" )); do 
  echo $1 
  shift 
done
```
$ chmod 777 argshift.sh

## OUTPUT
$ ./argshift.sh 1 2 3
 
 cat argshift1.sh
```bash
 #/bin/bash 
 # store arguments in a special array 
args=("$@") 
# get number of elements 
ELEMENTS=${#args[@]} 
 # echo each element in array  
# for loop 
for (( i=0;i<$ELEMENTS;i++)); do 
    echo ${args[${i}]} 
done
```
$ chmod 777 argshift.sh
## OUTPUT
$ ./argshift.sh 1 2 3
 
cat argshift.sh
```bash
#!/bin/bash 
set -x 
while (( "$#" )); do 
  echo $1 
  shift 
done
set +x
```
## OUTPUT
 ./argshift.sh 1 2 3
 
 
cat > nc.awk
```bash
BEGIN{}
{
print len=length($0),"\t",$0 
wordcount+=NF
chrcnt+=len
}
END {
print "total characters",chrcnt 
print "Number of Lines are",NR
print "No of Words count:",wordcount
}
 ```
cat>data.dat
```bash
bcdfghj
abcdfghj
bcdfghj
ebcdfghj
bcdfghj
ibcdfghj
bcdfghj
obcdfghj
bcdfghj
ubcdfghj
```
awk -f nc.awk data.dat
## OUTPUT 
 
cat > palindrome.sh
```bash
#num=545
echo "Enter the number"
read num
s=0
rev=""
temp=$num
while [ $num -gt 0 ]
do
	# Get Remainder
	s=$(( $num % 10 ))
	# Get next digit
	num=$(( $num / 10 ))
	# Store previous number and
	# current digit in reverse
	rev=$( echo ${rev}${s} )
done
if [ $temp -eq $rev ];
then
	echo "Number is palindrome"
else
	echo "Number is NOT palindrome"
fi
```
## OUTPUT 

$ chmod 755 palindrome.sh

$ ./palindrome.sh



# RESULT:
The Commands are executed successfully.
