PDF Aula 1 -  [[REDES Introducao 1.pdf]]

![[REDES Introducao 1.pdf]]

> Camadas
* Aplicação
* [[Transporte]] - faz o parse dos dados ([[Pacotes]]) e manda para aplicação
* Rede - Literal uma rede de conexão
* [[Enlace]] / Fisico - Utiliza protocolos.


serviços de comunicação fornecidos às aplicações: 
– entrega de dados confiável da origem ao destino - Forma mais segura, para tudo ao perder um pacote
– entrega de dados pelo “melhor esforço” (não confiável) - Exemplo de jogos, não é o mais seguro, mas funciona pois assim eu consigo ver mais rápido o inimigo, ou seja, recebo os pacotes de forma mais rápida. 

Com isso pode ocorrer congestionamento dos pacotes. Os roteadores podem estar recebendo muitos pacotes e não está conseguindo passar esses pacotes na Entrada/Saida

**Desvantagens de usar rede**

* Ataques de vírus pois podem ser espalhados pelas redes
* Eventuais problemas com o dispositivo da rede, tal como: HUB, switch, roteadores, etc.
* Invasão de hackers.

	Revisão

1. Cite sete recursos que podem ser compartilhados em uma rede.
Voz, video, imagens, redes, malwares, pastas, textos, etc.

2. Qual a diferença entre um hospedeiro e um sistema final? Cite os tipos de sistemas finais. Um servidor web é um sistema final?
Nenhuma. Sim, é um sistema final (host, hospedeiro) pois ele é a finalidade da requisição.

3.  Cite vantagens e desvantagens e desvantagens do uso de redes.
As vantagens são absurdas, como por exemplo a Internet que nos possibilita trocar dados com alguém de outro lado do mundo. As desvantagens é que esses dados podem ser mal intencionados como vírus.

4.  O que é a WWW. Qual sua relação com a internet?
A WWW (World Wide Web) é um sistema distribuído, que funciona na Internet.

5. O que é a internet? Comente somente a sua origem e evolução.
A Internet é uma rede de redes, onde trafegam todos os dados, pacotes, etc. Começou como a ARPANET contendo emails, logon remoto e tranferencia de arquivos, que ao longo do tempo foi evoluindo, adotando protocolos como o TCP, IP e ficando mais robusta no sentido de conectar globalmente os usuários.

PDF Aula 2 - [[REDES Introducao 2.pdf]]

Ao escolher um provedor de internet, ele vai lhe dar permissão para usar a *rede de acesso*  deles.

* Sistemas finais (hospedeiros)
	* Executar programas de aplicação.
	* Estão na borda da rede.

* Modelo cliente/servidor
	* hospedeiro cliente solicita, recebe serviço de servidor sempre ativo
	*  p. e. navegador/servidor Web; cliente/servidor de e-mail

* Modelo peer to peer
	* Uso mínimo (ou nenhum) de servidores dedicados
	* p. e. Skype, BitTorrent

Meios de acesso  a internet:
* DSL
Era um par trançado de fios em que era usado para o telefone que também servia para conectar a internet.

* Modens a cabo
Não usa infraestrutura de telefone, mas sim a de tv a cabo.
HFC: Hybrid Fiber Coax
rede de cabo e fibra conecta  casas ao roteador ISP
 -Casas compartilham acesso ao roteador
  -diferente de DSL, que tem acesso dedicado

Canal: Forma de pedir um meio físico.

* Ethernet
normalmente usado em empresas, universidades, etc.
Roteador > Switch > Computadores.

> Redes residenciais, o que normalmente temos.

* modem DSL ou a cabo
* roteador/firewall/NAT(network address translation)
* Ethernet
* ponto de acesso sem fio

O modem traduz os pacotes para como você recebe (por protocolos) a internet, exemplo:
Pacote > Fibra óptica

[[Topologia de Rede]]

* [[Full Mesh]]
* [[Interconexão Parcial]]
