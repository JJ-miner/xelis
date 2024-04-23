Hello les miner de xelis

Avant de commencer il est fortement conseiller d'être sur la dernière version béta de hiveos:

`hive-replace --beta`

répondez yes

vous aurez besoin des apps suivante si elles ne sont pas déja installé:

`apt install screen`

`apt install ntpdate`


Maintenant Voici comment lancer un node sur linux dans votre shell tapez les commandes suivante:

`screen`

`mkdir xelis`

`cd xelis`

`wget https://github.com/xelis-project/xelis-blockchain/releases/download/v1.9.2/x86_64-unknown-linux-gnu.tar.gz`

`tar -xf x86_64-unknown-linux-gnu.tar.gz`

`rm x86_64-unknown-linux-gnu.tar.gz`

`cd x86_64-unknown-linux-gnu`

`./xelis_daemon --allow-boost-sync`


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

`ctrl + a + c`

cela ouvre une nouvelle fenêtre screen

tapez la commande:

`cd xelis/x86_64-unknown-linux-gnu`

`./xelis_wallet`


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


Pour miner sur hiveos :


![image](https://github.com/JJ-miner/xelis/assets/167770964/9328cee6-8e3b-4e73-93ba-b026fd93db5b)


Nb: si vous ne mettez pas de worker_name le nom du par défaut sera "default"

en cas d'erreur :

![image](https://github.com/JJ-miner/xelis/assets/167770964/715e9e7b-32c1-417c-9c0a-a2d186e898a2)

lancez :sudo 

`cp /etc/apt/sources.list /etc/apt/sources.list.backup`

`echo "deb http://cz.archive.ubuntu.com/ubuntu jammy main" >> /etc/apt/sources.list && apt update && apt install libc6`

`rm /etc/apt/sources.list && cp /etc/apt/sources.list.backup /etc/apt/sources.list`
