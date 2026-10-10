# TFTP Client-Server File Transfer Using C

## Project Overview

The Trivial File Transfer Protocol (TFTP) Client-Server project focuses on implementing file transfer between a client and a server using C programming and UDP socket programming in a Linux environment.

TFTP is a lightweight file transfer protocol that uses the User Datagram Protocol (UDP) to transfer files between devices over a network. Unlike FTP, TFTP does not establish a TCP connection or provide built-in authentication. It uses request, data, acknowledgment, and error packets to manage file transfers.

The objective of this project is to understand network programming, client-server communication, file handling, UDP sockets, and the fundamentals of protocol implementation in C.

## Objectives

- Understand client-server architecture and network communication.
- Implement UDP socket programming in C.
- Explore the working principles of the TFTP protocol.
- Perform file reading and writing using C file-handling functions.
- Understand request and acknowledgment mechanisms in network protocols.
- Develop debugging and troubleshooting skills in Linux.

## Technologies Used

- **Programming Language:** C
- **Operating System:** Linux / Ubuntu
- **Networking:** UDP Socket Programming
- **Compiler:** GCC
- **Concepts:** Client-Server Architecture, File Handling, Network Protocols, Error Handling

## Key Features

- Client-server application structure.
- UDP-based communication.
- File-transfer request handling.
- File reading and writing operations.
- Protocol packet processing.
- Error detection and troubleshooting concepts.

*Note: These are project objectives and intended features. Include only the features that are implemented and tested successfully in your source code.*

## How TFTP Works

1. **Request:** The client sends a read request (RRQ) to download a file or a write request (WRQ) to upload a file.
2. **Server Response:** The server processes the request and responds with data or an acknowledgment, depending on the operation.
3. **Data Transfer:** The file is transferred in data blocks.
4. **Acknowledgment:** The receiver acknowledges each data block.
5. **Completion:** The transfer ends when the final data block is received and acknowledged.

## TFTP Packet Types

- **RRQ:** Read Request — requests a file from the server.
- **WRQ:** Write Request — requests to send a file to the server.
- **DATA:** Contains a block of file data.
- **ACK:** Acknowledges receipt of a data block.
- **ERROR:** Reports a protocol or file-transfer error.

## Concepts Learned

- Creating and using UDP sockets.
- Sending and receiving data between client and server.
- File operations using C.
- Structuring a network programming project using source and header files.
- Understanding packet formats and protocol operations.
- Debugging network communication and handling errors.

## Project Structure

```text
TFTP-Client-Server/
├── server.c
├── tftp.c
├── client1.c
├── client2.c
├── header.h
├── tftp_client.h
├── README.md
└── .gitignore
```

## Compilation

Compile the server and client using GCC, adjusting the filenames and linked source files to match the functions defined in your project.

Example:

```bash
gcc -Wall -Wextra server.c tftp.c -o server
```

Compile the client using its required source files:

```bash
gcc -Wall -Wextra client1.c client2.c -o client
```

## Future Enhancements

- Complete and test file upload and download operations.
- Implement correct TFTP request, data, acknowledgment, and error packet formats.
- Add timeout and retransmission handling.
- Improve validation and error handling.
- Test transfers between separate systems on a network.
- Improve reliability and document test results.

## Author

**Vedavathi C M**

Electronics and Communication Engineering Graduate

GitHub: https://github.com/Vedavathi-c-m
