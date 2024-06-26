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
![Screenshot 2024-03-21 102129](https://github.com/ARCH2006/OS-Linux-commands-Shell-script/assets/144300030/1dbb0ec7-e247-4a7a-9d92-ab3e624d8fcb)

cat > file2
```
anil aggarwal
barun sengupta
c.k. shukla
lalit chowdury
s.n. dasgupta
^d
```
### Display the content of the files
cat < file1
## OUTPUT
![Screenshot 2024-03-21 102249](https://github.com/ARCH2006/OS-Linux-commands-Shell-script/assets/144300030/fdf2069b-bc71-4953-8a8c-b81d936f5ff0)



cat < file2
## OUTPUT
![Screenshot 2024-03-21 102811](https://github.com/ARCH2006/OS-Linux-commands-Shell-script/assets/144300030/e579c596-2262-4aa8-99d8-29bd39fa8b52)


# Comparing Files
cmp file1 file2
## OUTPUT
 ![Screenshot 2024-03-21 102941](https://github.com/ARCH2006/OS-Linux-commands-Shell-script/assets/144300030/37582fb3-5661-462a-9db3-c3552ff08920)

comm file1 file2
 ## OUTPUT

 ![Screenshot 2024-03-21 103109](https://github.com/ARCH2006/OS-Linux-commands-Shell-script/assets/144300030/b2cca964-f2db-4f43-bed6-230331ac45dd)

diff file1 file2
## OUTPUT

![Screenshot 2024-03-21 103241](https://github.com/ARCH2006/OS-Linux-commands-Shell-script/assets/144300030/9c8e37e5-0ea5-4dbc-bc89-a81c8e8fe617)

#Filters

### Create the following files file11, file22 as follows:

cat > file11
![Screenshot 2024-03-21 103433](https://github.com/ARCH2006/OS-Linux-commands-Shell-script/assets/144300030/321a30f3-5f9d-4099-852e-4679d3d2c773)

Hello world
This is my world
^d
```
cat > file22
```
1001 | Ram | 10000 | HR
1002 | tom |  5000 | Admin
1003 | Joe |  7000 | Developer
^d


![Screenshot 2024-03-21 103722](https://github.com/ARCH2006/OS-Linux-commands-Shell-script/assets/144300030/3fcbb97e-eea1-442f-b6ce-344c72db13e3)

cut -c1-3 file11
## OUTPUT

![Screenshot 2024-03-21 103846](https://github.com/ARCH2006/OS-Linux-commands-Shell-script/assets/144300030/923e34b9-816e-4c27-9ddf-201f57819eaa)



cut -d "|" -f 1 file22
## OUTPUT

![Screenshot 2024-03-21 103924](https://github.com/ARCH2006/OS-Linux-commands-Shell-script/assets/144300030/9f4a017c-25f4-4e43-b0f8-6a8f743cc7ed)


cut -d "|" -f 2 file22
## OUTPUT

![Screenshot 2024-03-21 103952](https://github.com/ARCH2006/OS-Linux-commands-Shell-script/assets/144300030/77be0877-2aaf-4467-a505-8fd5fd3abfcc)

cat < newfile 
```
Hello world
hello world
^d
````
![Screenshot 2024-03-21 104212](https://github.com/ARCH2006/OS-Linux-commands-Shell-script/assets/144300030/99984836-3250-44b3-a23c-7fb6ed5223b8)

cat > newfile 
Hello world
hello world
 ![Screenshot 2024-03-21 104226](https://github.com/ARCH2006/OS-Linux-commands-Shell-script/assets/144300030/93e07b35-5eee-4ee6-ba9a-586323328f44)

grep Hello newfile 
## OUTPUT

![Screenshot 2024-03-21 104725](https://github.com/ARCH2006/OS-Linux-commands-Shell-script/assets/144300030/28ed7b06-f0f7-4ed4-895d-0fc22f2695a5)


grep hello newfile 
## OUTPUT
![Screenshot 2024-03-21 104736](https://github.com/ARCH2006/OS-Linux-commands-Shell-script/assets/144300030/1c7974b3-4426-437a-b458-5cdaee07a8aa)





grep -v hello newfile 
## OUTPUT

![Screenshot 2024-03-21 104743](https://github.com/ARCH2006/OS-Linux-commands-Shell-script/assets/144300030/48e1f6f6-fde4-4fb2-83cd-c402f06345a5)


cat newfile | grep -i "hello"
## OUTPUT

![Screenshot 2024-03-21 104751](https://github.com/ARCH2006/OS-Linux-commands-Shell-script/assets/144300030/a47221c6-c2eb-4708-b1a3-782d6361c473)



cat newfile | grep -i -c "hello"
## OUTPUT

![Screenshot 2024-03-21 104758](https://github.com/ARCH2006/OS-Linux-commands-Shell-script/assets/144300030/c027d811-39ec-4eae-8c97-304d5bbdfcbd)



grep -R ubuntu /etc
## OUTPUT
![Screenshot 2024-03-21 104943](https://github.com/ARCH2006/OS-Linux-commands-Shell-script/assets/144300030/7cc34e5b-3ced-4437-be48-5f413cf30a77)



grep -w -n world newfile   
## OUTPUT
![Screenshot 2024-03-21 105211](https://github.com/ARCH2006/OS-Linux-commands-Shell-script/assets/144300030/4995ff57-d3ad-488d-9a2f-62f543bbf0e2)


cat < newfile 
```
Hello world
hello world
Linux is world number 1
Unix is predecessor
Linux is best in this World
^d
```
![Screenshot 2024-03-21 105427](https://github.com/ARCH2006/OS-Linux-commands-Shell-script/assets/144300030/5df7629a-3b11-4808-9ae6-f8b13bd946d1)

cat > newfile
```
Hello world
hello world
Linux is world number 1
Unix is predecessor
Linux is best in this World
^d```
 ```
![Screenshot 2024-03-21 105516](https://github.com/ARCH2006/OS-Linux-commands-Shell-script/assets/144300030/50a67961-13d9-45e4-b380-b5bf99f8bbb4)


egrep -w 'Hello|hello' newfile 
## OUTPUT

![Screenshot 2024-03-21 105558](https://github.com/ARCH2006/OS-Linux-commands-Shell-script/assets/144300030/cca7bc3a-638d-4f80-8141-bfa54f553b33)


egrep -w '(H|h)ello' newfile 
## OUTPUT


![Screenshot 2024-03-21 105955](https://github.com/ARCH2006/OS-Linux-commands-Shell-script/assets/144300030/d03ef707-d6dc-4c25-b1c2-df99aeb26d1c)

egrep -w '(H|h)ell[a-z]' newfile 
## OUTPUT

![Screenshot 2024-03-21 110045](https://github.com/ARCH2006/OS-Linux-commands-Shell-script/assets/144300030/0530062f-a4b5-4e60-b3de-277d32168c86)



egrep '(^hello)' newfile 
## OUTPUT

![Screenshot 2024-03-21 110153](https://github.com/ARCH2006/OS-Linux-commands-Shell-script/assets/144300030/7a76ed0a-d35d-4a8c-a9b1-fcb7656cc820)


egrep '(world$)' newfile 
## OUTPUT


![Screenshot 2024-03-21 110312](https://github.com/ARCH2006/OS-Linux-commands-Shell-script/assets/144300030/3802c7bc-e059-4710-85a7-ec1c3e748a94)

egrep '(World$)' newfile 
## OUTPUT

![Screenshot 2024-03-21 110437](https://github.com/ARCH2006/OS-Linux-commands-Shell-script/assets/144300030/04cfcf43-47c0-4e98-a947-92aa3526f9db)

egrep '((W|w)orld$)' newfile 
## OUTPUT


![Screenshot 2024-03-21 110604](https://github.com/ARCH2006/OS-Linux-commands-Shell-script/assets/144300030/3111ddbb-38de-476b-92de-8c3b760696a0)

egrep '[1-9]' newfile 
## OUTPUT

![Screenshot 2024-03-21 110646](https://github.com/ARCH2006/OS-Linux-commands-Shell-script/assets/144300030/1ac94536-e23e-4065-9167-d921417cbd62)


egrep 'Linux.*world' newfile 
## OUTPUT
![Screenshot 2024-03-21 110839](https://github.com/ARCH2006/OS-Linux-commands-Shell-script/assets/144300030/71f44c2f-d104-462f-8785-68a0007ad3de)


egrep 'Linux.*World' newfile 
## OUTPUT
![Screenshot 2024-03-21 111021](https://github.com/ARCH2006/OS-Linux-commands-Shell-script/assets/144300030/d375eb14-d5ef-4302-9df1-1c97974e9052)


egrep l{2} newfile
## OUTPUT

![Screenshot 2024-03-21 111328](https://github.com/ARCH2006/OS-Linux-commands-Shell-script/assets/144300030/c8fc2d90-e362-4cd2-8f02-10c610da646e)


egrep 's{1,2}' newfile
## OUTPUT 
![Screenshot 2024-03-21 111420](https://github.com/ARCH2006/OS-Linux-commands-Shell-script/assets/144300030/677db0d0-4fa4-41bc-ad8a-b1e6a1df7dd3)


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
![Screenshot 2024-03-21 111956](https://github.com/ARCH2006/OS-Linux-commands-Shell-script/assets/144300030/95f61db0-d1d1-41e4-9435-8ddcd443d837)


sed -n -e '3p' file23
## OUTPUT


![Screenshot 2024-03-21 112540](https://github.com/ARCH2006/OS-Linux-commands-Shell-script/assets/144300030/f0d87f74-f752-4b18-b5b8-b50a7918ff88)

sed -n -e '$p' file23
## OUTPUT


![Screenshot 2024-03-21 113822](https://github.com/ARCH2006/OS-Linux-commands-Shell-script/assets/144300030/3e185f63-5c58-4309-aefd-10022584fa0d)

sed  -e 's/Ram/Sita/' file23
## OUTPUT

![Screenshot 2024-03-21 114000](https://github.com/ARCH2006/OS-Linux-commands-Shell-script/assets/144300030/c97cbba1-e572-4267-b1ed-1002bfecf628)


sed  -e '2s/Ram/Sita/' file23
## OUTPUT

![Screenshot 2024-03-21 114047](https://github.com/ARCH2006/OS-Linux-commands-Shell-script/assets/144300030/b90f9006-7756-406b-8cc9-55f59f34a2bf)


sed  '/tom/s/5000/6000/' file23
## OUTPUT



sed -n -e '1,5p' file23
## OUTPUT
![Screenshot 2024-03-24 225736](https://github.com/ARCH2006/OS-Linux-commands-Shell-script/assets/144300030/b9e54493-c2d8-4328-9856-1326a4c75550)



sed -n -e '2,/Joe/p' file23
## OUTPUT

![Screenshot 2024-03-24 225918](https://github.com/ARCH2006/OS-Linux-commands-Shell-script/assets/144300030/b9caa9fa-e039-45e4-9aca-65172526c183)



sed -n -e '/tom/,/Joe/p' file23
## OUTPUT
![Screenshot 2024-03-24 230013](https://github.com/ARCH2006/OS-Linux-commands-Shell-script/assets/144300030/e660fb8b-cfda-4e10-80a7-d9126ad34e7d)



seq 10 
## OUTPUT
![Screenshot 2024-03-24 230034](https://github.com/ARCH2006/OS-Linux-commands-Shell-script/assets/144300030/da23d47e-54de-4d7c-9e89-f6143ddfacad)



seq 10 | sed -n '4,6p'
## OUTPUT

![Screenshot 2024-03-24 230143](https://github.com/ARCH2006/OS-Linux-commands-Shell-script/assets/144300030/35f8a672-7bc4-4ef2-9c5c-bef4a6558666)


seq 10 | sed -n '2,~4p'
## OUTPUT



seq 3 | sed '2a hello'
## OUTPUT
![Screenshot 2024-03-24 230641](https://github.com/ARCH2006/OS-Linux-commands-Shell-script/assets/144300030/ef90dc44-9cb4-463d-9546-786838971128)



seq 2 | sed '2i hello'
## OUTPUT
![Screenshot 2024-03-24 230715](https://github.com/ARCH2006/OS-Linux-commands-Shell-script/assets/144300030/f795a026-6e18-40d0-8050-671a8a7c9812)


seq 10 | sed '2,9c hello'
## OUTPUT

![Screenshot 2024-03-24 230751](https://github.com/ARCH2006/OS-Linux-commands-Shell-script/assets/144300030/98068c09-7630-4d68-a561-9cf338b4f7ac)

sed -n '2,4{s/^/$/;p}' file23
## OUTPUT
![Screenshot 2024-03-24 230841](https://github.com/ARCH2006/OS-Linux-commands-Shell-script/assets/144300030/2c09d031-72fb-4e32-972f-70440ed0c570)



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
## OUTPUT
![Screenshot 2024-03-24 231040](https://github.com/ARCH2006/OS-Linux-commands-Shell-script/assets/144300030/22c337e9-6a2f-4fa2-9275-5ab98d80b9e0)


cat > file22
```
1001 | Ram | 10000 | HR
1001 | Ram | 10000 | HR
1002 | tom |  5000 | Admin
1003 | Joe |  7000 | Developer
1005 | Sam |  5000 | HR
1004 | Sit |  7000 | Dev
``` 
uniq file22
## OUTPUT
![Screenshot 2024-03-24 231221](https://github.com/ARCH2006/OS-Linux-commands-Shell-script/assets/144300030/0fb61656-d15e-4e4c-9fdb-e787a97bd160)



#Using tr command

cat file23 | tr [:lower:] [:upper:]
 ## OUTPUT
![Screenshot 2024-03-24 231556](https://github.com/ARCH2006/OS-Linux-commands-Shell-script/assets/144300030/30017b4e-199a-45a0-8e44-c2207695abb7)

cat < urllist.txt
```
www. yahoo. com
www. google. com
www. mrcet.... com
^d
 ```
![Screenshot 2024-03-24 231857](https://github.com/ARCH2006/OS-Linux-commands-Shell-script/assets/144300030/f4fd3aa4-353d-40e9-aec5-f187c05ae966)

cat > urllist.txt
```
www. yahoo. com
www. google. com
www. mrcet.... com
```
![Screenshot 2024-03-24 231912](https://github.com/ARCH2006/OS-Linux-commands-Shell-script/assets/144300030/e9ff8114-fc1e-4dad-8dc5-b4b5d6bb6dbe)

cat urllist.txt | tr -d ' '
 ## OUTPUT
 ![Screenshot 2024-03-24 232812](https://github.com/ARCH2006/OS-Linux-commands-Shell-script/assets/144300030/3d3722a0-b498-480b-a5d8-db22dc26fb77)

# Shell Script
```
echo '#!/bin/sh' > my-script.sh
echo 'echo Hello World‘; exit 0 >> my-script.sh
```
chmod 755 my-script.sh
./my-script.sh
## OUTPUT

 
cat << stop > herecheck.txt
```
hello in this world
i cant stop
for this non stop movement
stop
```
![Screenshot 2024-03-24 233219](https://github.com/ARCH2006/OS-Linux-commands-Shell-script/assets/144300030/7be20d94-812d-448c-9925-017bfe5bf951)

cat herecheck.txt
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
![Screenshot 2024-03-24 233300](https://github.com/ARCH2006/OS-Linux-commands-Shell-script/assets/144300030/50ecd577-fb99-43f4-b211-76bfc576e4ec)

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
![Screenshot 2024-03-24 233311](https://github.com/ARCH2006/OS-Linux-commands-Shell-script/assets/144300030/38edeac0-1705-4e86-9379-ca79e3b227bf)
 
chmod 777 scriptest.sh
 
./scriptest.sh 1 2 3

## OUTPUT
```
File name is ./scriptest.sh
File name is scriptest.sh
First arg. is 1
Second arg. is 2
Third arg. is 3
Fourth arg. is
The $@ is 1 2 3
The $\# is $#
The $$ is 124
 ```
ls file1
## OUTPUT
![307826499-e004d6ed-48ab-45a6-bfd8-ab8faa8788b5](https://github.com/ARCH2006/OS-Linux-commands-Shell-script/assets/144300030/19943430-9fff-41ef-a887-e011b392d7cb)

 
echo $?
## OUTPUT 
 
abcd
 
echo $?
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
##OUTPUT

![307828678-669c08af-be10-452a-a16b-2d960c674987](https://github.com/ARCH2006/OS-Linux-commands-Shell-script/assets/144300030/96d2172d-891e-49b1-a189-fe3372e8b089)


chmod 755 strcomp.sh
 
./strcomp.sh 
## OUTPUT
``
baseball is less than hockey
``
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
./psswdperm.sh
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

./ifnested.sh 
## OUTPUT

![307832276-efa998fe-2806-4eca-ace7-1d71dda33cf6](https://github.com/ARCH2006/OS-Linux-commands-Shell-script/assets/144300030/d87b630f-fa38-44ab-b5bc-86417b653276)


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

$ chmod 755 iftest.sh
 
$ ./iftest.sh 
##OUTPUT
![307833052-545398c0-2c77-4e44-b53a-6ef098142c6f](https://github.com/ARCH2006/OS-Linux-commands-Shell-script/assets/144300030/3d9c645d-9f56-4dcd-a53c-83b9d91c3adb)

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

$ chmod 755 ifnested.sh
 
$ ./ifnested.sh 
##OUTPUT
![307833801-3f9abd70-a9ff-43f5-9b46-39fd1f374d55](https://github.com/ARCH2006/OS-Linux-commands-Shell-script/assets/144300030/d4c2864e-4848-49a6-b0bc-bba13677a5e1)

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

$ chmod 755 elifcheck.sh
 
$ ./elifcheck.sh 
## OUTPUT
```
Welcome Ram
Please enjoy your visit
Welcome Rahim
Please enjoy your visit
Special testing account
gganesh, Do not forget to logout when you're done
Sorry, you are not allowed here
```

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
## OUTPUT
![307834688-73bf26c3-76c2-4dbe-8aa4-213a1cef52fb](https://github.com/ARCH2006/OS-Linux-commands-Shell-script/assets/144300030/9ba523fb-3610-48ef-bec2-26960584ae6f)


# RESULT:
The Commands are executed successfully.
