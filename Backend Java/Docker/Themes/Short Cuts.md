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
