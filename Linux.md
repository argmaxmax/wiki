# The Linux Operating System
## Operating Systems Concepts
Abstractions is one of the main concepts of operating systems concepts.
An Operating System itself is a program running on a computer, that maintains the system itself and also runs other programs.
An Operating System can be broken down into three parts in the following way:
1. Hardware  
		1. CPU  
		2. RAM  
		3. Disks  
		4. Network Ports  
2. Kernel  
		1. System Calls  
		2. Process Management  
		3. Memory Management  
		4. Device Drivers  
3. User Processes  
		1. GUI  
		2. Servers  
		3. Shell

Es gibt den Kernel und den User Mode. Der Kernel kann die Hardware uneingeschränkt nutzen, der user bzw die user processes nur einen kleinen Teil des sog Kernel Spaces, den User Space.
Um mit den Kernel zu kommunizieren, nutzen Prozesse system calls.

Beim managen von Prozessen nutzt den kernel context switches, welche eine art fliegender Wechsel zwischen Prozessen ist. Es laufen immer nur für kurze timeslices ein Prozess, bis der nächste ein bisschen Zeit vom Kernel eingeteilt bekommt.  Zwei Syscalls sind besonders wichtig, fork und exec. Jeder user Prozess außer init entsteht aus fork, und meistens wird auch exec ausgeführt um ein.  Wenn ein process fork callt, erstellt der kernel einen fast identischen prozess. Wenn ein process exec(program) callt, dann startet der kernel program, den current process ersetzend. 
Auf einem System gibt es mindestens den root user, und user sind da um berechtigungen und abgrenzungen zu unterstützen. Dabei hat jeder user space process einen user "owner" und der process heißt as owner laufend.

User können genau ihre eigenen processes zu einem gewissen grad beeinflussen. 

## The Linux Shell
### `cat` & co.
Der `cat` befehl gibt inhalte von endlich vielen Dateien aus: 
```
cat file_1 file_2
```
The `ls` command displays contents of directories. Using it, including filetypes in long version:
```
ls -l -F
```
The `cp` command copies `file1` into `file2` and replaces or `touch`es `file2`:
```
cp file_1 file_2
```
- renamed dateien `mv file_1 file_2`
- aber man kann auch mehrere files in ein directory moven mit: `mv file_1 file2 dir`
