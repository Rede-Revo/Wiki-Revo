---
description: Set de Vendas ou Set Estranho
icon: helmet-battle
cover: ../../../.gitbook/assets/Inserir_um_titulo_3.png
coverY: 0
layout:
  width: default
  cover:
    visible: true
    size: full
    mask: none
  title:
    visible: true
  description:
    visible: true
  tableOfContents:
    visible: true
  outline:
    visible: true
  pagination:
    visible: true
  metadata:
    visible: true
  tags:
    visible: true
  actions:
    visible: true
---

# Set de Vendas

## Introdução

O Set de Vendas ou Set Estranho, é um conjunto especial de vestimentas que concede bônus no valor recebido durante suas vendas na loja do servidor.

Inicialmente, suas quatro partes são encontradas como Itens estranhos, ao reunir e vestir todas as peças pela primeira vez, o conjunto é formado e cada item recebe seu próprio nível de perfeição, que determina seu bônus de venda e durabilidade.

## Formando o Set de Vendas

Para formar o conjunto, basta vestir simultaneamente as quatro partes do Set estranho, que são, Capacete Estranho, Peitoral Estranho, Calças Estranhas e Botas Estranhas, após colocar todas as partes como armadura, uma mensagem no chat será exibida, mostrando que você completou o Set de Vendas, nesse momento, todas as peças são atualizadas automaticamente e passam a exibir seu nível individual de perfeição e bônus de venda.

## Nível de perfeição

Cada parte recebe individualmente um nível de perfeição, variando de 1% a 100%, quanto maior sua perfeição, maior será o seu bônus e sua durabilidade. Por esse motivo, duas pelas do mesmo tipo podem possuir valores diferentes.

### Calculo do bônus de venda

O bônus é calculada em cima do nível de perfeição da pela, de forma simplificada, a formula seria:\
Bônus = 0,5+(Perfeição \* 0,015).\
Exemplo:\
Se o capacete de vendas tem 70% de perfeição, na fórmula ficaria:\
Bônus = 0,5+(70 \* 0,015) = 0,5+1,05 = 1,55\
Ou seja, o bônus nesse caso seria de 1,55%, mas isso é exibido na lore/descriçao da parte do set.&#x20;

{% hint style="info" %}
O valor exibido na descrição do item possui apenas duas casas decimais, porém o cálculo das vendas utiliza o valor interno completo, por esse motivo, somar apenas as porcentagens exibidas na descrição do item, pode resultar em uma pequena diferença em relação ao valor final recebido.
{% endhint %}

### Calculo da venda

Cada peça possui seu próprio bônus e os valores funcionam em conjunto durante as vendas, o cálculo é feito basicamente somando os bônus do set equipado, e depois adicionado em cima do valor que a venda ficaria.\
Exemplo:\
Vamos imaginar os seguintes bônus para cada set:\
\- Capacete: 1,80%\
\- Peitoral: 1,97%\
\- Calça: 1,27%\
\- Botas: 0,91%\
se somar todos esses valores chegará em 5,95%, teoricamente esse é o valor total do bônus, porém, devido as casas decimais internas utilizadas pelo sistema, o bônus real desse conjunto é de 5,945, esse valor real, é calculado com base na fórmula do bônus pelo nível de perfeição.

{% hint style="info" %}
Essa foi uma breve explicação de como funciona o cálculo do sistema internamente. Os cálculos demonstrados aqui, apenas servem como base de comparação, ainda sim, no resultado final, podem ter divergências, pois o servidor trabalha apenas até duas casas decimais nos Coins.&#x20;
{% endhint %}

### Set Perfeito

Uma peça que alcançar 100% de perfeição recebe o status especial Perfeito em frente do seu nome. Nesse caso em específico, não é realizada nenhum cálculo, o sistema entrega 2,5% de bônus e 125.000 pontos de durabilidade.

## Durabilidade

A durabilidade também é determinada pelo nível de perfeição da peça, para itens de 1% a 99% de perfeição, a durabilidade é de 1.000 pontos a cada 1%, então, uma parte com 45% de nível de perfeição, a durabilidade é de 45.000 pontos de durabilidade.

### Consumo da durabilidade

A durabilidade utilizada durante uma venda é calculada pela quantidade de slots vendidos, e não pela quantidade total de itens.\
Exemplo:

* 4 itens agrupados em 1 slot → consome 1 de durabilidade;
* 64 itens agrupados em 1 slot → consome 1 de durabilidade;
* 4 itens separados em 4 slots → consome 4 de durabilidade;
* 4 packs de 64 ocupando 4 slots → consome 4 de durabilidade.
* 4 packs de 64 ocupando 8 slots → consume 8 de durabilidade.

{% hint style="info" %}
O que importa para o consumo do Set de Vendas é quantos slots participaram da venda, independentemente da quantidade de itens.
{% endhint %}

## Reparação

As peças do set de Vendas podem ser reparadas usando itens especiais, atualmente existem dois itens que podem reparar o Set de Vendas, o Reparador Universal e o Reparador de Vendas, ambos podem ser encontrados na [Caixa Divina](https://wiki.rederevo.com/survival/caixas/divina#itens).

Para reparar basta usar o reparador por cima da peça no inventário.

### Demonstração

Em breve...

## Uso em conjunto com outros bônus

O benefício das peças funcionam simultaneamente com outros sistemas de vendas, como Boosters de venda, bônus da loja e similares.

{% hint style="info" %}
Os diferentes benefícios aplicados conforme a mecânica de cada sistema e não devem ser tratados necessariamente como uma simples soma direta das porcentagens.
{% endhint %}

## Obtenção

Primeiro você precisa do Set Estranho completo, que podem ser encontradas na [Caixa Divina](https://wiki.rederevo.com/survival/caixas/divina#itens).

Após conseguir todas as partes do set estranho, só equipar todos simultaneamente que o set Estranho irá converter automaticamente para Set de Vendas, gerando assim a Perfeição do item, juntamente com o bônus e durabilidade.
