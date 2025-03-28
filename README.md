# 3a.CREATION FOR ECHO CLIENT AND ECHO SERVER USING TCP SOCKETS
# AIM
To write a python program for creating Echo Client and Echo Server using TCP
Sockets Links.
## ALGORITHM:
1. Import the necessary modules in python
2. Create a socket connection to using the socket module.
3. Send message to the client and receive the message from the client using the Socket module in
 server .
4. Send and receive the message using the send function in socket.
## PROGRAM
```
import socket

s = socket.socket()
s.connect(('localhost', 8000))

while True:
    msg = input("Client > ")
    s.send(msg.encode())
    print("Server > ", s.recv(1024).decode())
import socket

s = socket.socket()
s.bind(('localhost', 8000))
s.listen(5)

c, addr = s.accept()

while True:
    ClientMessage = c.recv(1024).decode()
    c.send(ClientMessage.encode())
```
## OUPUT
![3a client](https://github.com/user-attachments/assets/434768e9-9fbb-4fbf-afbc-ee7d421043d3)
![3aserver](https://github.com/user-attachments/assets/5892500d-f5bf-4b31-bffd-3b272865d93d)
![run 3a client](https://github.com/user-attachments/assets/2811f8fb-82d8-48f1-8ecb-48e0fb61a6c8)
![run 3a server](https://github.com/user-attachments/assets/09efc290-d108-4195-b441-2218e9fb6c1a)

## RESULT
Thus, the python program for creating Echo Client and Echo Server using TCP Sockets Links 
was successfully created and executed.
