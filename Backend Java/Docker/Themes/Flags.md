
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
