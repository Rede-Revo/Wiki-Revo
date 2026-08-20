---
description: >-
  Loja física por baús serve para que jogadores possam comprar e vender grande
  quantidade de itens.
---

# 🪧 Loja Física dos Jogadores

{% hint style="warning" %}
Lojas são protegidas pelo sistema de proteção de terrenos!
{% endhint %}

{% hint style="warning" %}
Lojas físicas serão removidas quando a proteção for excluida!
{% endhint %}

{% hint style="warning" %}
Lojas serão removidas na próxima interação caso o dono não tenha mais permissão no terreno.
{% endhint %}

## Placa de Loja

As placas de loja permitem que os jogadores criem suas próprias lojas para vender e comprar itens de outros jogadores de forma simples e automática.\
Uma mesma loja pode vender itens, comprar itens ou fazer as duas ações ao mesmo tempo, todas as transações são feitas pelo jogador usando Coins ou Cashs, conforme configurada na placa da loja.

### Criação

Criar uma placa de loja é bem simples.

1. Segure o item na mão principal que quer vender, comprar ou fazer os dois.
2. Agache e bata em um baú ou barril.
3. Após isso, uma tela será aberta solicitando o valor que deseja vender o item.
4. Informe o valor que deseja vender o item e confirme. (Mesmo que for apenas comprar itens de outros jogadores, é necessário informar um valor aqui, mas é possível alterar isso depois.)
5. Pronto, você já tem uma placa vendendo item. (Por padrão, a placa é criada com a moeda Coins.)

{% hint style="warning" icon="light-emergency" %}
**IMPORTANTE**

O valor informado tanto na compra, quanto na venda é sempre do valor da unidade, ou seja, é o valor de 1 item, a quantidade, quem escolhe é o cliente.

Por exemplo, se você informar o valor de 500 Coins, cada unidade daquele item será vendida por 500 coins, independente da quantidade do item que você estava segurando no momento da criação.
{% endhint %}

### Gerenciamento

O dono da placa ao clicar nela, abre um menu gerencia da placa, permitindo alterar as configurações a qualquer momento.\
Por meio desse menu é possível configurar preços, moeda, compras, notificações, cupons, entre outros.

#### **Moeda**

Define qual moeda será usada nas compras e vendas, sendo elas, Coins e Cash, mas não é possível selecionar uma moeda diferente para compra e venda na mesma placa.

#### **Preço de Venda**

Define qual é o valor  que os jogadores deverão pagar por **cada unidade** do item ao comprar na sua loja.

{% hint style="info" %}
* Caso o valor informado seja 0, a loja deixará de vender o item.
* É possível alterar o valor a qualquer momento.
* O preço informado é sempre o valor de uma unidade.
{% endhint %}

#### **Preço de Compra**

Além de vender itens, sua loja pode também comprar itens de outros jogadores, ao informar um valor maior que 0, sua loja passará a comprar o item pelo valor informado.

{% hint style="info" %}
* Caso o valor informado seja 0, a loja deixará de comprar o item.
* É possível alterar o valor a qualquer momento.
* O preço informado é sempre o valor de uma unidade.
* Sua loja pode comprar e vender ao mesmo tempo.
{% endhint %}

#### **Alterar item**

É possível trocar o item comercializado pela placa de loja, para fazer isso, segure o item desejado e clique na placa, ao abrir o menu gerencial, selecione a opção **trocar item**, após isso, a loja passará a comercializar o item que está segurando.

#### **Notificações**

O menu de notificação permite escolher quais acontecimentos da loja deverão gerar avisos para você.

#### **Histórico**

Permite consultar todas as operações realizadas nas placas.

#### **Cupom**

