# Multicasting-multimedia-over-IP
A repository containing an Internet Television application that uses multicast on live-streaming of data using TCP and UDP socket programming.

It is an Internet Television application where the client establishes a control channel using TCP socket and receives multimedia streams over a UDP socket. User can pause, restart, change the channel and even terminate the channel. To perform these tasks and to make user interactive, GUI based application is made.

SERVER FOLDER

  server.c file (TCP code to send station info and site info) 
	1) To Compile: gcc server.c
	2) To Run    : ./a.out

  station1.c file (UDP code for station 1)
	1) To Compile: gcc station1.c
	2) To Run    : ./a.out 239.192.4.1

  station2.c (UDP code for statiion 2)
	1) To Compile: gcc station2.c
	2) To Run    : ./a.out 239.192.4.2

CLIENT FOLDER

  client.c file (TCP code to recieve station info and site info)
	1) To Compile: gcc `pkg-config --cflags gtk+-3.0` -o client client.c `pkg-config --libs gtk+-3.0`
	2) To Run    : sudo ./client <IP-ADDRESS of the server>

  receiver.c file (UDP code to receive data)
	--> Compiled and executed by the client.c file.


