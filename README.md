# Linux-programas-processos-pacotes

## Listar processos do terminal

````
ps
````

## Listar todos processos 

````
ps -e
````

## Listar todos processos com detalhes

````
ps -ef
````

## Listar por nome processos com detalhes

````
ps -ef | grep NomeDoPrograma
````

## Pesquisar dentro de um arquivo

````
grep California google.txt
````

## Encerrar um processo de id 16546

````
kill 16546
````

## Encerrar bruscamente um processo de id 16546

````
kill -9 16546
````

## Consumo de memória por processo

````
top
````

## Encerrar processos por nome 

````
killall NomeDoPrograma
````
ou
````
killall -9 NomeDoPrograma
````

## Ver os processos que estão pausados ou sendo executados em segundo plano no bash em que estamos

````
jobs
````

## Visualizar essa árvore de processos

````
pstree
````

## Executando e alterando arquivo

Usando gedit para criar um script de nome "dorme"

````
gedit dorme &
````

Criando um script

````
echo "Vou dormir"
sleep 5
echo "Terminei de dormir"
````

Executando com sh

````
sh dorme
````

Liberar execução por qualquer um

````
chmod +x dorme
````

Executando depois de liberar

````
./dorme
````

## Mostrar pasta que está instalado um programa(firefox)

````
 which firefox
````

## Mudar senha do usuário atual

````
passwd
````

## Mudar de usuário

````
su nomeusuario
````

Mudando para usuário root

````
su root
````

## Criar um usuário chamado jose

````
adduser jose
````

## Dar aos outros usuários o poder de ler e executar em um diretório jose

````
chmod o-rx jose
````

## Executar um arquivo globalmente só para um usuário(exmplo para guilherme)

Dentro do diretório workspace vamos criar um novo programa chamado oi, entraremos no diretório usando o comando cd e abriremos o gedit em background:

````
cd workspace
gedit oi &
````

Digitar dentro do arquivo:

````
echo "Oi, tudo bem?"
````

Permitir execução

````
chmod +x oi
````

Editar o arquivo para configurar variável global

````
gedit .bashrc &
````

Adicionar uma linha:

````
PATH=$PATH:/home/guilherme/workspace
````

Consultar variáveis de ambiente:

````
env
````

## Atualizar programas

````
sudo apt-get update
````

## Pesquisar programas de servidores ftp

````
apt-cache search ftp
````

## Instalar servidor ftp

````
sudo apt-get install vsftpd
````

## Remover servidor ftp

````
sudo apt-get remove vsftpd
````

## Instalando pacote baixado

````
sudo dpkg -i vsftpd-dbg_3.0.3-12+b1_amd64.deb
````

## Remover pacote

````
sudo dpkg -r [nome do pacote]
````
````
sudo dpkg -r vsftpd
````
