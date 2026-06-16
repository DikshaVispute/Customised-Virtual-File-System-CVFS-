# Customised-Virtual-File-System-CVFS-
A simulation of a Linux-like virtual file system implemented in C with inode-based architecture and custom shell commands.

## Project Overview
Customized Virtual File System (CVFS) is a Linux-based file system simulation project developed in C. The project mimics the internal working of an operating system file system by implementing concepts such as inodes, superblocks, file tables, file permissions, and file management operations.

The project provides a command-line shell interface where users can create, read, write, list, and delete virtual files inside the customized file system.

This project demonstrates:
- Operating System Concepts
- File System Architecture
- Inode Management
- Memory Management
- Command Line Shell Development
- File Handling Mechanisms

---

# Features
- Create Virtual Files
- Read Data from Files
- Write Data into Files
- Delete Files
- List Existing Files
- File Permission Management
- Manual Help Commands
- File Descriptor Management
- Simulated File System Environment
- User File Descriptor Table (UFDT)
- Inode-Based File Management

---

# Technologies Used
- C Programming
- Linux System Programming
- Dynamic Memory Allocation
- File System Concepts
- Command Line Interface
- Data Structures

---

# Project Structure

```
CVFS/
│
├── cvfs.c
└── README.md
```

---

# Core Components

## Boot Block
Stores information required during initialization of the virtual file system.

---

## Super Block
Maintains:
- Total Inodes
- Free Inodes

---

## Inode
Stores file-related metadata:
- File Name
- File Size
- File Type
- Permissions
- Buffer Address
- Reference Count

---

## File Table
Maintains:
- Read Offset
- Write Offset
- File Mode
- Inode Connection

---

## UAREA
Maintains:
- Process Information
- User File Descriptor Table (UFDT)

---

# Supported Commands

| Command | Description |
|---------|-------------|
| `creat` | Create new file |
| `write` | Write data into file |
| `read` | Read data from file |
| `unlink` | Delete file |
| `ls` | List all files |
| `help` | Display help page |
| `man` | Display manual page |
| `clear` | Clear terminal |
| `exit` | Terminate CVFS |

---

# File Permissions

| Permission | Value |
|------------|------|
| READ | 1 |
| WRITE | 2 |
| EXECUTE | 4 |

---

# How to Run the Project

## Step 1: Compile the Program

```
gcc cvfs.c -o cvfs
```

---

## Step 2: Run the Application

```
./cvfs
```

---

# Sample Commands

## Create File

```
creat Demo.txt 3
```

---

## Write into File

```
write 3
```

---

## Read from File

```
read 3 10
```

---

## Delete File

```
unlink Demo.txt
```

---

## List Files

```
ls
```

---

# Sample Output

```
-----------------------------------------------
----- Marvellous CVFS started succesfully -----
-----------------------------------------------
```

---

# Concepts Used
- File System Simulation
- Inode Architecture
- Super Block Management
- File Descriptor Table
- Dynamic Memory Allocation
- Command Line Parsing
- File Permissions
- Linked List Implementation
- Linux Shell Concepts

---

# Learning Outcomes
Through this project, you can learn:
- Internal working of operating system file systems
- File management using inodes
- Memory allocation techniques
- Linux command-line application development
- File descriptor management
- Virtual file system architecture

---

# Future Enhancements
- Directory Management
- Multi-user Support
- File Encryption
- Password Protected Files
- Copy and Move Commands
- File Compression
- Journaling Mechanism
- Persistent Storage Support

---

# Author
Developed by Om Mahale as an Operating System and System Programming project using C.

Source Code Reference: :contentReference[oaicite:0]{index=0}
