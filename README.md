# use_gdb_in_vscode

## this is a tutorial of remote gdb debug a program in VScode


1 Install Plugin

![alt text](image-1.png)

2 Run -> Add Configuration..., open the launch.json

![alt text](image-3.png)

3 Add configuration....
![alt text](image-4.png)

4 Select the {}C/C++: (gdb) Launch

![alt text](image.png)

5 Set program and args

note: 

program is the file(with path) of you will execute

for args, use coma and double quotes to seprater each character

for example : 

./bin/rdma_rc_example 192.100.222.22 -d xib_0 -g 1 -t write -s 4096

args is 192.100.222.22 -d xib_0 -g 1 -t write -s 4096

in the json, configure as "args": ["192.168.222.22", "-d", "xib_0", "-g", "1", "-t", "write", "-s", "4096"],

![alt text](image-5.png)

6 Add break points

![alt text](image-8.png)

7 run and debug

![alt text](image-9.png)