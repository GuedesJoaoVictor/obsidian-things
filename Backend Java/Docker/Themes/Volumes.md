
## O que são?
São uma solução para a persistência de dados de forma nativa pelo docker
## Quais os objetivos?
Os objetivos são bem diversos, você pode querer manter os dados de um banco de dados, compartilhamento de dados entre containers. 

São utilizados também arquivos de logs, para que quando um erro seja lançado, não se perca a causa do erro caso o sistema fique funcionando por muito tempo ou pelo container ser excluído, etc.

## Tipos de volumes
1. Volume *anônimo*. Normalmente iniciado com a tag -v (sem nome específico)
2. Containers *Nomeados*. Para melhor orquestração dos containers.
3.  **Bind Mounts**.  Tira o total gerenciamento do docker, fazemos um bind com o nosso filesystem. (Pode ser util para logs para que eles sejam armazenados em uma pasta do computador host)

