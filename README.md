# File Transfer Protocol

This project, for course Network Programming, implements FTP server and client by using socket programming in Unix. 

## Table of Contents

- [File Transfer Protocol](#project-name)
  - [Table of Contents](#table-of-contents)
  - [Description](#description)
  - [Features](#features)
  - [Installation](#installation)
  - [Usage](#usage)
  - [Contributing](#contributing)
  - [References](#references)

## Description

This project is a simple implementation of a File Transfer Protocol (FTP) using socket programming in Unix. The FTP server and client are designed to enable the transfer of files between a server and a client over a network. Our implementation of FTP should follow protocol design of the RFC 959 FTP. Moreover, our FTP server should commnicate with FileZilla client. 

## Features

Our basic functionalities for FTP

- Log in
- Check current working directory
- Open passive mode
- Create new directory
- Listing all the files in the current working directory
- Upload files
- Delete files
- Downloading files
- Change working directory
- ...

## Installation

For installation, you should download our resouce, then running the following

For server:
```bash
cd server
gcc -o server server.c
./server
```
For client:
```bash
cd client
gcc -o client client.c
./client 127.0.0.1 12345
#listen to local host at port 12345
```
## Usage

Our FTP supplies these command: USER, PASS, LIST, PWD, CWD, RMD, MKD, PASV, STOR, RETR, DELE, QUIT.

## Contributing

1. Nguyen Trong Huy [huy.nt210451@sis.hust.edu.vn]
2. Tran Duc Nam [nam.td215228@sis.hust.edu.vn]

## References

```bibtex
@misc{rfc959,
    series =    {Request for Comments},
    number =    959,
    howpublished =  {RFC 959},
    publisher = {RFC Editor},
    doi =       {10.17487/RFC0959},
    url =       {https://www.rfc-editor.org/info/rfc959},
    title =     {{File Transfer Protocol}},
    pagetotal = 69,
    year =      1985,
    month =     oct,
    abstract =  {This memo is the official specification of the File Transfer Protocol (FTP) for the DARPA Internet community. The primary intent is to clarify and correct the documentation of the FTP specification, not to change the protocol. The following new optional commands are included in this edition of the specification: Change to Parent Directory (CDUP), Structure Mount (SMNT), Store Unique (STOU), Remove Directory (RMD), Make Directory (MKD), Print Directory (PWD), and System (SYST). Note that this specification is compatible with the previous edition.},
}
```