As lojas também possuem um sistema de cupons, permitindo que crie e gerencie descontos que poderão ser utilizados pelos clientes durante a compra. [#sistema-de-cupons](loja-fisica-dos-jogadores.md#sistema-de-cupons "mention")

{% hint style="warning" %}
Os cupons são aplicados por venda, e não por item. Por exemplo, se um cupom tiver o limite de 2 usos, ele poderá ser utilizado em duas compras distintas, independentemente do jogador adquirir um ou duzentos itens de uma vez, isso contará como apenas um uso.
{% endhint %}

#### **Estado da Loja**

Permite ativar e desativar a venda de itens sem precisar excluir a placa de loja.

### Utilizando uma Loja

Uma loja pode permitir as duas operações:

* Comprar da loja: Você paga ao proprietário e recebe o item.
* Vender para a loja: Você entrega o item e recebe o pagamento do proprietário.

As ações utilizadas para abrir cada menu podem variar conforme a plataforma que você jogue, mas por padrão é:

* Interagir com a placa (Botão direito do mouse) → Comprar da loja.
* Atacar a placa (Botão esquerdo do mouse) → Vender para a loja.

{% hint style="info" %}
Caso a placa só realize uma opção, pode não ser exigido que execute uma ação específica, por exemplo, se a placa só compra item do jogador, pode ser que ao interagir com a placa(Botão direito) abra o menu para você vender um item para o dono da loja, pois não existe a ação de comprar o item da loja.
{% endhint %}

### Comprando de uma loja

Utilize a ação de interagir (Botão direito do mouse) com a placa para abrir o menu de compra, nesse menu serão exibidas todas as informações necessárias para comprar o item.

#### Item

Na parte superior, será exibido o **item que está sendo vendido pela loja.**

#### Preço

Logo abaixo serão exibidos, a moeda, valor e quantidade selecionada para a compra do item pelo cliente.

{% hint style="info" %}
O valor é atualizado automaticamente ao selecionar a quantidade ou aplicar um cupom.
{% endhint %}

#### Quantidade

É possível escolher a quantidade de **itens que deseja comprar**, ao alterar a quantidade, o valor será atualizado automaticamente na linha de cima.

#### Cupom

Caso você tenha um cupom válido da placa, poderá usar ele para obter descontos, é só usar a opção de **aplicar cupom**, após isso, irá exibir uma tela solicitando o código do cupom, após a confirmação, caso o cupom seja **válido**, o sistema aplicará o desconto e o valor da compra será atualizado automaticamente.

#### Finalização

Na ultima linha, terá a opção de  confirmar ou cancelar a compra, ao confirmar, o sistema irá validar a quantidade de itens e a quantidade de coins estando tudo certo, a transação é realizada.

{% hint style="success" %}
&#x20;**Coins adicionados para o dono da placa e item adicionado no inventário do cliente.**
{% endhint %}

### Vendendo um item para a loja

Utilize a ação de atacar(Botão esquerdo do mouse) a placa para abrir o menu de venda, nesse menu será exibidas todas as informações necessárias para vender um item.

#### Item

Na parte superior, será exibido o **item que está sendo comprado pela loja.**

#### Preço

Logo abaixo serão exibidos, a moeda, valor e quantidade selecionada para a venda do item pelo cliente.

{% hint style="info" %}
O valor é atualizado automaticamente ao selecionar a quantidade.
{% endhint %}

#### Quantidade

É possível escolher a quantidade de **itens que deseja vender para a loja**, ao alterar a quantidade, o valor será atualizado automaticamente na linha de cima.

#### Finalização

Na ultima linha, terá a opção de  confirmar ou cancelar a venda do item para a loja, ao confirmar, o sistema irá validar a quantidade de itens e a quantidade de coins, e estando tudo certo, a transação é realizada.

{% hint style="success" %}
&#x20;**Coins adicionados para o cliente e item enviado para o dono pela placa.**
{% endhint %}

## Comandos

<table><thead><tr><th width="370">Comando</th><th width="382">Descrição</th></tr></thead><tbody><tr><td>/lojaplaca</td><td>Lista todas as suas placas.</td></tr><tr><td>/lojaplaca history</td><td>Lista todas as compras e vendas em todas as suas placas.</td></tr><tr><td>/pw ir &#x3C;pwarp></td><td>Teleporta até uma pwarp.</td></tr><tr><td>/pw definir &#x3C;pwarp></td><td>Cria um ponto de teleporte no local atual. Existe um custo 500.000 coins.</td></tr><tr><td>/pw remover &#x3C;pwarp></td><td>Deleta o ponto de teleporte especificado.</td></tr><tr><td>/pw desc definir &#x3C;pwarp> &#x3C;descrição></td><td>Adiciona uma descrição a pwarp especificada.</td></tr><tr><td>/pw desc remover &#x3C;pwarp></td><td>Remove a descrição da pwarp especificada.</td></tr><tr><td>/pw icon definir &#x3C;pwarp></td><td>Define como ícone, o item que estiver segurando.</td></tr><tr><td>/pw icon remover &#x3C;pwarp></td><td>Remove o ícone da sua pwarp...</td></tr><tr><td>/pw categoria definir &#x3C;pwarp> &#x3C;categoria></td><td>Define uma categoria para a sua pwarp. Categorias disponíveis, Cidades, Construção, Farms, Livros, Lojas, Map-Arts, Minérios, Outras e Poções. Por padrão, a loja é criada na categoria Outras.</td></tr><tr><td>/pw categoria listar &#x3C;pwarp> </td><td>Exibe no chat a categoria atual da loja.</td></tr><tr><td>/pw redefinir &#x3C;pwarp></td><td>Muda o local de teleporte para o seu local atual. Nenhum dado é perdido. Existe um custo de 25.000 coins.</td></tr><tr><td>/pw ban definir &#x3C;pwarp> &#x3C;jogador></td><td>Bane o jogador da pwarp especificada, não permitindo teleportar via pwarp.</td></tr><tr><td>/pw ban remover &#x3C;pwarp> &#x3C;jogador></td><td>Remove o banimento do jogador na pwarp informada.</td></tr><tr><td>/pw ban listar &#x3C;pwarp></td><td>Lista todos os banimentos da pwarp especificada.</td></tr><tr><td>/pw senha definir &#x3C;pwarp> &#x3C;senha></td><td>Define uma senha para a pwarp especificada.</td></tr><tr><td>/pw senha remover &#x3C;pwarp></td><td>Remove a senha da pwarp especificada.</td></tr><tr><td>/pw bloquear &#x3C;pwarp></td><td>Bloqueia/Desbloqueia jogadores poderem teleportar para a pwarp especificada.</td></tr><tr><td>/pw favoritar &#x3C;pwarp></td><td>Adiciona ou remove a pwarp da sua lista de favoritas.</td></tr><tr><td>/pw avaliar &#x3C;pwarp> &#x3C;nota></td><td>Avalie a pwarp especificada com nota de 1 a 5.</td></tr><tr><td>/pw info &#x3C;pwarp></td><td>Exibe no chat as informações da pwarp.</td></tr><tr><td>/pw</td><td>Abre o menu.</td></tr></tbody></table>



## Sistema de Cupons

Aprimore sua estratégia de marketing criando e distribuindo cupons de desconto para os clientes da sua loja, atraindo assim um maior fluxo de visitantes e potencializando suas vendas.

### Como ativo um cupom de loja para poder usar?

Selecionado uma placa vendendo um item, será possível adicionar o cupom na parte inferior, ao clicar abrirá um outro menu solicitando o cupom, ao aplicar, o sistema irá verificar se o cupom é válido e aplicar ele na venda atual. Em casos onde o cupom seja inválido ou expirado, nenhum desconto será aplicado.

### Como crio um cupom?

Selecionado a placa é possível criar cupons pelo menu, para isso, ao selecionar a opção cupons, abrirá um menu listando todos os cupons ativos, juntamente com 2 opções, uma para criar um cupom ilimitado, qualquer jogador poderá usar enquanto ele estiver ativo, sendo necessário informar apenas o código do cupom e o percentual de desconto, a outra opção é o cupom limitado, por enquanto só é possível limitar por uso\*,  sendo necessário informar o código, percentual de desconto e o número máximo de usos.

{% hint style="info" %}
\*O cupom limitado, é limitado por uso, não por item, ele contará um uso sendo um item ou sendo cem itens.
{% endhint %}

#### Como deleto um cupom?

É possível deletar um cupom pelo menu administrativo da placa.

