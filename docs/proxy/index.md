# PROXY

## Instalação

```
sudo apt update
```
```
sudo apt install squid
```


## Configuração

Incluir o(s) nome(s) e o conteúdo do(s) arquivo(s) de configuração.

Após a instalação, o arquivo de configuração do Squid está localizado no diretório /etc/squid/squid.conf. Para editar este arquivo, execute o seguinte comando:

```nano /etc/squid/squid.conf ```

```Arquivo /etc/squid/squid.conf Já configurado :
```
[![acl_proxy](https://i.im.ge/2023/12/25/xLH1dy.acl-proxy.png)](https://im.ge/i/xLH1dy)

Fazer a configuração de 4 ACLs distintas, conforme a atividade passada em sala de aula.

Aqui está 4 ACLs destintas na qual eles são nome,redes socias,IP,e navegador .

[![acl_proxy](https://i.im.ge/2023/12/25/xLH1dy.acl-proxy.png)](https://im.ge/i/xLH1dy)

## Teste

O teste das ACLs funcionando no navegador :

Controle de acesso: você pode usar o Squid para restringir o acesso dos clientes ao Squid com base em seu endereço IP, nome de usuário ou grupo.

Restrição de conteúdo: você pode usar o Squid para restringir o conteúdo da Internet que os clientes podem acessar. Isso pode ser útil para bloquear sites de conteúdo adulto ou prejudicial.

Monitoramento: você pode usar o Squid para monitorar o uso do Squid. Isso pode ser útil para identificar usuários ou sites que estão usando um grande volume de largura de banda.
ACl de redes socias expecificamente o Facebook:

[![Facebook_proxy](https://i.im.ge/2023/12/25/xLHju4.Facebook-proxy.png)](https://im.ge/i/xLHju4)

ACL de nome:

[![nome_proxy](https://i.im.ge/2023/12/25/xLHPLP.nome-proxy.png)](https://im.ge/i/xLHPLP)


ACL de bloqueio de IP :

[![IP_proxy](https://i.im.ge/2023/12/25/xLHEtr.IP-proxy.png)](https://im.ge/i/xLHEtr)

ACL do browser firefox:

[![firefox_proxy](https://i.im.ge/2023/12/25/xLpMsh.firefox-proxy.png)](https://im.ge/i/xLpMsh)