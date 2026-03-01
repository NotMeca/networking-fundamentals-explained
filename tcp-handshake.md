# TCP 3-Way Handshake

## What is TCP?

TCP (Transmission Control Protocol) is a reliable, connection-oriented protocol used to establish communication between two devices.

## Purpose of the Handshake

The TCP 3-way handshake ensures:

- Both devices are reachable
- Sequence numbers are synchronized
- The connection is reliable

## The 3 Steps

1. SYN  
Client sends SYN packet to server to initiate connection.

2. SYN-ACK  
Server responds with SYN-ACK to acknowledge request.

3. ACK  
Client sends ACK to confirm connection establishment.

## Why This Matters in SOC

Security analysts monitor:

- Unusual SYN floods (DoS attacks)
- Repeated incomplete handshakes
- Suspicious outbound connections

## Wireshark Observation

In my capture:

- First packet: SYN
- Second packet: SYN-ACK
- Third packet: ACK

<img width="1044" height="49" alt="Screenshot 2026-03-01 172344" src="https://github.com/user-attachments/assets/4b83893c-4822-4d47-9e9a-086c44ea42e6" />

## Captured TCP 3-Way Handshake (Wireshark)

Client IP: 192.168.10.25  
Server IP: 184.28.9.100  
Client Port: 50759 (ephemeral port)  
Server Port: 80 (HTTP)

Step 1: Client sends SYN to initiate connection.  
Step 2: Server responds with SYN-ACK.  
Step 3: Client sends final ACK to establish connection.

The connection is successfully established after packet 107.
