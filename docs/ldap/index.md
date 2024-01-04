# LDAP

## Instalação

## Configuração

Incluir o(s) nome(s) e o conteúdo do(s) arquivo(s) de configuração.

- Criar duas OU: `vendedores` e `rh`;

Criar a OU vendedores:

O servidor LDAP OpenLDAP é configurado usando o arquivo /etc/openldap/slap.conf. Este arquivo contém as configurações básicas do servidor, como o domínio, o esquema e o armazenamento.

Para configurar o servidor LDAP para o domínio example.com, abra o arquivo /etc/openldap/slapd.conf e edite as seguintes linhas:


Pra criar a OU Vendedores da unidade orgazional assim como o DNS:

[![Screenshot from 2024-01-02 19-24-51](https://i.im.ge/2024/01/03/3MABLC.Screenshot-from-2024-01-02-19-24-51.png)](https://im.ge/i/3MABLC)

 Aqui já esta configurado A OU Vendedores.



- Mover o grupo `sobrenome1` e seus membros para a OU `vendedores`;


Criar a OU rh

[![Screenshot from 2024-01-02 19-25-07](https://i.im.ge/2024/01/03/3MCDFJ.Screenshot-from-2024-01-02-19-25-07.png)](https://im.ge/i/3MCDFJ)

Aqui já está configurado a OU RH .

Esses comandos criam as OUs vendedores e rh no domínio example.com.
- Mover os grupo `sobrenome2` e seus membros para a OU `rh`.


Arquivos de configuração

Os arquivos de configuração usados para criar as OUs e mover os grupos são os seguintes:


Esses arquivos são necessários para que o servidor LDAP possa entender os objetos e atributos usados nos comandos ldapadd e ldapmodify.


## Teste

Com toda essa configuração o LDAP já esta funcionando normalmente.
