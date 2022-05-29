
# 영속성 Persistence
### 영속성이란 무엇인가?
- 컴퓨터 충돌, 디스크 장애 등에도 불구하고 정보를 지속적으로 유지
- 



## I/O Devices
  #### System Architecture
  #### A Canonical Device
  #### The Canonical Protocol
  #### Lowering CPU overhead with Interrupt
  #### More Efficient Data Movement with DMA
  #### Methods of Device Interaction
  #### Fitting into the OS: The Device Driver
  #### Case Study: A simple IDE Disk Driver
  #### Historical Notes

## Hard Disk Drives
  #### The interface
  #### Basic Geometry
  #### A Simple Disk Drive
  #### I/O Time : Doing the Math
  #### Disk Scheduling
  
## Interlude: Files and Directories
  #### Files and Directories 
  #### File System Interface 
  #### Creating Files
  #### Reading and Writing Files
  #### Reading and Writing, But Not Sequentially 
  #### Shared file table entries: fork() and dup()
  #### Writing immediately with fsync()
  #### Renaming files
  #### Getting information about files
  #### Removing files
  #### Making Directories
  #### Reading Directories
  #### Deleting Directories
  #### Hard Links
  #### Symbolic Links
  #### Permission Bits and Access Control Lists
  #### Making and Mounting a file system 

  

## File System Implementation
  #### The Way to Think
  #### Overall Organization
  #### File Organization: The inode
  #### Directory Organization
  #### Free Space Mgmt.
  #### Access Paths: Reading and Writing
  #### Caching and Buffering
  
  
  
  
## Locality and The Fast File System (FFS)
  #### Poor performance
  #### FFS: Disk Awareness
  #### Organizing Structure: The Cylinder Group
  #### Policies: How to Allocate Files and Directories
  #### The Large-File Exception
  #### A Few Other Things about FFS
  
  
## Crash Consistency: FSCK and Journaling
  #### A Detailed Example
  #### Solution #1: The File System Checker
  #### Solution #2: Journaling (or WAL)
  #### Solution #3: Other Approaches
  
## Features of Various FS: Ext2/3/4, FAT, Flash FS
  #### Ext2
  #### Ext3
  #### Ext4
  #### FAT
  #### Flash-aware FS







  
