---
description: >-
  Alguns jogadores podem enfrentar algumas vezes problemas com a conexão em
  nosso servidor, então fizemos esse pequeno guia com algumas possíveis soluções
cover: ../.gitbook/assets/bannercomfundorevo.png
coverY: 0
---

# ⚙ Problemas de Conexão

### Se você acha que seu problema de conexão é culpa do servidor, tente um dos 2 ips diferentes:

* rederevo.com
* jogar.rederevo.com `(esse é o mais recomendado)`

### Ainda não resolveu?

Se você está enfrentando problemas de conexão, pode ser uma boa ideia limpar o seu cache DNS – um processo também conhecido como flush DNS. Isso pode soar como algo técnico e complicado, só que é muito mais fácil do que você pode imaginar.\
\
Aprenda a limpar o cache DNS:

#### **Microsoft Windows**

1. Pressione as teclas **Windows+R** juntas ou clique com o botão direito no menu **Iniciar** do Windows e então pressione **Executar**. Digite **cmd** para abrir o console do **Prompt de Comando** do Windows.  Se você ainda não tem privilégios de administrador, rode o **cmd** ao apertar **Ctrl + Shift + Enter**.
2. Digite **ipconfig/flushdns** no prompt de comando e aperte enter. Esse comando vai limpar os arquivos de cache DNS do seu computador e redefinir o cache de resolução DNS.
3. Se o processo foi bem-sucedido, você deverá ver a seguinte mensagem de confirmação:

![](<../.gitbook/assets/image (2) (1) (1) (1) (1).png>)

#### Linux <a href="#h-linux" id="h-linux"></a>

Por padrão, o Ubuntu não armazena um cache de registros DNS. Se você instalar manualmente um serviço como o **name service caching daemon** (nscd), os passos abaixo vão ensinar como promover o flush do cache DNS.

1. Pressione as teclas **Ctrl+Alt+T** juntas para abrir a janela do terminal.
2.  Insira o seguinte comando para limpar os arquivos de cache DNS no subdiretório **init.d**:

    ```
    sudo /etc/init.d/nscd restart
    ```

Confira agora o guia de como limpar o cache DNS num sistema que usa **systemd**.

1. Pressione as teclas **Ctrl + Alt + T** juntas para abrir a janela do terminal.
2.  Digite a seguinte linha de comando:

    ```
    systemd-resolve --flush-caches
    ```
3.  Insira o seguinte texto no prompt de comando para checar se o comando anterior limpou o cache DNS com sucesso.

    ```
    systemd-resolve --statistics
    ```

#### Mac OS X <a href="#h-mac-os-x" id="h-mac-os-x"></a>

Os passos para executar o flush do DNS no Mac OS X são simples, mas você precisa rodar o comando certo com base na sua versão atual do OS X.

1. Pressione a tecla **F4** e então insira **terminal** no campo de busca do Launchpad para abrir a janela do terminal.
2.  Se você está usando **Mac OS Sierra**, **X El Capitan**, **X Mavericks**, **X Mountain Lion** ou **X Lion** insira o seguinte comando:

    ```
    sudo killall -HUP mDNSResponder
    ```
3.  Para fazer o flush DNS no **Mac OS X Yosemite**, use o seguinte código:

    ```
    sudo discoveryutil udnsflushcaches
    ```
4.  Se você estiver rodando o **Mac OS X Snow Leopard**, o comando é este aqui:

    ```
    sudo dscacheutil -flushcache
    ```
5.  Para o **Mac OS X Leopard** e mais antigos, insira o seguinte comando para limpar o cache DNS:

    ```
    sudo lookupd -flushcache
    ```
6.  Para fazer o flush DNS no **Mac OS X High Sierra**, insira isso aqui no prompt de comando:

    ```
    sudo killall -HUP mDNSResponder
    ```
7. Aqui está o comando para flush do cache DNS no **Mac OS X Mojave**:
8. ```
   sudo killall -HUP mDNSResponder
   ```
9.  Se você está rodando o **Mac OS X Catalina**, use este comando:

    ```
    sudo killall -HUP mDNSResponder
    ```
10. Aqui está o comando para flush do cache DNS no **Mac OS X Big Sur**:

    ```
    sudo dscacheutil -flushcache;
    ```

    ```
    sudo killall -HUP mDNSResponder
    ```

### Mesmo assim o problema continua?

Tenta deixar sua rota mais limpa com o servidor utilizando o aplicativo da Cloudflare [https://1.1.1.1/](https://1.1.1.1/)

&#x20;                                                 ![](<../.gitbook/assets/image (1) (1) (2).png>)

#### E se mesmo assim não resolver então é algum problema com a sua conexão
