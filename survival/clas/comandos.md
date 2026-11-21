---
description: Lista com todos os comandos do sistema de clans.
icon: rectangle-terminal
---

# Comandos



{% hint style="info" icon="question" %}
Dicas para interpretar esta página:

<> Argumento obrigatório.

\[] Argumento opcional.

\| Argumento limitado por opções.
{% endhint %}

## Comandos

### Comandos iniciais

<table data-header-hidden="false" data-header-sticky><thead><tr><th width="273">Comando</th><th>Descrição</th><th data-hidden>Permissão</th><th data-hidden>Comando para permissão</th></tr></thead><tbody><tr><td>/clan guia</td><td>Abre o livro que explica o sistema de clãs.</td><td>Qualquer jogador</td><td>Qualquer jogador</td></tr><tr><td>/clan criar &#x3C;tag> &#x3C;nome></td><td>Cria um clã com a tag e o nome escolhidos.*</td><td>Qualquer jogador</td><td>Qualquer jogador</td></tr><tr><td>/clan entrar &#x3C;tag></td><td>Entra em um clã público ou envia um pedido de entrada.</td><td>Qualquer jogador</td><td>Qualquer jogador</td></tr><tr><td>/clan convites</td><td>Lista os convites que você recebeu.</td><td>Qualquer jogador</td><td>Qualquer jogador</td></tr><tr><td>/clan aceitar &#x3C;tag></td><td>Aceita o convite do clã indicado.</td><td>Qualquer jogador</td><td>Qualquer jogador</td></tr><tr><td>/clan recusar &#x3C;tag></td><td>Recusa o convite do clã indicado.</td><td>Qualquer jogador</td><td>Qualquer jogador</td></tr><tr><td>/clan perfil [tag]</td><td>Mostra o perfil do clã indicado.(Se não informar, retorna o perfil do seu clan)</td><td>Qualquer jogador</td><td>Qualquer jogador</td></tr><tr><td>/clan online [public|request]</td><td>Lista clãs com membros online. Use public para filtrar os públicos ou request para ver os que recebem pedidos de entrada.</td><td>Qualquer jogador</td><td>Qualquer jogador</td></tr><tr><td>/clan ranking [kdr|bank]</td><td>Mostra a classificação dos clãs. Use kdr para ordenar por kdr ou use bank para ordenar por saldo no banco.</td><td>Qualquer jogador</td><td>Qualquer jogador</td></tr></tbody></table>

{% hint style="info" %}
\*Existe um custo de 500.000 Coins por clan criado.
{% endhint %}

### Membros

<table data-header-hidden="false" data-header-sticky><thead><tr><th width="258">Comando</th><th>Descrição</th><th data-hidden>Permissão</th><th data-hidden>Comando para permissão</th></tr></thead><tbody><tr><td>/clan convidar &#x3C;jogador></td><td>Convida um jogador para o seu clã.</td><td><code>INVITE_MEMBERS</code></td><td><code>/clan permissao &#x3C;cargo> INVITE_MEMBERS</code></td></tr><tr><td>/clan pedidos</td><td>Lista os jogadores que pediram para entrar no clã.</td><td>Qualquer jogador</td><td>Qualquer jogador</td></tr><tr><td>/clan aprovar &#x3C;jogador></td><td>Aprova o pedido de entrada de um jogador.</td><td><code>INVITE_MEMBERS</code></td><td><code>/clan permissao &#x3C;cargo> INVITE_MEMBERS</code></td></tr><tr><td>/clan rejeitar &#x3C;jogador></td><td>Recusa o pedido de entrada de um jogador.</td><td><code>INVITE_MEMBERS</code></td><td><code>/clan permissao &#x3C;cargo> INVITE_MEMBERS</code></td></tr><tr><td>/clan membros [tag]</td><td>Lista os membros do clan especificado ou o seu, caso não informe nenhum. </td><td>Qualquer jogador</td><td>Qualquer jogador</td></tr><tr><td>/clan expulsar &#x3C;jogador></td><td>Expulsa um membro do clã.</td><td><code>KICK_PLAYERS</code></td><td><code>/clan permissao &#x3C;cargo> KICK_PLAYERS</code></td></tr><tr><td>/clan transferir &#x3C;jogador></td><td>Transfere a liderança do clã para outro membro.</td><td>APENAS FUNDADOR</td><td>APENAS FUNDADOR</td></tr><tr><td>/clan abandonar</td><td>Faz você sair do clã.</td><td>Qualquer jogador</td><td>Qualquer jogador</td></tr><tr><td>/clan debandar</td><td>Dissolve o clã permanentemente.</td><td>APENAS FUNDADOR</td><td>APENAS FUNDADOR</td></tr></tbody></table>

