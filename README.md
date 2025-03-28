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
CLIENT:
import socket
s=socket.socket()
s.connect(('localhost',8000))
while True:
 msg=input("Client > ")
 s.send(msg.encode())
 print("Server > ",s.recv(1024).decode())
SERVER:
import socket
s=socket.socket()
s.bind(('localhost',8000))
s.listen(5)
c,addr=s.accept()
while True:
 ClientMessage=c.recv(1024).decode()
 c.send(ClientMessage.encode())
```
## OUPUT
![3a client](https://github.com/user-attachments/assets/ea3d9ad1-bc03-4ae5-ba1f-f4f9db4d2712)
![3aserver](https://github.com/user-attachments/assets/9c9280b5-053a-4709-806f-ee9520f7391f)
![run 3a client](https://github.com/user-attachments/assets/d0a29bb4-ec3e-454a-b84a-b80d25559e48)
![run 3a server](https://github.com/user-attachments/assets/37735eda-ba65-4584-8783-fa4f9bbe322f)

## RESULT
Thus, the python program for creating Echo Client and Echo Server using TCP Sockets Links 
was successfully created and executed.
