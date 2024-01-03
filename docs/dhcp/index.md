# DHCP

## Instalação
Vai ser preciso instalar o dnsmasq

apk add dnsmasq


## Configuração

Incluir o(s) nome(s) e o conteúdo do(s) arquivo(s) de configuração.

Arquivo de Configuração do dnsmasq é :

`/etc/dnsmasq.conf `

dentro desse arquivo e criado dentro dele o arquivo teste.conf :

`nano /etc/dnsmasq.conf/teste.conf`


- Distribuir um intervalo (*range* em inglês) de endereços IP; (15 pontos)
Após instalar o pacote, você precisará configurar o servidor DHCP. Você pode fazer isso editando o arquivo de configuração /etc/dnsmasq.conf.

Aqui está um exemplo de configuração básica para o servidor DHCP:

`interface=eth0`

`dhcp-range=192.168.1.100,192.168.1.254,255.255.255.0,12h`

Este exemplo configura o servidor DHCP para atribuir endereços IP no intervalo de 192.168.1.100 a 192.168.1.254 com uma máscara de rede de 255.255.255.0 e um tempo de arrendamento de 12 horas.

Você pode configurar o servidor DHCP com uma variedade de opções. Para obter mais informações, consulte a documentação do dnsmasq.

Para reiniciar o servidor DHCP, você pode usar o seguinte comando:

sudo systemctl restart dnsmasq

Após reiniciar o servidor, ele começará a atribuir endereços IP aos clientes DHCP.

Configurando o servidor DHCP para um intervalo de endereços IP específico

Você pode configurar o servidor DHCP para atribuir endereços IP em um intervalo específico de endereços IP. Para fazer isso, use a opção dhcp-range.

O formato da opção dhcp-range é o seguinte:

dhcp-range=início-do-intervalo,fim-do-intervalo,máscara-de-rede,tempo-de-arrenda

- Reservar 2 endereços (IP fixo) fora do intervalo do item anterior. (5 pontos)

o exemplo de configuração no windownsxp:

[![Servidor dhcp](https://i.im.ge/2023/12/30/x85Q5r.Servidor-dhcp.png)](https://im.ge/i/x85Q5r)



Configurando o servidor DHCP para um intervalo de endereços MAC específicos


## Teste

Aqui está um Teste do servidor dhcp no windowns xp:

[![Servidor dhcp](https://i.im.ge/2023/12/30/x85Q5r.Servidor-dhcp.png)](https://im.ge/i/x85Q5r)
