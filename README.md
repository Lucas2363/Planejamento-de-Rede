# Planejamento de Rede

Este projeto foi apresentado pela escola SENAI de informática. Ele é o planejamento de uma rede principal ''Marciana'' onde temos varias sub-redes e vlans atribuidas a cada 
um ipv4 e ipv6 e o uso de uma rota padrão para todas as redes.

## Rede

Neste projeto utilizamos um **ip de classe C** : 192.168.0.0 e um **IPV6** : 2001:db8:cafe:1::/64 e dividimos esse ip em sub-redes para uma melhor segurança e trafégo da rede sendo as sub-redes:

![Alt Text](https://i.ibb.co/kBdP17f/sub-redes.png)

A rede também foi dividida em 7 vlans (com a vlan nativa) seguindo a imagem abaixo:

![Alt Text](https://i.ibb.co/phVxkj2/vlan.png)


## Computadores

Cada computador está configurado com seus próprios ips estáticos, com um gateway e dns-server conforme a imagem abaixo:

![Alt Text](https://i.ibb.co/zR9tBgD/Computadores.png)

Os computadores estão atrelados a um switch da sua respectiva rede, utilizando mode access 

![Alt Text](https://i.ibb.co/ByW3419/imagem-2021-02-02-165504.png)




