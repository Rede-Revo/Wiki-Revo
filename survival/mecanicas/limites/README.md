---
icon: octagon-minus
cover: ../../../.gitbook/assets/Inserir_um_titulo_3.png
coverY: 0
---

# Limites

## Introdução

Para ajudar a manter a estabilidade e desempenho do servidor, alguns blocos, itens e entidades possuem limites.

A forma de aplicação desse limite varia conforme o sistema, mas na maioria dos casos desta página, a verificação ocorre no momento da colocação, ou seja, caso o limite já tenha sido atingido, o servidor simplesmente impede que seja colocado outro.

{% hint style="info" %}
Os limites de criaturas(mobs) possuem regras detalhadas e estão disponíveis para consulta na página de [Mobs](https://wiki.rederevo.com/survival/mecanicas/limites/mobs#introducao).
{% endhint %}

## Limites

### Drusas de Ametistas e Geradores de Criaturas

As drusas de Ametista e os Geradores de Criaturas possuem limite por chunck.

<table><thead><tr><th width="211">Item</th><th>Limite</th></tr></thead><tbody><tr><td>Drusas de Ametista</td><td>72 drusas por Chunck</td></tr><tr><td>Geradores de Criaturas</td><td>2 spawners por Chunck</td></tr></tbody></table>

A verificação no caso das drusas e spawners ocorrem no momento da colocação, ou seja, caso o limite já tenha excedido o sistema não permitirá uma nova colocação.

### Redstone

Componentes de redstone possuem limite por chunck.

<table><thead><tr><th width="237.666748046875">Item</th><th>Limite</th></tr></thead><tbody><tr><td>Bancada Automática</td><td>8 bancadas automáticas por chunck</td></tr><tr><td>Comparador de Redstone</td><td>16 comparadores de redstone por chunk</td></tr><tr><td>Ejetor</td><td>16 ejetores por chunk</td></tr><tr><td>Liberador</td><td>16 liberadores por chunk</td></tr><tr><td>Observador</td><td>16 observadores por chunck</td></tr><tr><td>Pistão</td><td>16 pistões por chunck</td></tr><tr><td>Pistão Grudento</td><td>16 pistões grudentos por chunk</td></tr><tr><td>Repetidor de Redstone</td><td>16 repetidores de redstone por chunk</td></tr><tr><td>Funil</td><td>10 funis por chunck</td></tr><tr><td>Pó de redstone</td><td>32 pós de redstone por chunk</td></tr></tbody></table>

Para todos os itens citados acima, o limite é verificado no momento da colocação, ou seja, se o limite já estiver ultrapassado, não será possível colocar um novo bloco.

{% hint style="info" %}
Cada item possui sua própria contagem, por exemplo, o limite de compradores de redstone não interferem na quantidade de observadores ou pistões que podem ser colocados na mesma chunck.
{% endhint %}

### Carrinho de Mina com Funil

O carrinho de mina com funil funciona de forma um pouco diferente dos demais itens de redstone.&#x20;

<table><thead><tr><th width="247">Item</th><th>Limite</th></tr></thead><tbody><tr><td>Carrinho de Mina com Funil</td><td>4 carrinhos de mina com funil em um raio de 16 blocos</td></tr></tbody></table>

No caso do carrinho com funil, o limite não é calculado por chunck, podendo existir no máximo 4 carrinhos em um raio de 16 blocos.

Diferente dos demais limites desta página, o limite dos carrinhos com funil é calculado mediante análises periódicas no raio do carrinho, caso o sistema identifique que existem mais de 4 carrinhos de mina com funil em um raio de 16 blocos, o(s) carrinho(s) com funil excedente(s) será(ão) removido(s) pelo sistema.

{% hint style="warning" %}
Quando um carrinho de mina com funil é removido pelo sistema de limites, os itens dentro dele são dropados no local que aconteceu a remoção.
{% endhint %}

