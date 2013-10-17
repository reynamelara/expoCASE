#encoding:utf-8
import socket  
  
s = socket.socket()   
s.bind(("localhost", 8000))  
s.listen(1)  
  
sc, addr = s.accept()  
  
while True:  
      recibido = sc.recv(1024)  
      if recibido == "salir":  
         break        
      print "Recibido:", recibido  
      sc.send(recibido)  
  
print "adios"  
  
sc.close()  
s.close() 