# Planejamento de Rede

## Objetivo

O objetivo deste projeto foi utilizar todos os conhecimentos de rede passados pela Escola SENAI de informática para planejar e montar uma rede com as seguintes caracteristicas:

* Protocolos IPv4 e IPv6 em um esquema de pilha dupla
* Divisão de sub-redes
* Criação de vlans de suas respectivas redes
* Rota padrão no roteador
* Conexão via SSH
* Configurações básicas de switchs e roteador

## Rede

Neste projeto utilizamos um **ip de classe C**: 192.168.0.0 e um **IPV6**: 2001:db8:cafe:1::/64 e dividimos esse ip em sub-redes para uma melhor segurança e trafégo da rede sendo as sub-redes:

![Alt Text](https://i.ibb.co/kBdP17f/sub-redes.png)

A rede também foi dividida em 7 vlans (com a vlan nativa) seguindo a imagem abaixo:

![Alt Text](https://i.ibb.co/phVxkj2/vlan.png)


## Computadores

Cada computador está configurado com seus próprios ips estáticos, com um gateway padrão de cada rede e dns-server que já foi pré montado e sua mascará de rede de acordo com a sua sub-rede, conforme a imagem abaixo:

![Alt Text](https://i.ibb.co/zR9tBgD/Computadores.png)

Os computadores estão atrelados a um switch da sua respectiva rede, utilizando mode access em suas interfaces segue uma imagem da topologia abaixo:

![Alt Text](https://i.ibb.co/ByW3419/imagem-2021-02-02-165504.png)

## Switchs 

Cada Switch foi configurado com banner, senha na console e na enable, criadas suas respectivas vlans, adicionado as suas portas mode access e trunk e um dominio para acessar 
o site contido no server HTTP. Todos os Switchs se encontram em um switch core referente a imagem abaixo: 

![Alt Text](https://i.ibb.co/mqrZXtJ/imagem-2021-02-02-170306.png)


## Roteador e Rota Padrão

No roteador foram feitas as mesmas configurações padrões feitas no switch mas temos a adição de uma rota padrão que na topologia a rota padrão é o SRV-CLOUD e também utilizamos um método chamado rout-on-a-stick onde criamos sub-interfaces para cada vlan na rede conforme a imagem abaixo:

![Alt Text](https://i.ibb.co/fkRB4qg/imagem-2021-02-02-171006.png)

## PC Suporte e Acesso via SSH

Na topologia foi adicionado o pc do suporte que tem como função acessar os dispositivos de rede por meio do SSH configurado em cada switch da topologia que tem seus respectivos endereços ips para acesso via ssh conforme a imagem abaixo:

![Alt Text](https://i.ibb.co/8gc1Ndz/imagem-2021-02-02-173327.png)

## Topologia final

tendo todos equipamentos e computadores configurados temos acesso ao site contido no server HTTP segue abaixo uma imagem do acesso ao site e da toplogia final

![Alt Text](https://drive.google.com/thumbnail?id=1WGnb2qdjPpWGZxKwdhWFXtOZHw07q6jS&authuser=0&sz=w1325-h627)

![Alt Text](https://media-exp1.licdn.com/dms/image/C4D22AQFhag-CZfdP1w/feedshare-shrink_2048_1536/0/1611325326772?e=1615420800&v=beta&t=aVBXVYky6DTl-9tGhCD2dud2bYgIGakn2CihzHD0hLM)

Autor: Lucas Silva Conrado






