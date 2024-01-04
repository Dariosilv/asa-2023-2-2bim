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

Aqui está o arquivo de configuração `/etc/dnmasq.d/asa.conf .`

[![Screenshot from 2024-01-03 20-54-41](https://i.im.ge/2024/01/04/3l2FFa.Screenshot-from-2024-01-03-20-54-41.png)](https://im.ge/i/3l2FFa)


Este exemplo configura o servidor DHCP para atribuir endereços IP no intervalo de 192.168.1.100 a 192.168.1.254 com uma máscara de rede de 255.255.255.0 e um tempo de arrendamento de 12 horas.

Você pode configurar o servidor DHCP com uma variedade de opções. Para obter mais informações, consulte a documentação do dnsmasq.

Para reiniciar o servidor DHCP, você pode usar o seguinte comando:

rc-service dnsmasq restart 

Após reiniciar o servidor, ele começará a atribuir endereços IP aos clientes DHCP.

Configurando o servidor DHCP para um intervalo de endereços IP específico

Você pode configurar o servidor DHCP para atribuir endereços IP em um intervalo específico de endereços IP. Para fazer isso, use a opção dhcp-range.

O formato da opção dhcp-range é o seguinte:

dhcp-range=início-do-intervalo,fim-do-intervalo,máscara-de-rede,tempo-de-arrenda

- Reservar 2 endereços (IP fixo) fora do intervalo do item anterior. (5 pontos)


Configurando o servidor DHCP para um intervalo de endereços MAC específicos


## Teste

Aqui está o Teste no windownsXp :

E está funcionado os IP configurados :

[![Conf](https://i.im.ge/2024/01/04/3l149m.Screenshot-from-2024-01-03-20-45-56.png)](https://im.ge/i/3l149m)


Agora está aqui o teste no clone do windowns.

[![Screenshot from 2024-01-03 20-57-46](https://i.im.ge/2024/01/04/3l2dLz.Screenshot-from-2024-01-03-20-57-46.png)](https://im.ge/i/3l2dLz)