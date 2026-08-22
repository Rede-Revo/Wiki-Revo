---
description: Lista com todos os comandos do sistema de terrenos.
icon: rectangle-terminal
cover: ../../.gitbook/assets/Inserir_um_titulo_3.png
coverY: 0
---

# Comandos

### Criação e redimensionamento

<table><thead><tr><th width="227.3333740234375">Comando</th><th width="510">Descrição</th></tr></thead><tbody><tr><td>/terreno proteger &#x3C;raio></td><td>Cria uma proteção com o raio informado, usando sua posição atual como centro.</td></tr><tr><td>/terreno dividir</td><td>Ativa ou desativa o modo de criação de subterrenos.</td></tr><tr><td>/terreno dividir &#x3C;raio></td><td>Cria uma subproteção com o raio informado, usando sua posição atual como centro.</td></tr><tr><td>/terreno expandir &#x3C;raio></td><td>Aumenta o terreno na direção que estiver olhando.</td></tr></tbody></table>

### Consulta e remoção

<table><thead><tr><th width="227.3333740234375">Comando</th><th width="510">Descrição</th></tr></thead><tbody><tr><td>/terreno lista</td><td>Exibe no chat uma lista com todos os seus terrenos.</td></tr><tr><td>/terreno desproteger</td><td>Deleta o terreno que você estiver.</td></tr><tr><td>/terreno info</td><td>Exibe no chat informações sobre o terreno.</td></tr><tr><td>/terreno desprotegertudo</td><td>Solicita a remoção de todos os seus terrenos.</td></tr><tr><td>/terreno reivindicar</td><td>Solicita a reivindicação de um <a href="https://wiki.rederevo.com/survival/terrenos/terreno-abandonado">terreno abandonado</a>.</td></tr></tbody></table>

### Permissões

<table><thead><tr><th width="302">Comando</th><th width="436.6666259765625">Descrição</th></tr></thead><tbody><tr><td>/terreno confiarfarm &#x3C;nick></td><td>Concede permissão para interagir com plantações.</td></tr><tr><td>/terreno confiaracesso &#x3C;nick></td><td>Concede permissão de acesso.</td></tr><tr><td>/terreno confiararmazem &#x3C;nick></td><td>Concede permissão de armazém.</td></tr><tr><td>/terreno confiar &#x3C;nick></td><td>Concede permissão de construção.</td></tr><tr><td>/terreno confiartudo &#x3C;nick></td><td>Concede permissão de gerenciamento.</td></tr><tr><td>/terreno confiarlista</td><td>Exibe no chat todos os jogadores com permissão.</td></tr><tr><td>/terreno desconfiar &#x3C;nick></td><td>Remove a permissão dos jogadores.</td></tr></tbody></table>



{% hint style="info" %}
Você também pode usar a tag #all no lugar do nick para conceder essa permissão para todos os jogadores.
{% endhint %}

### Permissão em subterrenos

<table><thead><tr><th width="227.3333740234375">Comando</th><th width="509.9998779296875">Descrição</th></tr></thead><tbody><tr><td>/terreno restrito</td><td>Alterna a herança de permissões no subterreno que estiver.</td></tr><tr><td>/terreno restrito &#x3C;on|off></td><td>Ativa ou desativa a herança de permissões no subterreno que estiver, quando ativado, as permissões do terreno principal não são válidas para esse subterreno.</td></tr></tbody></table>

### Explosões

<table><thead><tr><th width="227.3333740234375">Comando</th><th width="510">Descrição</th></tr></thead><tbody><tr><td>/terreno explosoes</td><td>Alterna a permissão para explosões quebrarem blocos dentro do terreno.</td></tr><tr><td>/terreno explosoes on</td><td>Permite que as explosões quebrem blocos dentro do terreno.</td></tr><tr><td>/terreno explosoes off</td><td>Impede que as explosões quebrem blocos dentro do terreno.</td></tr></tbody></table>

{% hint style="warning" %}
Isso também é válido para mobs, como o creeper, evite sair do jogo com essa opção ligada.
{% endhint %}

### Controle de entrada

<table><thead><tr><th width="227.333251953125">Comando</th><th width="510.0001220703125">Descrição</th></tr></thead><tbody><tr><td>/terreno privado</td><td>Proíbe qualquer jogador de entrar no seu terreno, exceto os que tem permissão no local.</td></tr><tr><td>/claimban ban &#x3C;nick></td><td>Proíbe esse jogador de entrar no seu terreno.</td></tr><tr><td>/claimban unban &#x3C;nick></td><td>Remove a proibição do jogador de entrar no seu terreno.</td></tr><tr><td>/claimban list</td><td>Exibe a lista de todos os jogadores proibidos de entrar no seu terreno.</td></tr></tbody></table>

### Blocos de proteção

<table><thead><tr><th width="227.3333740234375">Comando</th><th width="510">Descrição</th></tr></thead><tbody><tr><td>/terreno blocos</td><td>Exibe no chat a quantidade de blocos que você tem, usou, e total.</td></tr><tr><td>/comprarblocos &#x3C;qt></td><td>Compra a quantidade de blocos especificada. Cada bloco custa 25 coins.</td></tr></tbody></table>

{% hint style="warning" %}
Antes de comprar blocos de proteção, confira a quantidade e valor total. O sistema não tem confirmação, assim que o comando é executado, os coins são descontados e os blocos adicionados.
{% endhint %}
