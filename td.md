# TD4 Iperf
#### 1.

Je crée tout d'abord une VM.
J'installe les paquets nécessairres, soit "iperf".

Je prends les 2 scripts disponibles sur le moodle, le premier créant deux interfaces virtuelles en ethernet (Veth) et le deuxième permettant de troubler le réseau interne.

Je lance alors iperf sur ma VM avec la commande donnée : 

./simul.sh 10.12.0.1 10.12.0.2'iperf -B 10.12.0.1 -s'
On voit que le serveur s'est bien lancé.

Je fais un show de mes interfaces réseau pour voir mes cartes 

-> Je ne vois que le carte client, mais qui est bien en 10.12.0.2
Et si je lance un iperf -c (client) sur le serveur (10.12.0.1), il se connecte bien. 





