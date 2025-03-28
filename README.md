![run 3a server](https://github.com/user-attachments/assets/74160a84-6eaf-4dc6-a222-11980fe10ea5)# 3a.CREATION FOR ECHO CLIENT AND ECHO SERVER USING TCP SOCKETS
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
![run 3a server](https://github.com/user-attachments/assets/55786c20-4867-4d1c-937c-92c8f936098f)
![run 3a client](https://github.com/user-attachments/assets/3895a6db-10ee-4d6e-b3a5-1f988003a5c6)
![3aserver](https://github.com/user-attachments/assets/a161fbbd-32a9-438f-acc2-0aa398708892)
![3a client](https://github.com/user-attachments/assets/fc084f04-6515-4565-9a2f-e1191faa8eb3)


## RESULT
Thus, the python program for creating Echo Client and Echo Server using TCP Sockets Links 
was successfully created and executed.
