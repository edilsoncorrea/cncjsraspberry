## Tutorial sobre como instalar o CNCJS no Raspberry


[Tutorial muito bom sobre a instalação do CNCJS no Raspberry](https://github.com/cncjs/cncjs/wiki/Setup-Guide:-Raspberry-Pi-%7C-Install-Node.js-via-Package-Manager-*(Recommended)*) . Este tutorial foi montado quase que inteiramente a partir dele. Referência: Mitch Bradley edited this page on 6 Feb 2021 · 21 revisions

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

Algo parecido com isso deve ser mostrado no terminal:
```
2019-10-04T22:45:16.701Z - info init Loading configuration from "/home/pi/.cncrc"
2019-10-04T22:45:17.931Z - info init Starting the server at http://127.0.1.1:8000
```
