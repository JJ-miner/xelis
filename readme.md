JJ-TEAM DE JEANJEANLABRICOLE

https://discord.gg/MAn8QdFS

https://www.youtube.com/watch?v=NLYhvbqVWuo

Hello les mineurs de xelis

Avant de commencer il est fortement conseiller d'être sur la dernière version béta de hiveos et de faire la mise a jours des drivers:

`hive-replace --beta`

répondez yes

`nvidia-driver-update`

vous aurez besoin des apps suivante si elles ne sont pas déja installé:

`apt install screen`

`apt install ntpdate`


Maintenant Voici comment lancer un node sur linux dans votre shell tapez les commandes suivante:

`mkdir xelis`

`cd xelis`

`wget https://github.com/xelis-project/xelis-blockchain/releases/download/v1.9.2/x86_64-unknown-linux-gnu.tar.gz`

`tar -xf x86_64-unknown-linux-gnu.tar.gz`

`rm x86_64-unknown-linux-gnu.tar.gz`

`cd x86_64-unknown-linux-gnu`

`screen -S node-xelis ./xelis_daemon --allow-boost-sync`


Pour vérifier que notre node est synced nous allons sur https://explorer.xelis.io/ on regarde le dernier block 

![image](https://github.com/JJ-miner/xelis/assets/167770964/92983b4f-ef56-417f-8bb7-57f326dc0b42)




cela concorde notre node est bien synced 



![image](https://github.com/JJ-miner/xelis/assets/167770964/165249c4-b06f-4dee-a4fc-937791ea0e06)

si vous avez une erreur :

![image](https://github.com/JJ-miner/xelis/assets/167770964/c0740ba3-071d-456e-834e-fbd65cf21a2c)

lancez la commande :

`ntpdate -s pool.ntp.org`

Maintenant le wallet

tapez les touches:

`ctrl + a + d`

cela detache le screen en laissant le node tourné pour y retourné il suffira de taper 

`screen -r node-xelis`

tapez la commande:

`cd xelis/x86_64-unknown-linux-gnu`

`screen -S wallet-xelis ./xelis_wallet`


![image](https://github.com/JJ-miner/xelis/assets/167770964/4dab90ad-ed44-4d2b-ab16-c4d79a419f22)


tapez :

`create`


![image](https://github.com/JJ-miner/xelis/assets/167770964/478e2433-7779-4294-a923-db1efdfe59c7)


tapez le nom du wallet que vous désirez ici teamjj:


![image](https://github.com/JJ-miner/xelis/assets/167770964/e2ed3876-4933-431e-850b-c6bc4716b17d)


puis choisissez votre mdp qui vous faudra entrer deux fois:


![image](https://github.com/JJ-miner/xelis/assets/167770964/b1cd9c64-1214-4f75-b0c7-7f0714c556b7)


![image](https://github.com/JJ-miner/xelis/assets/167770964/2b553e7c-4e79-4d5a-a142-3d1ce0320543)


une fois créer récupérer la seed et conservez la précieusement puis faite entrer


![image](https://github.com/JJ-miner/xelis/assets/167770964/c0651825-3a11-47ab-84e5-6ec557040d7a)


![image](https://github.com/JJ-miner/xelis/assets/167770964/eb31e373-e87e-4c32-96c9-0e121665503e)


maintenant tapez:

`display_address`


![image](https://github.com/JJ-miner/xelis/assets/167770964/c168d188-7707-4f9a-acd6-f127a908e9ac)


vous obtiendrez votre address 


![image](https://github.com/JJ-miner/xelis/assets/167770964/4b809607-9566-4e78-901a-2999ddf00a74)

maintenant on ferme le screen comme pour le node

`ctrl + a + d`

Pour miner sur hiveos :


version xelis_miner-v1.9.2e.tar.gz utilise le miner xelis-taxminer

Nous ne sommes pas les dev du miner xelis-taxminer il y a 10% de fee 

Nous avons juste adapté le miner dans un custom pour hiveos

c'est une version béta 

Pour dual miner


![image](https://github.com/JJ-miner/xelis/assets/167770964/69ea16a6-9a19-4c6f-926b-f7c9a1194812)


Pour miner juste GPU

Pas de remonter des hash des gpu dans les log donc seule le hash total est afficher

![image](https://github.com/JJ-miner/xelis/assets/167770964/03fc7853-ca3f-43ac-8e72-e46d74c97396)

il est possible d'utiliser nvtool 

![image](https://github.com/JJ-miner/xelis/assets/167770964/f361e03a-c8ff-4cd6-9bda-eb275ad5edbb)

Pour miner juste CPU

![image](https://github.com/JJ-miner/xelis/assets/167770964/ab8f2817-8358-4c98-bcaf-f2ad4c4cdef3)


Attention compatible uniquement avec les cpu avx2 ou supérieur


Nb: si vous ne mettez pas de worker_name le nom du par défaut sera "default"

en cas d'erreur :

![image](https://github.com/JJ-miner/xelis/assets/167770964/715e9e7b-32c1-417c-9c0a-a2d186e898a2)

lancez :sudo 

`cp /etc/apt/sources.list /etc/apt/sources.list.backup`

`echo "deb http://cz.archive.ubuntu.com/ubuntu jammy main" >> /etc/apt/sources.list && apt update && apt install libc6`

`rm /etc/apt/sources.list && cp /etc/apt/sources.list.backup /etc/apt/sources.list`

Calculez vos gains potentiels:

https://explorer.xelis.io/mining-calculator

rejoignez nous sur le discord de JJ

https://discord.gg/MAn8QdFS


