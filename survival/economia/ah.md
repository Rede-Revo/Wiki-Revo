---
description: Menu onde jogadores podem vender e comprar itens.
---

# 🛒 Mercado

## O que é o Mercado? <a href="#criar-uma-loja" id="criar-uma-loja"></a>

O mercado é um sistema que permite aos jogadores comprar e anunciar itens para a venda de maneira simples, sem precisar visitar uma loja. Ele pode ser acessado de qualquer lugar\*, e as negociações podem ser realizadas usando as duas moedas disponíveis no servidor, Coins ou Cash.



## Comandos



| Comando                                        | Descrição                                                                                                                                                                                           |
| ---------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| /ah                                            | Abre o menu com todos os itens anunciados                                                                                                                                                           |
| /ah open \[menu]                               | Abre o menu especificado, caso não informe nenhum abrirá o menu padrão, main.                                                                                                                       |
| /ah sell \<valor> \<quantidade> \<Coins\|Cash> | Anuncia o item que estiver segurando pelo valor, quantidade e moeda informada.                                                                                                                      |
| /ah search \[pesquisa]                         | Inicia uma pesquisa dos itens anunciados atualmente. É possível pesquisar por nome, descrição, material ou nick. Caso não informe uma pesquisa, o sistema abrirá uma placa para inserir a pesquisa. |
| /ah view \[nick]                               | Exibe todos os itens anunciados pelo jogador especificado, caso não informe nenhum jogador, o sistema abrirá seus itens anunciados.                                                                 |
| /ah history                                    | Exibe o histórico de todos os itens vendidos. É exibido os itens de todos os jogadores.                                                                                                             |
| /ah deleted                                    | Abre um menu exibindo todos os itens excluídos pelo sistema.                                                                                                                                        |

{% hint style="info" %}
Todas as vendas realizadas em Coins será cobrado uma taxa de 5% sobre o valor total. Vendas realizadas em cash não tem cobrança de taxa.
{% endhint %}

## Expiração

Os itens serão expirados após 7 dias da data de criação do anúncio e estarão disponíveis para resgate do proprietário no menu dos seus anúncios.

{% hint style="warning" %}
## ATENÇÃO

Após 30 dias, os itens serão excluídos permanentemente e não poderão ser recuperados.
{% endhint %}

<sup><sub>\*Mercado não está disponível no mundo de eventos.<sub></sup>