### Cargos e permissões

<table data-header-hidden="false" data-header-sticky><thead><tr><th width="375">Comando</th><th>Descrição</th><th data-hidden>Permissão</th><th data-hidden>Comando para permissão</th></tr></thead><tbody><tr><td>/clan cargos</td><td>Abre o menu de cargos e permissões.</td><td>Qualquer jogador</td><td>Qualquer jogador</td></tr><tr><td>/clan cargo &#x3C;jogador> &#x3C;cargo></td><td>Altera o cargo de um membro.</td><td><code>MANAGE_ROLES</code></td><td><code>/clan permissao &#x3C;cargo> MANAGE_ROLES</code></td></tr><tr><td>/clan cargopermissoes &#x3C;cargo> &#x3C;permissão></td><td>Ativa ou desativa uma permissão do cargo indicado.</td><td><code>MANAGE_ROLES</code></td><td><code>/clan permissao &#x3C;cargo> MANAGE_ROLES</code></td></tr><tr><td>/clan cargocriar &#x3C;nome></td><td>Cria um cargo com o nome escolhido.</td><td><code>MANAGE_ROLES</code></td><td><code>/clan permissao &#x3C;cargo> MANAGE_ROLES</code></td></tr><tr><td>/clan cargonome &#x3C;cargo> &#x3C;nome></td><td>Altera o nome de um cargo.</td><td><code>MANAGE_ROLES</code></td><td><code>/clan permissao &#x3C;cargo> MANAGE_ROLES</code></td></tr><tr><td>/clan cargotag &#x3C;cargo> &#x3C;tag-rgb|reset></td><td>Define a tag colorida do cargo no chat. Use reset para restaurar a exibição padrão.</td><td><code>MANAGE_ROLES</code></td><td><code>/clan permissao &#x3C;cargo> MANAGE_ROLES</code></td></tr><tr><td>/clan cargopeso &#x3C;cargo> &#x3C;peso></td><td>Define o peso do cargo na hierarquia. Cargos de peso maior podem gerenciar cargos de peso menor quando têm a permissão necessária. Peso mínimo 1, máximo 49.</td><td><code>MANAGE_ROLES</code></td><td><code>/clan permissao &#x3C;cargo> MANAGE_ROLES</code></td></tr><tr><td>/clan cargodeletar &#x3C;cargo></td><td>Exclui um cargo criado pelo clã.</td><td><code>MANAGE_ROLES</code></td><td><code>/clan permissao &#x3C;cargo> MANAGE_ROLES</code></td></tr></tbody></table>

### Banco e taxa

<table data-header-hidden="false" data-header-sticky><thead><tr><th width="328">Comando</th><th>Descrição</th><th data-hidden>Permissão</th><th data-hidden>Comando para permissão</th></tr></thead><tbody><tr><td>/clan banco</td><td>Abre o banco do clã.</td><td>Qualquer jogador</td><td>Qualquer jogador</td></tr><tr><td>/clan bancodepositar &#x3C;valor></td><td>Transfere Coins do seu saldo para o banco do clã. O depósito mínimo é de 100 Coins.</td><td><code>DEPOSIT_MONEY</code></td><td><code>/clan permissao &#x3C;cargo> DEPOSIT_MONEY</code></td></tr><tr><td>/clan bancosacar &#x3C;valor></td><td>Retira Coins do banco do clã.</td><td><code>WITHDRAW_MONEY</code></td><td><code>/clan permissao &#x3C;cargo> WITHDRAW_MONEY</code></td></tr><tr><td>/clan bancoextrato</td><td>Mostra as entradas e saídas do banco do clã.</td><td>Qualquer jogador</td><td>Qualquer jogador</td></tr><tr><td>/clan fidelidade &#x3C;valor></td><td>Define quanto cada membro paga ao clã como taxa de fidelidade. </td><td>APENAS FUNDADOR</td><td>APENAS FUNDADOR</td></tr><tr><td>/clan intervalofidelidade &#x3C;horas></td><td>Define o intervalo, em horas, entre as cobranças da taxa de fidelidade.*</td><td>APENAS FUNDADOR</td><td>APENAS FUNDADOR</td></tr></tbody></table>

