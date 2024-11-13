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
