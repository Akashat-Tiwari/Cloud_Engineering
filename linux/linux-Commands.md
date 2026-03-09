# Linux Basics 

**->**  Linux is an "open-source operating system kernel" created by Linus Torvalds in 1991. It serves as the core of many operating systems (called "distributions") used worldwide. Linux is built on a kernel + userspace model

**->**  '$' symbol at the starting is not the part of a command , it indicates the command should be typed into the terminal . 

## Three major linux distribution families : 
 ### **#1**  Red Hat family systems (Red Hat Enterprise Linux : RHEL)

**->**  widely used by Enterprises which hosts their own systems 

**->**  feDora is upstream for Red Hat 

### **#2**  SUSE family systems

**->**  widely used in retail

**->**  SLES (SUSE Linux Enterprise Server) is upstream for openSUSE

### **#3**  Debian family systems (ubuntu, Linux mint)

**->**  Debian family is upstream for ubuntu

**->**  ubuntu LTS (Long term support) as the reference to the debian family distribution

**->**  widely used in cloud deployments

## Common Linux terms  

**->**  ### Kernel : manages hardware (CPU, memory, devices) and applications , BRAIN of a Linux OS

**->**  ### Distribution (Distro) : kernel + tools + package manager bundled together, collection of the software making up a linux OS

**->**   Boot Loader : Program that boots the OS 

**->**   Service : Program that runs as a background Process

**->**   fileSystem : Methods for storing and organising files

**->**   X Window System : standard toolkit and protocol to build GUI on nearly all Linux systems

**->**   Desktop Environment : GUI on top of the OS

**->**   Command line :  Interface for typing commands on top of the OS

**->**   Shell :   interface to interact with the system (bash, zsh),  interpreter that interprets the command line input and instructs the OS to perform any necessary task

## System Startup 

### Boot process :

**->**  1. BIOS-Basic I/O System (The first Step) 

**->**  2. Master Boot Record (MBR) : First sector of the HardDisk - size of MBR is just 512 bytes 

**->**  3. Boot Loader eg. Grub

**->**  4. kernel 

**->**  5. Initial RAM disk

**->**  6. Parent Process

**->**  6. Command shell using gitty

**->**  6. X window System (GUI)

### Linux FileSystems : 