{% hint style="info" %}
\*O intervalo pode ser definido de 24 a 720 horas, cada alteração demora 1 dia para ser efetivada.
{% endhint %}

### Baú e evolução

<table data-header-hidden="false" data-header-sticky><thead><tr><th width="334">Comando</th><th>Descrição</th><th data-hidden>Permissão</th><th data-hidden>Comando para permissão</th></tr></thead><tbody><tr><td>/clan bau [página]</td><td>Abre o baú compartilhado na página indicada. Para guardar ou retirar itens, o cargo precisa de ACCESS_CHEST.</td><td><code>VIEW_CHEST</code></td><td><code>/clan permissao &#x3C;cargo> VIEW_CHEST</code></td></tr><tr><td>/clan bauregistro</td><td>Mostra quem guardou ou retirou itens do baú.</td><td>Qualquer jogador</td><td>Qualquer jogador</td></tr><tr><td>/clan evoluir &#x3C;nivel|aliado|rival></td><td>Melhora o clã. A opção escolhida aumenta a capacidade de membros, aliados ou rivais.</td><td><code>UPGRADE_CLAN</code></td><td><code>/clan permissao &#x3C;cargo> UPGRADE_CLAN</code></td></tr><tr><td>/clan mercado &#x3C;reset-kdr></td><td>Permite comprar vantagens no mercado do clã.</td><td><code>MARKET_BUY</code></td><td><code>/clan permissao &#x3C;cargo> MARKET_BUY</code></td></tr></tbody></table>

### Home, Base e relações

<table data-header-hidden="false" data-header-sticky><thead><tr><th width="252">Comando</th><th>Descrição</th><th data-hidden>Permissão</th><th data-hidden>Comando para permissão</th></tr></thead><tbody><tr><td>/clan home</td><td>Teleporta você para a home do seu clã.</td><td><code>HOME_GO</code></td><td><code>/clan permissao &#x3C;cargo> HOME_GO</code></td></tr><tr><td>/clan home &#x3C;tag></td><td>Teleporta você para a home do clã indicado, desde que ela seja pública.</td><td>Qualquer jogador</td><td>Qualquer jogador</td></tr><tr><td>/clan sethome</td><td>Define a home do clã na sua posição por 50.000 Coins. Se já houver uma home, a nova posição substitui a anterior.*</td><td><code>HOME_SET</code></td><td><code>/clan permissao &#x3C;cargo> HOME_SET</code></td></tr><tr><td>/clan delhome</td><td>Remove a home do clã.</td><td><code>HOME_DELETE</code></td><td><code>/clan permissao &#x3C;cargo> HOME_DELETE</code></td></tr><tr><td>/clan publichome</td><td>Torna a home pública/privada para que outros jogadores possam visitá-la usando /clan home &#x3C;tag>.</td><td><code>HOME_SET</code></td><td><code>/clan permissao &#x3C;cargo> HOME_SET</code></td></tr><tr><td>/clan reagrupar</td><td>Chama os membros online para a base do clã.</td><td><code>HOME_SET</code></td><td><code>/clan permissao &#x3C;cargo> HOME_SET</code></td></tr><tr><td>/clan reagruparaceitar</td><td>Aceita uma solicitação de agrupamento.</td><td>Qualquer jogador</td><td>Qualquer jogador</td></tr><tr><td>/clan aliado add &#x3C;tag></td><td>Envia um pedido de aliança ou aceita um pedido do clã indicado.</td><td><code>ALLY_ADD</code></td><td><code>/clan permissao &#x3C;cargo> ALLY_ADD</code></td></tr><tr><td>/clan aliado remove &#x3C;tag></td><td>Encerra a aliança ou recusa um pedido do clã indicado.</td><td><code>ALLY_REMOVE</code></td><td><code>/clan permissao &#x3C;cargo> ALLY_REMOVE</code></td></tr><tr><td>/clan rival [tag]</td><td>Declara ou encerra uma rivalidade.**</td><td><code>RIVAL_ADD</code> / <code>RIVAL_REMOVE</code></td><td>Declarar rivalidade: <code>/clan permissao &#x3C;cargo> RIVAL_ADD</code><br>Encerrar rivalidade: <code>/clan permissao &#x3C;cargo> RIVAL_REMOVE</code></td></tr></tbody></table>

