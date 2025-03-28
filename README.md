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
s.bind(('localhost', 8000))
s.listen(5)

c, addr = s.accept()

while True:
    ClientMessage = c.recv(1024).decode()
    c.send(ClientMessage.encode())
import socket

s = socket.socket()
s.connect(('localhost', 8000))

while True:
    msg = input("Client > ")
    s.send(msg.encode())
    print("Server > ", s.recv(1024).decode())

```

## OUPUT
![run 3a server](https://github.com/user-attachments/assets/a748f4b9-949c-4e92-bab0-4a5e9fc292e8)
![run 3a client](https://github.com/user-attachments/assets/4830ef46-298a-474b-8d78-a14f9ea878a2)
![3aserver](https://github.com/user-attachments/assets/34dd885d-7276-4443-9155-e3d7c1336b87)
![3a client](https://github.com/user-attachments/assets/897b57e4-2b17-4455-9ace-5b14bf54232c)

## RESULT
Thus, the python program for creating Echo Client and Echo Server using TCP Sockets Links 
was successfully created and executed.
