## Tutorial sobre como instalar o CNCJS no Raspberry


[Tutorial muito bom sobre a instalação do CNCJS no Raspberry](https://github.com/cncjs/cncjs/wiki/Setup-Guide:-Raspberry-Pi-%7C-Install-Node.js-via-Package-Manager-*(Recommended)*)

```
curl -sL https://deb.nodesource.com/setup_10.x | sudo -E bash -
sudo apt install -y nodejs build-essential npm
sudo npm install -g npm@latest
```
  
Ignore os avisos dos passos do instalador do npm.  Segundo o autor do texto, o npm está apenas sendo chato.

```
sudo npm install -g cncjs@latest --unsafe-perm
```  

Se os comandos acima gerarem algum erro, você pode dar uma olhada [aqui](https://github.com/cncjs/cncjs/wiki/Setup-Guide:-Raspberry-Pi-%7C-Installation-Problems-and-Solutions) para possíveis soluções.

### Testando a instalação

Neste ponto você pode realizar um teste rápido para ver se o cncjs está funcionando. Entre isso no prompt do terminal:

```
cncjs
```
