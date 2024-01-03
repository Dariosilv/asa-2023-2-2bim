# SMB

## Instalação
Comandos de instalação  no alpine linux e configuração:

apk add samba

apk add openssh

rc-service samba status

```/etc/init.d/samba [opção] start vai iniciar o samba 
```

samba-tool domain provision –use-rfc2307 –interactive 

é usado para provisionar um novo domínio Samba Active Directory e habilitar as extensões NIS (Network Information Service). O NIS é um protocolo para compartilhar informações de usuário e grupo entre sistemas Unix.

[![Instalação_Samba](https://i.im.ge/2023/12/22/xuFPpz.Instalacao-Samba.png)](https://im.ge/i/xuFPpz)

Esse comando é para o serviço do servidor samba .



## Configuração

Incluir o(s) nome(s) e o conteúdo do(s) arquivo(s) de configuração.

1. Criar 2 grupos para dois de seus sobrenomes;

Na Criação dos Grupos ira ser feito dois Grupos com o seu sobrenome Com duas OU Norte é Sul:

[![Criação_usuarios](https://i.im.ge/2023/12/22/xFpYzM.Criacao-usuarios.png)](https://im.ge/i/xFpYzM)

Nesse Comando é Criado os Grupos na Qual eles são Lima,Silva e Támbem foi criado os usuarios dos Grupos Correspondente.

2. Criar 4 usuários, dois para cada um dos sobrenomes;

Nesta imagem e Criado Quatro usuarios para os Grupos Lima,Silva:

[![Criação_usuarios](https://i.im.ge/2023/12/22/xFpYzM.Criacao-usuarios.png)](https://im.ge/i/xFpYzM)

esses usuarios são criados pois todo servidor precisa de usarios no Banco de Dados e no Samba não pode ser Diferente.

3. Compartilhar duas pastas com dois de seus sobrenome, compartilhado para o grupo com o sobrenome correspondente.

Compartilhamento de pastas:

comandos:


```cd /srv/samba```

```nano  /etc/samba/smb.conf ```


```modificar o arquivo /etc/hosts e /etc/hostname```


```configurar o arquivo /etc/samba/smb.conf```


Arquivo /etc/samba/smb.conf configurado:

[![Compartilhamento_pastas](https://i.im.ge/2023/12/22/xFBtJL.Compartilhamento-pastas.png)](https://im.ge/i/xFBtJL)


## Teste

Pra fazer o teste se está funcionando tem que logar em outro usuarios dos grupos:

[![login_usuarios](https://i.im.ge/2023/12/22/xOMIE6.login-usuarios.png)](https://im.ge/i/xOMIE6)

Nesta imagem está logado um usuario do grupo Lima.