{% hint style="info" %}
\*O saldo é descontado do banco do clan.

\*\*Cada ação usa a permissão correspondente, sendo RIVAL\_ADD para declarar rivalidade e RIVAL\_REMOVE para encerrar um rivalidade.
{% endhint %}

### Chat e mural

<table data-header-hidden="false" data-header-sticky><thead><tr><th width="247">Comando</th><th>Descrição</th><th data-hidden>Permissão</th><th data-hidden>Comando para permissão</th></tr></thead><tbody><tr><td>/. &#x3C;mensagem></td><td>Envia uma mensagem apenas ao seu clan.</td><td>Qualquer jogador</td><td>Qualquer jogador</td></tr><tr><td>/a &#x3C;mensagem></td><td>Envia uma mensagem aos aliados.</td><td>Qualquer jogador</td><td>Qualquer jogador</td></tr><tr><td>/clan canal</td><td>Fixa o canal de conversa para enviar as próximas mensagens ao clã ou aos aliados.</td><td>Qualquer jogador</td><td>Qualquer jogador</td></tr><tr><td>/clan avisos</td><td>Mostra os avisos publicados no mural do clã.</td><td>Qualquer jogador</td><td>Qualquer jogador</td></tr><tr><td>/clan avisar &#x3C;mensagem></td><td>Publica uma mensagem de até 100 caracteres no mural. Você pode usar cores de /cores ou em <a href="../../ajuda/cores-rgb.md">HEX</a>.*</td><td><code>NEWSLETTER_ADD</code></td><td><code>/clan permissao &#x3C;cargo> NEWSLETTER_ADD</code></td></tr></tbody></table>

{% hint style="info" %}
\*Os códigos de cor contam para o limite.
{% endhint %}

### Configurações

<table data-header-hidden="false" data-header-sticky><thead><tr><th width="358">Comando</th><th>Descrição</th><th data-hidden>Permissão</th><th data-hidden>Comando para permissão</th></tr></thead><tbody><tr><td>/clan descricao &#x3C;descrição></td><td>Altera a descrição do clã. O texto deve ter de 10 a 40 caracteres, sem contar os códigos de cor.</td><td>APENAS FUNDADOR</td><td>APENAS FUNDADOR</td></tr><tr><td>/clan modtag &#x3C;HEX cor|reset|codigo rgb></td><td>Personaliza a exibição da tag com cores e negrito, preservando as letras da tag.</td><td><code>CUSTOM_TAG_CHANGE</code></td><td><code>/clan permissao &#x3C;cargo> CUSTOM_TAG_CHANGE</code></td></tr><tr><td>/clan banner</td><td>Define o estandarte que você segura como bandeira do clã.*</td><td><code>BANNER_CHANGE</code></td><td><code>/clan permissao &#x3C;cargo> BANNER_CHANGE</code></td></tr><tr><td>/clan bannerremover</td><td>Remove a bandeira do clã.</td><td><code>BANNER_CHANGE</code></td><td><code>/clan permissao &#x3C;cargo> BANNER_CHANGE</code></td></tr><tr><td>/clan entrada</td><td>Define o modo de entrada. No público, o jogador entra diretamente. Por pedido, ele solicita a entrada e aguarda aprovação. No privado, precisa receber um convite. Apenas o membro fundador pode mudar o modo.</td><td>APENAS FUNDADOR</td><td>APENAS FUNDADOR</td></tr><tr><td>/clan fogoamigo membros</td><td>Ativa ou desativa o dano entre membros do próprio clã.</td><td><code>FF_MEMBER_CHANGE</code></td><td><code>/clan permissao &#x3C;cargo> FF_MEMBER_CHANGE</code></td></tr><tr><td>/clan fogoamigo aliados</td><td>Ativa ou desativa o dano entre membros do clã e seus aliados.</td><td><code>FF_ALLY_CHANGE</code></td><td><code>/clan permissao &#x3C;cargo> FF_ALLY_CHANGE</code></td></tr></tbody></table>

