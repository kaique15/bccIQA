# bccIQA

Índice de Qualidade da Água(IQA) - 1º Semestre(2016) BCC Senac.

Linux(somente):

Compilando:

Juntamente à interface gráfica:

Primeiramente é necessário ter o compilador gcc instalado, caso não tenha, abra o terminal e digite os seguintes códigos:

sudo apt-get update
sudo apt-get upgrade
sudo apt-get install build-essential
gcc -v
make -v
Após a instalação do compilador gcc, o próximo passo é instalar o GTK+3 utilizando o comando:

sudo apt-get install libgtk-3-dev
Entre na pasta gtk deste repositório utilizando o comando cd(exemplo: cd Desktop\bccIQA\gtk), estando dentro da pasta digite:

gcc -o CalculadoraIQA main.c `pkg-config --cflags --libs gtk+-3.0` -export-dynamic -lm
Por fim, digite ./CalculadoraIQA e preencha os valores adequados.

Sem interface gráfica:

Primeiramente é necessário ter o compilador gcc instaldo, caso não tenha, abra o terminal e digite os seguintes códigos:

sudo apt-get update
sudo apt-get upgrade
sudo apt-get install build-essential
gcc -v
make -v
Tendo o arquivo Makefile em mãos, abra o terminal. Com o terminal aberto, certifique-se em estar localizado na pasta onde contém os arquivos deste repositório, utilize o comando cd (exemplo: cd Desktop\bccIQA). Por fim digite o comando: make all, gerando assim o executável deste projeto.

Concluindo os passos anteriores, para executar o programa ainda no terminal, digite ./main e preencha as informações necessárias para se calcular o IQA.

Referências:

https://help.ubuntu.com/community/InstallingCompilers
