# Planejamento de Rede

## Objetivo

O objetivo deste projeto foi utilizar todos os conhecimentos de rede passados pela Escola SENAI de informática para planejar e montar uma rede com as seguintes características:

* Protocolos IPv4 e IPv6 em um esquema de pilha dupla;
* Divisão de sub-redes;
* Criação de vlans de suas respectivas redes;
* Rota padrão no roteador;
* Conexão via SSH;
* Configurações básicas de switchs e roteador.

## Rede

Neste projeto utilizamos um **ip de classe C**: 192.168.0.0 e um **IPV6**: 2001:db8:cafe:1::/64 e dividimos esse ip em sub-redes para uma melhor segurança e tráfego da rede sendo as sub-redes:

![Alt Text](https://i.ibb.co/kBdP17f/sub-redes.png)

A rede também foi dividida em 7 vlans (com a vlan nativa) seguindo a imagem abaixo:

![Alt Text](https://i.ibb.co/phVxkj2/vlan.png)


## Computadores

Cada computador está configurado com seus próprios ips estáticos, com um gateway padrão de cada rede, dns-server que já foi pré montado e sua mascará de rede de acordo com a sua sub-rede, conforme a imagem abaixo:

![Alt Text](https://i.ibb.co/zR9tBgD/Computadores.png)

Os computadores estão atrelados a um switch da sua respectiva rede, utilizando mode access em suas interfaces. Segue uma imagem da topologia abaixo:

![Alt Text](https://i.ibb.co/ByW3419/imagem-2021-02-02-165504.png)

## Switchs 

Cada switch foi configurado com banner, senha na console e na enable, criadas suas respectivas vlans, adicionado os mode access e trunk às suas portas e um domínio para acessar 
o site contido no server HTTP. Todos os switchs se encontram em um switch-core referente a imagem abaixo: 

![Alt Text](https://i.ibb.co/mqrZXtJ/imagem-2021-02-02-170306.png)


## Roteador e Rota Padrão

No roteador, foram feitas as mesmas configurações padrões feitas no switch, mas temos a adição de uma rota padrão, que na topologia, a rota padrão é o SRV-CLOUD e também utilizamos um método chamado rout-on-a-stick, onde criamos sub-interfaces para cada vlan na rede conforme a imagem abaixo:

![Alt Text](https://i.ibb.co/fkRB4qg/imagem-2021-02-02-171006.png)

## PC Suporte e Acesso via SSH

Na topologia, foi adicionado o pc do suporte que tem como função acessar os dispositivos de rede por meio do SSH configurado em cada switch da topologia, que tem seus respectivos endereços ips para acesso via SSH conforme a imagem abaixo:

![Alt Text](https://i.ibb.co/8gc1Ndz/imagem-2021-02-02-173327.png)

## Topologia final

Tendo todos os equipamentos e computadores configurados, temos acesso ao site contido no server HTTP. Segue abaixo uma imagem do acesso ao site e da topologia final;

![Alt Text](https://i.ibb.co/4mF3WKz/entregavel-sprint-3.png)

![Alt Text](https://media-exp1.licdn.com/dms/image/C4D22AQFhag-CZfdP1w/feedshare-shrink_2048_1536/0/1611325326772?e=1615420800&v=beta&t=aVBXVYky6DTl-9tGhCD2dud2bYgIGakn2CihzHD0hLM)

* Autor: Lucas Silva Conrado
* Revisão: Sasha Sanches






