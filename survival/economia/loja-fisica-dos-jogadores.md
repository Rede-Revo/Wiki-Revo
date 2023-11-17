---
description: >-
  Loja física por baús serve para que jogadores possam comprar e vender grande
  quantidade de itens.
---

# Loja Física dos Jogadores

## Criar uma Loja <a href="#criar-uma-loja" id="criar-uma-loja"></a>

{% hint style="warning" %}
Lojas são protegidas pelo sistema de proteção de terrenos!
{% endhint %}

{% hint style="warning" %}
Lojas físicas serão removidas quando a proteção for excluida!
{% endhint %}

{% hint style="warning" %}
Custo: 100 Coins por loja criada
{% endhint %}

## Sistema de Cupons

Aprimore sua estratégia de marketing criando e distribuindo cupons de desconto para os clientes da sua loja, atraindo assim um maior fluxo de visitantes e potencializando suas vendas.

### Como ativo um cupom de loja para poder usa-lo?

Utilize `/pshop discount install <código>`, lembre-se de sempre usar esse comando quando for fazer compra em alguma loja utilizando cupons.

Utilize o comando `/pshop disount info` para ver informações de seu cupom ativo.

### Como crio um cupom?

#### Para criar para todas as suas placas de loja:

`/pshop discount create <código> PLAYER_ALL_SHOPS <porcentagem> <uso-máximo> <preço mínimo ou -1 caso não queira definir um valor mínimo> <data de expiração ou -1 para sem data>`

Exemplo:

`/pshop discount create REVONIVER PLAYER_ALL_SHOPS 25 10 -1 -1`

Esse exemplo criaria o cupom REVONIVER com 25% de desconto sem valor mínimo e sem data de expiração

#### Para criar para placas de loja em especifico:

`/pshop discount create <código> SPECIFIC_SHOPS <porcentagem> <uso-máximo> <preço mínimo ou -1 caso não queira definir um valor mínimo> <data de expiração ou -1 para sem data>`

Exemplo:

`/pshop discount create REVONIVER PLAYER_ALL_SHOPS 25 10 -1 -1`

Esse exemplo criaria o cupom REVONIVER com 25% de desconto sem valor mínimo e sem data de expiração

Para definir quais lojas devem aceitar este desconto digite o comando: `/pshop discount config addshop` olhando para a placa de loja ou use `/pshop discount config removeshop` para remover.

#### Como deleto um cupom?

Basta digitar o comando `/pshop discount remove <código>.`

{% hint style="info" %}
O tempo de expiração aceita o formato Zulu Time e UNIX Timestamp no formato de segundos

Existe um site on-line que pode ajudá-lo a converter o tempo: https://www.unixtimestamp.com/

Para o formato Zulu Time (ISO 8601 Estendido): `yyyy-MM-dd'T'HH:mm:ssZZ`
{% endhint %}
