---
title: "OverTheWire Bandit Solutions: Levels 0 to 5"
layout: post
date: 2024-08-13
categories: bandit solutions 
---

# OverTheWire Bandit Solutions: levels 0 to 5

Well, good afternoon, good evening, and good night everyone, wherever you are in the world. Welcome to the first installation of my OverTheWire Bandit Solutions guide: *A Linux Admin's Guide to Solving OverTheWire's Bandit*. You can call me Anya, and I will be beginning with **level 0 up to level 5** of Bandit in this installment. There's a lot of good stuff coming up—we're going to learn about **ls, cat, and find**. Let's forge ahead and finish up Bandit!

## Bandit Level 0 to 1

### Level Goal

The goal of this level is to connect to the Bandit game server using SSH. The password for the next level is stored in a file named `readme` located in the home directory.

### Steps

1. **Connect to the Bandit server** using SSH:

    ```bash
    ssh bandit0@bandit.labs.overthewire.org -p 2220
    ```

    Use the password `bandit0` when prompted.

2. **List the contents** of the home directory:

    ```bash
    ls
    ```

3. **Read the `readme` file** to find the password for the next level:

    ```bash
    cat readme
    ```

4. **SSH into Bandit 1** using the password you found:

    ```bash
    ssh bandit1@bandit.labs.overthewire.org -p 2220
    ```

---

## Bandit Level 1 to 2

### Level Goal

The password for the next level is stored in a file called `-` located in the home directory.

### Steps

1. **List the contents** of the home directory:

    ```bash
    ls
    ```

2. **Read the file named `-`** by specifying the file path:

    ```bash
    cat ./-
    ```

3. **SSH into Bandit 2** using the password you found:

    ```bash
    ssh bandit2@bandit.labs.overthewire.org -p 2220
    ```

---

## Bandit Level 2 to 3

### Level Goal

The password for the next level is stored in a file called `spaces in this filename` located in the home directory.

### Steps

1. **List the contents** of the home directory:

    ```bash
    ls
    ```

2. **Read the file** with spaces in its name by enclosing it in quotes:

    ```bash
    cat "spaces in this filename"
    ```

3. **SSH into Bandit 3** using the password you found:

    ```bash
    ssh bandit3@bandit.labs.overthewire.org -p 2220
    ```

---

## Bandit Level 3 to 4

### Level Goal

The password for the next level is stored in a hidden file in the `inhere` directory.

### Steps

1. **Navigate to the `inhere` directory**:

    ```bash
    cd inhere
    ```

2. **List all files, including hidden ones**:

    ```bash
    ls -a
    ```

3. **Read the hidden file** to find the password:

    ```bash
    cat .hidden
    ```

4. **SSH into Bandit 4** using the password you found:

    ```bash
    ssh bandit4@bandit.labs.overthewire.org -p 2220
    ```

---

## Bandit Level 4 to 5

### Level Goal

The password for the next level is stored in a file with human-readable content among many other files in the `inhere` directory.

### Steps

1. **Navigate to the `inhere` directory**:

    ```bash
    cd inhere
    ```

2. **Identify the file with human-readable content**:

    ```bash
    file ./*
    ```

    Look for the file that is identified as ASCII text.

3. **Read the contents** of the identified file to find the password:

    ```bash
    cat ./-file07
    ```

4. **SSH into Bandit 5** using the password you found:

    ```bash
    ssh bandit5@bandit.labs.overthewire.org -p 2220
    ```
---

Congratulations on making it through levels 0 to 5! These introductory levels of Bandit are excellent for familiarizing yourself with basic Linux commands and concepts. 

Stay tuned for the next part, where we'll tackle even more challenging levels.

---

Thanks for following along! If you found this guide helpful, feel free to share it with others or leave a comment below. 

Until next time, happy hacking!
