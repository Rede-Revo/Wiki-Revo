---
description: >-
  Como o Revonildo, o bot do Discord da Rede Revo, coleta, usa, armazena e
  protege os seus dados.
---

# Política de Privacidade do Bot

**Última atualização:** 22 de outubro de 2026

Esta política explica quais dados o **Revonildo** (o bot do Discord da **Rede Revo**) trata, para que, por quanto tempo e quais são os seus direitos. Ela vale para o bot no servidor de Discord da Rede Revo e no servidor da equipe. Para o servidor de Minecraft e o site, valem os [Termos de Uso e Serviço](/broken/pages/c96fe1ad8cf68d5253e8ce842a40192cb62d4db2).

{% hint style="info" %}
**Resumo rápido**

* O bot só trata dados para fazer as funções que você vê no servidor: tickets, denúncias, sugestões, ranking, sorteios, logs de moderação e o assistente de IA.
* **Não vendemos nem compartilhamos seus dados** com anunciantes.
* O assistente de IA responde com base na **wiki pública** e **não** é usado para punir ninguém.
* Você pode pedir acesso, correção ou exclusão dos seus dados a qualquer momento (veja [Seus direitos](/broken/pages/983872f1e67f348457dffc9e869abbdd2cae3c1d#seus-direitos)).
{% endhint %}

## Quem somos

O controlador dos dados é a **Rede Revo**, responsável pelo servidor e pelo bot.

* Site: [rederevo.com](https://rederevo.com/)
* Wiki: [wiki.rederevo.com](https://wiki.rederevo.com/)
* Contato sobre privacidade: abra um **ticket** no Discord da Rede Revo ou escreva para **contato.rederevo@gmail.com**.

## Quais dados o bot trata

### Dados que o próprio Discord fornece

Ao interagir com o bot, ele recebe do Discord:

* seu **ID de usuário**, nome de usuário, apelido no servidor e avatar;
* seus **cargos** no servidor e a **data em que entrou** nele (usados, por exemplo, em `/userinfo` e nas checagens de permissão);
* o canal, o servidor e o horário em que você usou um comando, botão ou formulário.

### Conteúdo de mensagens

O bot lê o texto das mensagens do servidor **apenas** para as funções abaixo. Ele não faz perfil, nem análise de comportamento, nem guarda as conversas gerais.

| Função                     | O que o bot faz com a mensagem                                                                                                                                                                                                            |
| -------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Respostas automáticas      | Detecta perguntas sobre o **IP** do servidor e sobre **cupons** e responde.                                                                                                                                                               |
| Upload de logs             | Lê o filtro `localizar: <palavra>` enviado junto de um anexo `.log`, `.txt` ou `.yml` e publica o log em um serviço externo (veja [Serviços de terceiros](/broken/pages/983872f1e67f348457dffc9e869abbdd2cae3c1d#servicos-de-terceiros)). |
| Canais com regras próprias | Valida o formato das mensagens em canais de mídias, de tarefas da equipe e de divulgação.                                                                                                                                                 |
| Logs de moderação          | Mantém **em memória** (até 10.000 mensagens, apagadas ao reiniciar o bot) o texto de mensagens recentes para que a equipe veja o conteúdo de mensagens **apagadas ou editadas**.                                                          |
| Starboard                  | Copia o texto de uma mensagem para o canal de destaques quando ela recebe reações suficientes.                                                                                                                                            |
| Tickets                    | Gera a **transcrição** da conversa do ticket ao fechá-lo.                                                                                                                                                                                 |
| Assistente de IA           | Lê a pergunta feita ao bot (veja [Assistente de IA](/broken/pages/983872f1e67f348457dffc9e869abbdd2cae3c1d#assistente-de-ia)).                                                                                                            |

O sistema de **ranking** conta que você enviou uma mensagem, mas **não lê o conteúdo** dela.

### Dados que você nos envia ao usar os sistemas

| Sistema                                         | Dados armazenados                                                                                                                          |
| ----------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------ |
| **Tickets**                                     | ID e nome no Discord, canal, horário de abertura, respostas iniciais, quem atendeu e a transcrição da conversa.                            |
| **Denúncias**                                   | Seu ID e nome, o nick denunciado, o seu nick no servidor, as regras violadas, as evidências e as informações adicionais que você escrever. |
| **Apelações de punição**                        | Seu ID e nome, nick, regra, explicação e plataforma.                                                                                       |
| **Recuperação de conta**                        | Seu ID e nome, nick no jogo e as informações de verificação que você enviar (como localizações das _homes_ e **endereço IP**).             |
| **Sugestões**                                   | Seu ID e nome, local da sugestão e as respostas do formulário.                                                                             |
| **Formulários da equipe** (Ajudante/Construtor) | Seu ID e as respostas do formulário.                                                                                                       |
| **Parcerias e divulgação**                      | Seu ID, nome e os links que você informar (por exemplo, canal de YouTube ou Twitch).                                                       |
| **Sorteios**                                    | Seu ID, para registrar que você participa.                                                                                                 |
| **Ranking de XP**                               | Seu ID, o XP acumulado e o horário da última mensagem que rendeu XP. Também conta o **tempo em canais de voz**, sem gravar áudio.          |
| **Avaliação do atendimento**                    | Seu ID e a nota (1 a 5) dada ao final do ticket.                                                                                           |
| **Registro de nick** (`/lognick`, equipe)       | O nick informado pela equipe.                                                                                                              |

### Dados do servidor de Minecraft

O bot recebe do servidor de Minecraft, por uma conexão interna, **registros de eventos** (por exemplo, logs de punições e de atividades) e os publica em canais restritos à equipe, para moderação. Também consulta o **saldo de moedas** e o **ranking** de um jogador no banco da economia, e o **status** do servidor (jogadores online e versão).

### O que o bot **não** trata

* Não grava áudio nem vídeo.
* Não lê mensagens diretas entre outros usuários.
* Não coleta senhas, dados de cartão ou dados bancários. Pagamentos acontecem fora do bot, na loja oficial.
* Não coleta a lista de membros do servidor nem a monitora.
* Não usa seus dados para publicidade nem faz perfilamento comercial.

## Para que usamos os dados

* **Prestar os serviços** que você pede: abrir e fechar tickets, registrar denúncias, apelações e sugestões, sortear prêmios, dar cargos e ranking.
* **Moderação e segurança** do servidor: aplicar as [regras](/broken/pages/bbb1cfa1b1c5b006506b1353fa3f84eb7320f6e8), registrar mensagens apagadas ou editadas, investigar denúncias e prevenir abuso.
* **Atendimento**: responder dúvidas (inclusive com IA) e encaminhar o seu caso à equipe.
* **Melhorar o bot**: corrigir erros e ajustar o funcionamento. Não usamos seus dados para treinar modelos de IA.

## Base legal (LGPD)

Tratamos dados com base na **Lei Geral de Proteção de Dados (Lei nº 13.709/2018)**, conforme a função:

* **execução do serviço que você solicitou** (tickets, sorteios, sugestões, ranking);
* **legítimo interesse** da comunidade em manter o servidor seguro e moderado (logs de moderação, denúncias, prevenção a fraude);
* **cumprimento de obrigação legal ou regulatória**, quando houver exigência.

## Assistente de IA

O bot tem um assistente de IA, que responde pelo comando `/ia` ou quando alguém **menciona** o bot (ou responde a uma resposta dele).

### Como funciona

* Ele responde dúvidas sobre o servidor com base na **wiki pública**: busca os trechos mais relevantes e monta a resposta, com **links para as fontes**.
* Algumas respostas consultam **informações em tempo real**: status do servidor, agenda de eventos, cupons ativos da loja, ranking de moedas e de doadores e o saldo de moedas **de um nick que você mesmo informa**. Todas essas consultas são **somente leitura**.
* Em respostas sobre regras e punições, o bot avisa que a palavra final é da equipe.
* Quando o **atendimento com IA em tickets** estiver ativo, ele conversa com você para coletar o que a equipe precisa saber (categoria, nick, plataforma, local do ocorrido) e **encaminha o caso para um atendente humano**. A IA **não** pune, não decide e não executa ações de moderação.

### Provedor

A IA roda em um provedor externo, a **NVIDIA**. Ela só é usada para responder: **não treinamos nem ajustamos modelos de IA com os seus dados**.

### O que é enviado ao provedor de IA

Em cada pergunta, são enviados ao provedor de IA:

* o texto da sua pergunta, com as menções de usuários trocadas pelo nome;
* as **últimas mensagens da sua conversa** com o bot naquele canal (memória curta, veja abaixo);
* os **trechos da wiki** encontrados;
* o **resultado das consultas** feitas pelo bot (por exemplo, o saldo de moedas de um nick);
* no atendimento por tickets, as mensagens que você escrever no seu canal de atendimento.

{% hint style="warning" %}
**Não escreva senhas, dados de cartão, documentos ou outros dados pessoais sensíveis** em perguntas à IA ou na conversa de atendimento com a IA.
{% endhint %}

### Memória da conversa

A memória do assistente é **curta e temporária**: fica apenas na memória do bot (não em banco de dados), é separada por usuário e por canal e é **esquecida** depois de alguns minutos sem uso ou quando o bot reinicia.

### Registros

Para diagnóstico, o bot registra no log do servidor a pergunta feita à IA, com o seu nome e ID. Esses registros têm acesso restrito à equipe técnica e aparecem apenas no console do servidor: não são gravados em arquivo e são descartados quando o bot reinicia ou o console é limpo.

### Limites

A IA pode errar. As respostas são **geradas por IA** e vêm marcadas assim: **confira a fonte antes de agir**. Em caso de dúvida sobre regras ou punições, abra um ticket.

## Com quem compartilhamos

Os dados ficam acessíveis à **equipe da Rede Revo** conforme o cargo e a necessidade (por exemplo, apenas a equipe vê tickets, denúncias e logs de moderação). Para fazer o bot funcionar, usamos os prestadores abaixo.

### Serviços de terceiros

| Serviço                 | Para quê                                                                   | O que recebe                                                                                                                                 |
| ----------------------- | -------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------- |
| **Discord**             | Plataforma onde o bot funciona.                                            | Tudo o que você escreve e faz no Discord, conforme a [política de privacidade do Discord](https://discord.com/privacy).                      |
| **NVIDIA**              | Inferência do assistente de IA.                                            | O descrito em [O que é enviado ao provedor de IA](/broken/pages/983872f1e67f348457dffc9e869abbdd2cae3c1d#o-que-e-enviado-ao-provedor-de-ia). |
| **mclo.gs**             | Publicar logs de Minecraft anexados no Discord.                            | O conteúdo do arquivo de log que você anexar. O link gerado é público para quem o tiver.                                                     |
| **imgbb** e **TinyPic** | Converter imagens em link e hospedar imagens anexadas a tarefas da equipe. | A imagem enviada. O link gerado é público para quem o tiver.                                                                                 |
| **CentralCart**         | Loja oficial: cupons ativos e ranking de doadores.                         | Só consultas do bot. O ranking exibe **apenas o nick**, nunca o valor gasto.                                                                 |
| **mcsrvstat.us**        | Status do servidor de Minecraft.                                           | O endereço do servidor (nenhum dado seu).                                                                                                    |

Alguns desses serviços podem processar dados **fora do Brasil**. Ao usar essas funções, você concorda com essa transferência, que é feita apenas na medida necessária para o recurso funcionar.

{% hint style="warning" %}
**Não anexe logs ou imagens com informações pessoais** (senhas, tokens, IPs, documentos) nos canais que usam serviços externos: os links gerados são públicos.
{% endhint %}

Também podemos divulgar dados quando exigido por **lei, ordem judicial** ou para proteger a segurança da comunidade e de terceiros.

## Por quanto tempo guardamos

| Dado                                                     | Retenção                                                                                                                                                                                                                                                                                       |
| -------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Memória da conversa com a IA                             | Alguns minutos sem uso, ou até o bot reiniciar.                                                                                                                                                                                                                                                |
| Cache de mensagens (logs de apagadas/editadas)           | Em memória, até 10.000 mensagens, apagado ao reiniciar o bot.                                                                                                                                                                                                                                  |
| Dados de **tickets**                                     | No sistema de tickets atual, o registro é apagado ao fechar. No atendimento com IA, o registro (categoria, nick, plataforma, local, resumo e datas) é mantido, marcado como encerrado, por **até 1 ano**. Nos dois casos, a **transcrição** fica no canal de logs da equipe por **até 1 ano**. |
| Denúncias, apelações, sugestões, formulários e parcerias | Enquanto forem necessários para a análise e para o histórico de moderação, por **até 1 ano**.                                                                                                                                                                                                  |
| Ranking de XP                                            | Enquanto você estiver no servidor. Ao sair, o seu registro de ranking (ID, XP e horário da última mensagem) é apagado automaticamente.                                                                                                                                                         |
| Sorteios                                                 | Os participantes são apagados quando o sorteio termina.                                                                                                                                                                                                                                        |
| Logs técnicos do bot                                     | Aparecem apenas no console do servidor, sem gravação em arquivo. Descartados ao reiniciar o bot ou limpar o console.                                                                                                                                                                           |

Quando um dado deixa de ser necessário, ele é apagado ou anonimizado, salvo obrigação legal de guardar.

## Como protegemos os dados

* Acesso aos dados restrito à equipe, por função.
* Banco de dados em rede interna do servidor, com credenciais próprias e fora do código-fonte público.
* Canais de tickets, denúncias e logs visíveis só para a equipe.
* O bot pede ao Discord **só as permissões e os dados de que precisa** e não baixa a lista de membros do servidor.
* Quando o bot gera uma senha temporária no processo de recuperação de conta, ela é guardada apenas **criptografada (hash)**.

Nenhum sistema é 100% seguro. Se houver um incidente que possa afetar os seus dados, vamos avisar os envolvidos e a **ANPD**, nos termos da lei.

## Seus direitos

Pela LGPD, você pode, a qualquer momento:

* **confirmar** que tratamos seus dados e **acessá-los**;
* **corrigir** dados incompletos ou desatualizados;
* pedir a **exclusão** ou a **anonimização** de dados desnecessários;
* pedir a **portabilidade** dos seus dados;
* **revogar** consentimentos e **se opor** a um tratamento;
* pedir informações sobre com quem compartilhamos seus dados.

Para exercer qualquer direito, abra um **ticket** no Discord ou use o contato acima. Poderemos pedir que você **confirme sua identidade** antes de atender. Alguns dados podem ser mantidos quando houver obrigação legal ou necessidade de preservar o histórico de moderação.

Você também pode parar de usar o bot a qualquer momento ou sair do servidor (o que apaga o seu registro de ranking). Dados em tickets, denúncias e logs só são apagados mediante pedido ou conforme os prazos acima.

## Crianças e adolescentes

O Discord exige idade mínima de **13 anos**. O bot não se destina a menores dessa idade e não coleta dados de propósito de quem não pode usar a plataforma. Se você é responsável por um menor e acredita que ele nos enviou dados, fale com a equipe para a exclusão.

## Mudanças nesta política

Podemos atualizar esta política para refletir mudanças no bot ou na lei. A data no topo mostra a última revisão. Mudanças relevantes serão **avisadas no Discord** da Rede Revo.

## Contato

Dúvidas, pedidos ou reclamações sobre privacidade: abra um **ticket** no Discord da Rede Revo ou fale com **contato.rederevo@gmail.com**. Você também pode recorrer à **Autoridade Nacional de Proteção de Dados (ANPD)**.
