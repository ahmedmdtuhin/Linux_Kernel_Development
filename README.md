
# HelloModule – Linux Kernel Module

This project demonstrates a simple **"Hello, World!"** Linux kernel module written in C. It introduces the basics of kernel module programming, including initialization and cleanup functions, and how to build and load modules in the Linux kernel.

## 📂 Directory Structure

```
HelloModule/
├── hello.c          # Main kernel module source
├── Makefile         # Makefile to build the module
```

## 🧩 Features

- Prints "Hello, Kernel!" on insertion
- Logs "Goodbye, Kernel!" on removal
- Demonstrates `module_init` and `module_exit`

## 🛠️ Build & Run

### 🧱 Build the Module

```bash
make
```

### 📦 Insert the Module

```bash
sudo insmod hello.ko
```

### 🔍 Check Kernel Log

```bash
dmesg | tail
```

### 🧹 Remove the Module

```bash
sudo rmmod hello
```

## 📎 Requirements

- Linux system with kernel headers installed
- GCC and `make` tools

## 🧠 Learning Purpose

This is a learning project for getting started with Linux Kernel Module Development.

📘 Based on [Linux Kernel Programming](https://www.udemy.com/course/linux-kernel-programming/)

---

> 🧪 Caution: Loading kernel modules can crash your system if done improperly. Use on virtual machines or development environments.
