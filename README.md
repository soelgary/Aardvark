The first thing we did when writing the code for this project was work on producing valid packets. We spent a lot of time sending packets over the network and sniffing them with wireshark to ensure we can build valid packets. The next step was to actually get the handshake working. For the handshake, we ran into difficulties because we weren't getting responses from the syn, then when we finally got it working, we were getting retransissions of the syn/ack when we sent an ack. After the handshake was working we worked on the http part and sending/receiving data. The biggest issue we ran into here was noticing dropped packets and reordering received packets.