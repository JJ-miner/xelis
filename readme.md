Hello les miner de xelis
Voici comment lancer un node sur linux dans votre shell tapez les commandes suivante:

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

Pour miner sur hiveos 