{% hint style="info" %}
\*Custa 1.000.000 de Coins e são descontados do banco do clan.
{% endhint %}

## Permissões

Para definir ou remover uma permissão para um cargo use `/clan permissao <cargo> <permissão>`.  se o cargo já tiver a permissão ela será removido, caso contrário, ela será definida.&#x20;

Cada permissão define o que os membros do cargo podem fazer, nas tabelas de comando, os definidos como "Qualquer  Jogador" indica que o comando não exige nenhuma permissão de cargo.&#x20;

### Listagem

<table data-header-hidden="false" data-header-sticky><thead><tr><th width="214">Permissão</th><th>Descrição</th></tr></thead><tbody><tr><td>KICK_PLAYERS</td><td>Expulsar jogadores do clã.</td></tr><tr><td>INVITE_MEMBERS</td><td>Convidar jogadores e aprovar ou recusar pedidos de entrada.</td></tr><tr><td>ACCESS_CHEST</td><td>Colocar e retirar itens do baú do clã.</td></tr><tr><td>VIEW_CHEST</td><td>Consultar o conteúdo do baú do clã.</td></tr><tr><td>DEPOSIT_MONEY</td><td>Depositar Coins no banco do clã.</td></tr><tr><td>WITHDRAW_MONEY</td><td>Sacar Coins do banco do clã.</td></tr><tr><td>HOME_GO</td><td>Teleportar para a home do clã.</td></tr><tr><td>NEWSLETTER_ADD</td><td>Publicar um aviso no mural do clã.</td></tr><tr><td>RIVAL_REMOVE</td><td>Remover um clã da lista de rivais.</td></tr><tr><td>RIVAL_ADD</td><td>Adicionar um clã à lista de rivais.</td></tr><tr><td>ALLY_REMOVE</td><td>Encerrar uma aliança ou recusar um pedido.</td></tr><tr><td>ALLY_ADD</td><td>Enviar ou aceitar um pedido de aliança.</td></tr><tr><td>HOME_DELETE</td><td>Remover o ponto de teleporte da base do clã.</td></tr><tr><td>HOME_SET</td><td>Definir a home, torná-la pública e chamar os membros online para a base.</td></tr><tr><td>FF_MEMBER_CHANGE</td><td>Ativar ou desativar o fogo amigo entre membros do próprio clã.</td></tr><tr><td>FF_ALLY_CHANGE</td><td>Ativar ou desativar o fogo amigo entre o clã e seus aliados.</td></tr><tr><td>CUSTOM_TAG_CHANGE</td><td>Personalizar as cores e o negrito da tag do clã.</td></tr><tr><td>BANNER_CHANGE</td><td>Alterar o estandarte do clã.</td></tr><tr><td>MANAGE_ROLES</td><td>Gerenciar os cargos do clã.</td></tr><tr><td>UPGRADE_CLAN</td><td>Aumentar a capacidade de membros, aliados ou rivais.</td></tr><tr><td>MANAGE_MISSIONS</td><td>Gerenciar as missões do clã.</td></tr><tr><td>MARKET_BUY</td><td>Fazer compras no mercado do clã.</td></tr><tr><td>FEE_ALERTS</td><td>Receber a lista de membros que não pagaram a taxa de fidelidade do clã.</td></tr></tbody></table>

### Hierarquia

Um grupo com MANAGE\_ROLES pode alterar o cargo de jogadores que estejam abaixo dele na hierarquia, ao editar um cargo de peso menor, só poderá ser alteradas as permissões que o próprio cargo possuí. Exemplo:\
Se o seu cargo tiver MANAGE\_ROLES e HOME\_SET, você poderá alterar HOME\_SET em um grupo de peso menor, mas se quiser alterar HOME\_DELETE, o seu cargo precisará ter essa mesma permissão, caso contrário, não será possível alterar.&#x20;
