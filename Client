import socket

s = socket.socket(socket.AF_INET,socket.SOCK_STREAM)

s.connect(("127.0.0.1",5555))

while True:
        data = str(input("Client >>"))
        edata = bytes(data,encoding='utf-8')
        s.send(edata)

        rdata = s.recv(1024)
        rdata = rdata.decode('utf-8')
        print("Recieved : ", rdata)
