# DNS

## Instalação

Na instalação do DNS foi craido Dois Container um macau e outro olinda .

e tambem e modificado o arquivo `/etc/resolv.conf.`

`nano /etc/resolv.conf`

Os container usados na instalaçao do DNS :

[![Container](https://i.im.ge/2024/01/04/3lSSw1.Container.png)](https://im.ge/i/3lSSw1)

falta colocar os  prints do arquivo modificado para o DNS.

## Configuração

Incluir o(s) nome(s) e o conteúdo do(s) arquivo(s) de configuração.

Cinco registros (4 pontos cada):

- 3 do tipo A (Endereços);

Criação de 3 registros de recurso do tipo A => Hosts:

`nome dos 3 registros: macau, olinda, goiania :`

[![Dns](https://i.im.ge/2024/01/04/3lSsXm.Dns.png)](https://im.ge/i/3lSsXm)


- 2 do tipo CNAME (`www` e `docs`);

Criação de 2 registros do Tipo CNAME :

`Nome dos 2 registros : docs,www .`

[![Dns](https://i.im.ge/2024/01/04/3lSsXm.Dns.png)](https://im.ge/i/3lSsXm)

## Teste

Falta colocar o print do ping.


