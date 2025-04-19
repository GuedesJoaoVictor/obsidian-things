# [[Short Cuts]]

docker image ls - lista imagens locais

docker run image ${nome} - roda a imagem, baixa caso não tenha sido localizada

docker pull ${nome} - baixa a imagem do docker hub para ser usada localmente.

docker container ls - lista os containers sendo utilizados **atualmente**.

docker container ls -a - lista **todos** os containers.

docker container  run -p 5555:5555 - faz com que tudo o que esteja sendo rodado na porta 5555 do container seja  redirecionada para a máquina local.

*Como fazer um container continuar sendo executado?*
O docker é manipulado por meio de flags, então usaremos uma flag para que isso possa ser possível.

Ex: docker container run -i (interativo) -t (abre a instancia de um terminal para ser usado localmente) ubuntu

ou pode ser usado assim também: docker container run -it ubuntu

já o comando: docker container stop, é usado para "**desativar**" um container. devendo passar como argumento para o comando, o id do container.
Ex: docker container stop 5a47ac248759 - sendo essa numeração o id do container.

# [[Flags]]

docker run --name - escolhemos o *nome* do container para rodar 
docker run -d - faz com que o docker **libere** o nosso terminal para que  rode em segundo plano a imagem.

---
O comando docker run **sempre** lança um novo container.
--
docker logs nome_do_container - mostra os últimos *logs* do container.

docker run nome da imagem -p porta : porta - faz com que a nossa porta **local** da máquina escute o que está acontecendo na porta do container **docker**

docker tag <id_imagem> <nome_imagem>:<tag_imagem>

docker build  -t <nome:tag> .

docker system prune -a

# [[Volumes]]

## O que são?
São uma solução para a persistência de dados de forma nativa pelo docker
## Quais os objetivos?
Os objetivos são bem diversos, você pode querer manter os dados de um banco de dados, compartilhamento de dados entre containers. 

São utilizados também arquivos de logs, para que quando um erro seja lançado, não se perca a causa do erro caso o sistema fique funcionando por muito tempo ou pelo container ser excluído, etc.

## Tipos de volumes
1. Volume *anônimo*. Normalmente iniciado com a tag -v (sem nome específico)
2. Containers *Nomeados*. Para melhor orquestração dos containers.
3.  Bind Mounts