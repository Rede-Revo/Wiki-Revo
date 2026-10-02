---
icon: key
---

# Autenticação Java

## Introdução

Os jogadores da versão Java podem possuir contas registradas no servidor como originais ou piratas, o tipo de registro da conta define a forma de autenticação(Login) usado para entrar no servidor.&#x20;

{% hint style="info" %}
O tipo do UUID da conta é definido em seu primeiro registro no servidor e não é alterado ao mudar a forma de autenticação, isso significa que uma conta registrada como pirata em seu primeiro login continuará usando o UUID pirata mesmo após ativar a autenticação original, dessa mesma forma, uma conta registrada como original continuará usando um UUID original mesmo após ser alterado a forma de autenticação para pirata.&#x20;
{% endhint %}

{% hint style="info" %}
O UUID funciona como a identidade da sua conta. é ele que garante que todos os seus itens, terrenos, pets, tags, homes, pwarps e progressos continuem salvos com você, independentemente de você trocar de nick ou alterar sua conta entre original e pirata.
{% endhint %}

## Conta pirata para original

Caso você possua uma conta registrada no servidor como pirata e posteriormente adquira uma conta original usando o mesmo nick, você poderá ativar a autenticação original diretamente pelo servidor, usando o comando <kbd>/premium \<senha></kbd> , essa senha é a cadastrada no momento do registro da conta, após executar o comando, você será desconectado do servidor e no seu próximo acesso, o sistema tentará validar sua conta através da autenticação oficial da Mojang, caso a validação ocorra com sucesso, os próximos acessos utilizarão a autenticação da conta original.

Mas caso você tente realizar o acesso sem estar devidamente autenticado em uma conta original, será exibido um erro informando que a conta não esta autenticada no Minecraft, como mecanismo de segurança, caso a alteração para a conta original não seja concluída,  a conta voltará a ser identificada como pirata, permitindo que o jogador continue jogando normalmente.&#x20;

{% hint style="warning" %}
### **ATENÇÃO**

O comando <kbd>/premium \<senha></kbd> deve ser utilizado apenas pelo proprietário da conta e somente quando possuir acesso a uma conta original com o mesmo nick.&#x20;
{% endhint %}

{% hint style="warning" %}
### **ATENÇÃO**

Uma vez a conta registrada como pirata, ela sempre será pirata, ou seja, trocar o nick na Mojang após usar o comando de conversão de autenticação, os dados não serão passados para o novo nick.
{% endhint %}

## Conta original para pirata

A conversão de uma conta registrada como original para uma autenticação pirata, não pode ser realizada diretamente pelo jogador.

O procedimento para conversão de autenticação original para pirata é realizado gratuitamente pela Staff e somente em situações especificas, mediante abertura de ticket e a comprovação do ocorrido.

A conversão só poderá ser analisada nos seguintes casos:

* Perda ou bloqueio do acesso a sua conta Microsoft.
* Problemas após a alteração do nick da conta original.

{% hint style="info" %}
A solicitação passará por análise da equipe mesmo que cumpram todos os requisitos acima, ou seja, cumprir esses requisitos não garante que sua conta será convertida em autenticação pirata.&#x20;
{% endhint %}

### Alteração de nick para um já registrado

Antes de alterar seu nick da sua conta original, é necessário verificar se o novo nick que você deseja trocar não está registrado no Servidor, caso você altere seu nick no Minecraft para um já registrado no servidor, o sistema de proteção impedirá que os dados da conta anterior sejam transferidos para esse novo nick.

Nessa situação, você poderá solicitar a conversão da autenticação da sua conta original para autenticação pirata, mas isso só vai permitir que você consiga acessar sua conta no nick antigo.

{% hint style="info" %}
A existência de registro não depende do jogador ter acessado o Survival, ou seja, comando dentro do survival não garantem que o nick não possui registro no servidor.

Um jogador pode ter registro no servidor e nunca ter entrado no Survival. Para fins de propriedade da conta no servidor, será considerado o jogador que registrou primeiro o nick.
{% endhint %}

### Mudanças na conta

Quando uma conta original é convertida para autenticação pirata:

* O UUID original é preservado .
* Nenhum progresso é transferido para outra conta(UUID).
* Os dados permanecem vinculados na mesma conta(UUID).
* A validação de conta pelo Minecraft/Mojang deixa de ser exigida.
* O acesso a conta passa exigir a senha cadastrada no servidor.

Ou seja, o procedimento não é uma transferência  de conta, é apenas uma forma de mudar a forma usada para autenticar no servidor.

### Esqueci minha senha

A senha usada após a conversão é a mesma cadastrada no seu primeiro acesso ao servidor, caso tenha esquecido sua senha temos uma página explicando o passo a passo de como recuperar o acesso. [recuperacao.md](recuperacao.md "mention")

## Condições para contas originais convertidas para pirata

Contas registradas como originais e posteriormente convertidas para autenticação pirata, são destinadas exclusivamente ao uso pessoal.

Após a conversão, é proibido:

* Compartilhar o acesso à conta.
* Emprestar a conta.
* Vender ou doar a conta.
* Fornecer a senha ou permitir o acesso de terceiros.

{% hint style="info" %}
Ao solicitar a conversão da autenticação original para pirata, você declara estar ciente e de acordo com essas condições
{% endhint %}

{% hint style="danger" %}
## **IMPORTANTE**

Caso seja identificado o compartilhamento, empréstimo, venda, doação, acesso a terceiros ou qualquer ação proibida citado acima, a conta será bloqueada permanentemente.&#x20;

Caso o proprietário considere que o bloqueio ocorreu de forma incorreta, poderá abrir um ticket para explicar a situação e solicitar uma novo análise.
{% endhint %}

## Contas originalmente registradas como piratas

As restrições adicionais descritas acima, não se aplicam as contas registradas como piratas, essas contas continuam sujeitas normalmente as regras gerais do Servidor, inclusive as regras relacionada a venda de conta, consulte as regras para evitar problemas futuros. [regras](../regras/ "mention")

## Retornar para a autenticação de registro

O jogador poderá voltar quando achar necessário para o seu tipo de autenticação de registro, usando os comandos:

<table><thead><tr><th width="175">Comando</th><th>Descrição</th></tr></thead><tbody><tr><td>/original &#x3C;senha></td><td>Define uma conta como original.</td></tr><tr><td>/pirata &#x3C;senha></td><td>Define uma conta como pirata.</td></tr></tbody></table>

{% hint style="info" %}
Caso ocorra algum erro durante o procedimento, o jogador poderá abrir um ticket para que a equipe verifique o ocorrido.
{% endhint %}
