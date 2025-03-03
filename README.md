# Echoserver
Echo server and client using python socket

# AIM:

To develop a simple webserver to serve html programming pages.

## DESIGN STEPS:

### Step 1:

Design of echo server and client using python socket

### Step 2:

Implementation using Python code

### Step 3:

Testing the server and client 

## PROGRAM:
##client
```
import socket
HOST, PORT = '127.0.0.1', 65432
with socket.create_connection((HOST, PORT)) as s:
    s.sendall(b'gokul prakash m, 212223240041')
    print(f'Received: {s.recv(1024)!r}')
```
##server
```
import socket
host,port='127.0.0.1',65432
with socket.create_server((host,port))as s:
    conn,addr=s.accept()
    with conn:
        print(f'connected by {addr}')
        while data :=conn.recv(1024):
            conn.sendall(data)
```


## OUTPUT:
![image](https://github.com/user-attachments/assets/d94b3bff-491e-4c87-978f-76f75b54cd2c)


## RESULT:
The program is executed successfully
