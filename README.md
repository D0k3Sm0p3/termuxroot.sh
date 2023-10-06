# termuxroot.sh
bash command to get android mobile root access using Termux App


#!/bin/sh

# Instale os pacotes necessários
apt update
apt install -y proot su-root

# Obtenha o binário SuperSU
wget https://github.com/Chainfire/SuperSU/releases/download/v2.8.9/supersu-v2.8.9.zip
unzip supersu-v2.8.9.zip

# Execute o SuperSU
proot -S su-root /data/data/com.chainfire.supersu/files/su
