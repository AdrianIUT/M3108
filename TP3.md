# TP3/4 Netflow

J'installe FProbe. Je modifie ensuite son fichier de configuration pour mettre les IP et les ports de chaque poste.

Je clone le repository git donné. Je fais ensuite : 

```docker-compose up -d nfsen```

Je me met dans le dossier git au préalable.

Je rentre dans le fichier data/nfsen/etc/nfsen.conf (Dans le container docker)(Dans la partie %sources)data

'Joris' => { 'port' => '1551', 'col' => '#50B719', 'type' => 'netflow' },
'Edouard' => { 'port' => '1552', 'col' => '#50B719', 'type' => 'netflow' },
'Oriane' => {'port'=>'1553','col'=>'#50B719','type'=>'netflow'},
'Moi' => {'port'=>'1554','col'=>'#50B719','type'=>'netflow'},
'Flavien' => {'port'=>'1556','col'=>'#50B719','type'=>'netflow'},
'Bastien' => {'port'=>'1557','col'=>'#50B719','type'=>'netflow'},
'Maxime' => {'port'=>'1666','col'=>'#50B719','type'=>'netflow'},
 
Je rentre dans le navigateur ```10.214.0.116:6080/nfsen```

Je vois sur les graphes une barre 
Je clique sur le graphe en question et je vois que c'est mon traffic
