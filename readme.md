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


