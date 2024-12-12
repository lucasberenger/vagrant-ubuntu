# Criação de VM Ubuntu 20.04 com Synced Folder

## Objetivos do projeto:
1. Praticar a criação de ambientes de virtualização utilizando Vagrant.
2. Configurar uma máquina virtual com Ubuntu 20.04, ajustando parâmetros de rede, CPU e memória.
3. Sincronizar pastas entre o host e a máquina virtual.

## Descrição
O Vagrantile configura a máquina virtual com o nome de "Ubuntu-01", utilizando 1GB de memória e 1 CPU. Além disso, sincroniza a pasta hello/, que contém o arquivo hello.txt, com o diretório /home/vagrant/hello, que será criado quando a máquina virtual for iniciada.

## Passo a passo para rodar a VM

1. Certifique-se de ter instalado em sua máquina local o [VirtualBox](https://www.virtualbox.org/) e o [Vagrant](https://www.vagrantup.com/).
2. Clone o repositório e acesse a sua pasta com o terminal.
3. Antes de iniciar o projeto, é necessário alterar o nome da sua placa de rede (parâmetro 'bridge' dentro do Vagrantfile).
4. Feito isso, inicie a máquina virtual utilizando o comando ``` vagrant up ``` em seu terminal.
5. Uma vez iniciada, realize o acesso via ssh com o comando ``` vagrant ssh ```.
6. Para conferir se a pasta hello/ se encontra na máquina virtual, passe o comando ``` ls ``` ou ``` cat hello/hello.txt``` para ver o conteúdo do arquivo de texto no terminal.

