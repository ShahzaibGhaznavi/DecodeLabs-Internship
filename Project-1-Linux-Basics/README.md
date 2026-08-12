# Project 1: Linux & Command Line Basics

## Objective

Practice basic Linux commands and perform a web application setup using files, directories, logs, verification, backup, and permissions.

## Web App Setup

### 1. Scaffold

Created the application log directory:

```bash
sudo mkdir -p /app/logs
```

### 2. Config

Created the application configuration file:

```bash
sudo touch /app/config.conf
```

### 3. Inject

Created the server log and added the `Started` message:

```bash
sudo sh -c 'echo "Started" > /app/logs/server.log'
```

Verified the log content:

```bash
cat /app/logs/server.log
```

Output:

```text
Started
```

### 4. Verify

Checked the current working directory and application structure:

```bash
pwd
sudo ls -R /app
```

The `/app` directory contains:

```text
/app/
├── config.conf
└── logs/
    └── server.log
```

### 5. Backup

Created a backup of the server log:

```bash
sudo mv /app/logs/server.log /app/logs/server.bak
```

Verified the backup:

```bash
sudo ls -l /app/logs
```

### 6. Audit

Checked the configuration file and its permissions:

```bash
sudo ls -l /app/config.conf
```

## Skills Practiced

* Linux directory and file management
* `mkdir`
* `touch`
* `echo`
* `cat`
* `pwd`
* `ls`
* File backup using `mv`
* Basic file permission inspection
* Working with application logs

## Result

Completed the Linux & Command Line Basics project on an Ubuntu server by creating the required application structure, configuration file, server log, log backup, and verifying file permissions.
