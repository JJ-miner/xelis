Hello les miner de xelis
Voici comment lancer un node sur linux dans votre shell tapez les commandes suivante:

screen
mkdir xelis
cd xelis
wget https://github.com/xelis-project/xelis-blockchain/releases/download/v1.9.1/x86_64-unknown-linux-gnu.tar.gz
tar -xf x86_64-unknown-linux-gnu.tar.gz
rm x86_64-unknown-linux-gnu.tar.gz
cd x86_64-unknown-linux-gn
./xelis_daemon  --allow-boost-sync


Pour vérifier que notre node est synced nous allons sur https://explorer.xelis.io/ on regarde le dernier block 

![image](https://github.com/JJ-miner/xelis/assets/167770964/92983b4f-ef56-417f-8bb7-57f326dc0b42)




cela concorde notre node est bien synced 



![image](https://github.com/JJ-miner/xelis/assets/167770964/165249c4-b06f-4dee-a4fc-937791ea0e06)


Maintenant le wallet
tapez les touches:
ctrl + a + c

cela ouvre une nouvelle fenètre screen
tapez la commande:
./xelis_wallet


![image](https://github.com/JJ-miner/xelis/assets/167770964/4dab90ad-ed44-4d2b-ab16-c4d79a419f22)


tapez :
create


![image](https://github.com/JJ-miner/xelis/assets/167770964/478e2433-7779-4294-a923-db1efdfe59c7)


tapez le nom du wallet que vous désirez ici teamjj:


![image](https://github.com/JJ-miner/xelis/assets/167770964/e2ed3876-4933-431e-850b-c6bc4716b17d)


puis choisissez votre mdp qui vous faudrat entrer deux fois:


![image](https://github.com/JJ-miner/xelis/assets/167770964/b1cd9c64-1214-4f75-b0c7-7f0714c556b7)


![image](https://github.com/JJ-miner/xelis/assets/167770964/2b553e7c-4e79-4d5a-a142-3d1ce0320543)


une fois créer récuprer la seed et conservez la précieusement puis faitre entrer


![image](https://github.com/JJ-miner/xelis/assets/167770964/c0651825-3a11-47ab-84e5-6ec557040d7a)


![image](https://github.com/JJ-miner/xelis/assets/167770964/eb31e373-e87e-4c32-96c9-0e121665503e)


maintenant tapez:
display_address


![image](https://github.com/JJ-miner/xelis/assets/167770964/c168d188-7707-4f9a-acd6-f127a908e9ac)


vous obtiendrez votre address 


![image](https://github.com/JJ-miner/xelis/assets/167770964/4b809607-9566-4e78-901a-2999ddf00a74)


Pour miner sur hiveos :


![image](https://github.com/JJ-miner/xelis/assets/167770964/9328cee6-8e3b-4e73-93ba-b026fd93db5b)


Nb: si vous ne mettez pas de worker_name le nom du par défaut sera "default"
ENJOY!!
