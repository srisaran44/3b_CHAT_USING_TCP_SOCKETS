# 3b.CREATION FOR CHAT USING TCP SOCKETS
## AIM
To write a python program for creating Chat using TCP Sockets Links.
## ALGORITHM:
1. Import the necessary modules in python
2. Create a socket connection to using the socket module.
3. Send message to the client and receive the message from the client using the Socket module in
 server
4. Send and receive the message using the send function in socket.
## PROGRAM

## CLIENT.PY:
<img width="1099" height="580" alt="Screenshot 2026-05-19 131232" src="https://github.com/user-attachments/assets/a818606d-8225-4bce-b8c4-ac196cb15f81" />
## SERVER.PY:
import socket
s=socket.socket()
s.bind(('localhost',8009))
s.listen(5)
c,addr=s.accept()
while True:
 ClientMessage=c.recv(1024).decode()
 print("Client > ",ClientMessage)
 msg=input("Server > ")
 c.send(msg.encode())


## OUPUT
<img width="870" height="671" alt="Screenshot 2026-05-19 114907" src="https://github.com/user-attachments/assets/2a9d8a27-ef6d-44a1-865a-640998cbb298" />

## RESULT
Thus, the python program for creating Chat using TCP Sockets Links was successfully 
created and executed.
