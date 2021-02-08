import socket

sock = socket.socket(socket.AF_INET,socket.SOCK_STREAM)
sock.bind(("127.0.0.1",5555))
sock.listen(1)
print("Waiting for Connection....\n")


while True:
    conn, add = sock.accept()
    print("Connection From ", add)
    while True:
        rdata = conn.recv(1024)
        d_data = rdata.decode('utf-8')
        if not d_data:
                break
        else:
                print(d_data)
                sdata = str(input("Server :"))
                e_sdata = bytes(sdata,'utf-8')
                conn.send(e_sdata) # send fuction accept only data in bytes :)
