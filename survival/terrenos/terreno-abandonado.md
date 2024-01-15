---
description: Tempo inativo necessário para terrenos serem consideradas abandonadas.
cover: ../../.gitbook/assets/Inserir_um_titulo_3.png
coverY: 0
---

# 🕸 Terreno Abandonado

Terrenos são consideradas abandonadas de acordo com o tempo que o dono dele fica sem acessar o servidor (offline). Quanto maior a proteção, mais tempo leva para o terreno ser considerado abandonado.\
\
Caso encontre um terreno abandonado utilize o comando `/terrenoreivindicar` para reivindicar a propriedade ao custo de `250 coins` por bloco, segue a tabela de tempo necessário para que um terreno seja considerado abandonado:

## Tempo necessário

<table><thead><tr><th align="center">Tempo offline (dias)</th><th align="center">Tamanho (blocos)</th><th data-hidden align="center">Preço por Bloco</th><th data-hidden></th></tr></thead><tbody><tr><td align="center">90</td><td align="center">Até 999</td><td align="center"></td><td></td></tr><tr><td align="center">120</td><td align="center">1000 a 9.999</td><td align="center">50</td><td></td></tr><tr><td align="center">150</td><td align="center">10.000 a 24.999</td><td align="center">75</td><td></td></tr><tr><td align="center">180</td><td align="center">25.000 a 49.999</td><td align="center">100</td><td></td></tr><tr><td align="center">240</td><td align="center">50.000 a 99.999</td><td align="center"></td><td></td></tr><tr><td align="center">360</td><td align="center">100.000+</td><td align="center"></td><td></td></tr></tbody></table>

{% hint style="info" %}
O custo de reivindicação é de 250 coins por bloco.
{% endhint %}

### **Exemplo:**&#x20;

Terreno de `1000` blocos.

* Tempo para expirar: `60 dias` -> `(1000 a 9.999 blocos)`
* Custo total para reivindicar: `$250.000 coins`

{% hint style="info" %}
O preço por bloco reduz em 1 coin por dia a mais de inatividade de acordo com o tempo excedente ao prazo até o mínimo de 25 coins por bloco.
{% endhint %}

### Exemplos (dias excedentes ao prazo):

Terreno de `1000` blocos.&#x20;

* 61 dias -> Custo por bloco `$249 coins` -> `$249.000 coins`
* 62 dias -> Custo por bloco `$248 coins` -> `$248.000 coins`
* 63 dias -> Custo por bloco `$247 coins` -> `$247.000 coins`
* 64 dias -> Custo por bloco `$246 coins` -> `$246.000 coins`
* 65 dias -> Custo por bloco `$245 coins` -> `$245.000 coins`
* 66 dias -> Custo por bloco `$244 coins`-> `$244.000 coins`&#x20;
* ...&#x20;
* 285 dias -> Custo por bloco `$25 coins`-> `$25.000 coins`&#x20;

## Terreno Abandonado

### Descrição

Proteções são consideradas abandonadas de acordo com o tempo que o dono da proteção fica sem acessar o servidor (offline). Quanto maior a proteção, mais tempo leva para a proteção ser considerada abandonada.

### Remoção

* Verifique a quantidade de blocos de proteção da proteção com o graveto.
* Verificar o tempo offline do jogador dono da proteção através do graveto ou utilizando `/seen <nick>`.
* Utilize o comando `/terrenoreivindicar` verifique o valor necessário para reivindicação e confirme digitando `confirmar` no chat.

{% hint style="warning" %}
Sistema válido para todos os jogadores, inclusive jogadores banidos.
{% endhint %}

## Terrenos Próximos

### Descrição

* É considerado terrenos próximos todas as construções dentro de um raio de `50 blocos`.
* Será levado em consideração também o jogador que construiu no local primeiro.

### Remoção

* Remoção manual realizada pela Staff após abertura de ticket.
* É preciso que um ticket seja aberto informando as coordenadas da proteção.
*   O ticket será resolvido em até 3 dias uteis após sua abertura.

    * O tempo pode variar por motivos de força maior.



    ### **Motivo**

{% hint style="danger" %}
## Regra 15 - Anti-jogo <a href="#id-01" id="id-01"></a>

Qualquer atitude que desestabilize a harmonia do servidor ou o convívio e relacionamento entre os players. As práticas mais comuns de anti-jogo são, por exemplo homes ou warps de armadilhas (trap) com finalidade exclusiva de matar um player e se apossar de seus itens, inventar histórias ou induzir jogadores a enviar pedidos de teleportes e matá-los em seguida, criar uma proteção a menos de 50 blocos de outro jogador atrapalhando o mesmo de expandir ou editar itens seja seu nome, lore ou encantamento com intuito de confundir jogadores (Renomear um gancho de armadilha com nome de chave misteriosa por exemplo).
{% endhint %}

{% hint style="warning" %}
Regra válida para todos os jogadores, inclusive jogadores que doaram em nosso site.
{% endhint %}
