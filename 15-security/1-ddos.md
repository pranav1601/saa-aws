## ddos

- distributed denial oof service
- make the website unable to users
- -large packet floods, using combnation of reflection and amplification techniques or by using large botnets

## layer 4 ddos

- SYN flood - works on tcp
- tcp 3 way handshake - client sends server syn, server sends back syn-ack, client sends back ack

## syn floods - 

- overwhelm a server by sending large number os SYN, sends back syn ACK but cliens ignores. Resources of server keep waiting for ack response which never comes
- pprevents legitiemate client

## amplification attack

- ntp, ssdp, dns, chargen, snmp
- send a third party server a request using spooefed ip address
- server will then respond to the request with a greater payload than the inital request to the spoofed ip address
- this means that if attacker sends a packet wth a spoofed ip address of 64 bytes, ntp serrver would respond with up to 3456 bytes of traffic
- attackers can coordinate this and use mulitple ntp server a second to send legitimate ntp traffic to the target

## layer 7 atttack

- flood of get/post requests

> 