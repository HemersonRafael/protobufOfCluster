# protobufOfCluster

Processo de instalação do protobuf

Processe of protobuf install

Caso não tenha o zip e unzip instalados basta executar o comando:
If you do not have the zip and unzip installed just run the command:

sudo apt-get install zip unzip

Baixar e descompactar o protobuf:

Download and unpack the protobuf:

sudo -i
apt-get update
apt-get install dh-autoreconf
wget https://github.com/HemersonRafael/protobufOfCluster/archive/master.zip
unzip v2.5.0.zip
cd protobuf-2.5.0

Gere os arquivos de configuração da compilação:

Generate the build configuration files:

./autogen.sh
./configure --prefix=/usr


Compilação e instalação do protobuf:

Build and install protobuf:

make
make check
make install
