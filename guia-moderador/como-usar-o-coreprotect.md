# Como usar o CoreProtect

## 0 - Sumário

-> [#1 - Comandos principais](como-usar-o-coreprotect.md#id-1-comandos-principais)\
-> [#2 - Como utilizar os comandos](como-usar-o-coreprotect.md#id-2-como-utilizar-os-comandos)\
-> [#3 - Uso detalhado do /co l](como-usar-o-coreprotect.md#id-3-uso-detalhado-do-co-lookup)\
-> [#4 - Exemplos praticos com /co l](como-usar-o-coreprotect.md#id-4-exemplos-praticos-com-co-lookup)\
-> [#5 - Limitações e cuidados ao analisar logs](como-usar-o-coreprotect.md#id-5-limitacoes-e-cuidados-ao-analisar-logs)\
-> [#6 - Análise de comandos e mensagens](como-usar-o-coreprotect.md#id-6-analise-de-comandos-e-mensagens)\
-> [#7 - Passo a passo para começar](como-usar-o-coreprotect.md#id-7-passo-a-passo-para-comecar)

## 1 - Comandos principais:

/co near -> Realiza uma busca simplificada na região.\
/co i -> Habilita o modo de inspeção.\
/co l -> Permite realizar busca com filtros.

## 2 - Como utilizar os comandos:

Obs.: Os comandos devem ser executados por mundo, ou seja, não será possível ver logs do mundo Vermelho enquanto estiver no mundo Verde, por exemplo.\
/co near -> Ao usar o comando, ele realizará uma busca rápida pelas ações recentes em uma área próxima.\
/co i -> Ao usar o comando, ativa o modo de inspeção por clique, permitindo ver logs diretamente de um local específico.\
Quando ativado:

Clique esquerdo no bloco:\
-> Mostra logs de colocação e quebra.\
-> Exemplo: Quer saber quem colocou um bloco, clique com o botão esquerdo do mouse sobre ele para ver quem colocou e quem quebrou (se aplicável).

Clique direito no bloco:\
Exibe logs de interações e transações, dependendo do tipo de bloco:\
-> Baús, barris, shulkers, funis, fornalhas, etc.: mostra quem adicionou ou removeu itens.(Por algum motivo, no momento da criação desse arquivo, para ver as logs de adição e remoção do enderchest físico, precisa usar o lookup com action:item)\
-> Portas, alçapões, alavancas, botões, etc.: mostra quem interagiu (abriu, fechou, acionou).\
-> Placas: mostra todo o histórico de texto que já foi escrito nela.\
-> Bloco quebrado: se clicar no bloco abaixo de onde estava o bloco removido, mostrará as logs do bloco acima.

Tentativa de colocar um bloco:\
-> Se tentar colocar um bloco em um local com o modo de inspeção ativo, exibirá no chat as logs do bloco naquele local.(Se o modo de inspeção estiver ativo, o bloco não será colocado de forma efetiva)\
Lembrete importante: O modo de inspeção não desativa automaticamente. Para sair do modo, use novamente o comando: /co i.

/co l ->\
Esse comando é usado quando precisa de resultados específicos, permitindo muitas possibilidades de filtros.\
-> Argumentos do comando: /co l a:\<ação> u:\<usuário> t: r: b: item: i: e:.\
Obs.: Não é necessário usar todos ao mesmo tempo.

### 3 - Uso detalhado do /co lookup:

#### action:\<ação> ou a:\<ação> ->

**Ações possíveis:**\
**a:block** -> Use sempre que quiser ver apenas interações de bloco, ou seja, colocar e quebrar. Ao usar ação block, será exibido no chat apenas interação de blocos colocados ou removidos.\
**a:break** -> Use sempre que quiser ver apenas blocos quebrados pelo player, ou seja, será exibido apenas os blocos que o player quebrou. Ao usar a ação break, será exibido no chat todos os blocos quebrados pelo player. Obs.: Será exibido blocos quebrados, não necessariamente significa que o player pegou o bloco.\
**a:chat** -> Use sempre que precisar verificar o que foi digitado pelo player no chat sem uso do "/". Ao usar a ação chat, será exibido no chat, tudo que foi digitado pelo player sem o uso da "/" antes. Obs.: Vale ressaltar que será exibido tudo que foi digitado no chat sem o /, não necessariamente irá exibir mensagens enviadas pelo player, exemplo, se o player usa "/l Oi, bom dia!", com a ação chat não será exibido, pois ele usou um comando para enviar a mensagem, mas se o player escreve apenas "Oi, tudo bem", nesse caso será exibido nas ações de chat, pois o player não usou comando para enviar, independente se a mensagem foi para o global, local ou para um chat travado, se não usou comando, será exibido com a ação chat.\
**a:click** -> Use sempre que quiser ver logs de click, isso é bem amplo, qualquer interação que o player tenha clicado irá trazer com essa ação, seja clique em baú, barril, shulker, porta, alavanca, botão, alçapão, craft, fornalha, e por aí vai. Ao usar a ação click, será exibido no chat todas as interações de clique.\
**a:command** -> Use sempre que quiser ver logs de comando. Ao usar a ação command, será exibido no chat tudo que o player escreveu como comando, independente de ser um comando válido ou não, isso inclue comandos de chat também, como o /l ou /g. Obs.: Podem ser exibidos comandos derivados de menus ou de outros comandos, ou seja, nem sempre os comandos que serão exibidos com action:command, foram comandos digitados manualmente pelo player.\
**a:container** -> Use sempre que quiser ver apenas interações de armazém, ou seja, colocou e tirou itens de baus/barris/shulkers etc. Ao usar ação container, será exibido no chat apenas interações de colocar e remover itens de conteiners. Obs.: Adição em locais onde tem inventário, como fornalhas, bigornas, mesa de ferraria, também irão aparecer aqui, mesmo que o player tenha aberto de forma virtual.\
**a:drop** -> Use sempre que quiser ver apenas interações de drop ou lançamentos. Ao usar a ação drop, será exibido no chat logs de itens lançados ou dropados, como, por exemplo, atirar uma flecha, jogar um poção ou dropar um item mesmo.\
**a:inventory** -> Use sempre que quiser ver logs da perspectiva do inventário do player. Ao usar ação inventory, será exibido todas as ações que removem/adicionem itens ao inventário do player. Obs.: Não irá exibir adições/remoções no enderchest virtual /ec ou no /lixo.\
**a:item** -> Use sempre que quiser ver apenas interações com itens, ou seja, sempre que dropar ou pegar um item. Ao usar ação item, será exibido no chat apenas interações com itens.\
**a:kill** -> Use sempre que quiser ver logs de mortes em uma região. Ao usar a ação kill, será exibido tanto mortes de player como de mobs.\
**a:pickup** -> Use sempre que quiser ver logs de itens/blocos que o player pegou. Ao usar a ação pickup, será exibido no chat todos os itens que o player pegou. Obs.: Itens recolhidos de forma automática pelo /auto, serão exibidos aqui também.\
**a:place** -> Use sempre que quiser verificar blocos colocados, ou seja, semelhante ao block, mas só será exibido blocos colocados pelo player. Ao usar a ação place, será exibido no chat todos os blocos colocados.\
**a:remove** -> Use sempre que quiser ver apenas blocos quebrados pelo player, ou seja, será exibido apenas os blocos que o player quebrou. Ao usar a ação break, será exibido no chat todos os blocos quebrados pelo player. Obs.: Será exibido blocos quebrados, não necessariamente significa que o player pegou o bloco. (Mesma coisa do break)\
**a:session** -> Use sempre que precisar ver quando o player entrou ou saiu do servidor. Ao usar a ação session, será exibido no chat todas as logs de entrada e saída do player.\
**a:sign** -> Use sempre que quiser verificar logs de placas. Ao usar a ação sign será exibido no chat o histórico de mensagens de placas.\
Essas são todas as ações disponíveis para uso. Será explicado mais para frente com exemplos.\
Obs.: Podem ser usados sinais + e - antes de algumas ações, isso limita a um tipo específico de ação.

#### user:\<usuário> ou u:\<usuário> ->

Use esse filtro para buscar ações realizadas por jogadores específicos ou por múltiplos usuários ao mesmo tempo. Também é possível filtrar por entidades e causas especiais, como fogo ou explosões. Obs.: Para usuários que não sejam players, é necessário colocar o # antes do nome.\
Exemplo de alguns users que podem ser usados:\
u:#fire - Filtra por fogo.\
u:#tnt - Filtra por tnt.\
u:#lava - Filtra por lava.\
u:#water - Filtra por água.\
u:#piston - Filtra por pistão.\
u:#explosion - Filtra por explosão.\
u: - Filtra por nick.\
u:# - Filtra por mob.\
Esses são os principais.\
Obs.: Coloque como user, quem praticou a ação.

#### time:\<tempo> ou t:\<tempo> ->

Use esse filtro para limitar o intervalo de tempo da busca, ele aceita até cinco unidades de tempo diferentes (s-Segundo, m-Minuto, h-Hora, d-Dia, e w-Semana), podendo ser combinadas entre si. Ex.:\
t:5s - Irá realizar a busca nos últimos 5 segundos.\
t:5m - Irá realizar a busca nos últimos 5 minutos.\
t:5h - Irá realizar a busca nos últimos 5 horas.\
t:5d - Irá realizar a busca nos últimos 5 dias.\
t:5w - Irá realizar a busca nos últimos 5 semanas.\
Obs.: É possível combinar múltiplas unidades em um único valor. Ex.: t:10d2h irá buscar logs dos últimos 10 dias e 2 horas.

#### radius:\<raio> ou r:\<raio> ->

Use esse filtro para buscar em um raio específico, ele aceita de 0 a 100 blocos de distância, busca pelo mundo ou por dimensão. Ex.:\
r:10 - Fará uma busca em 10 blocos para cada lado.\
r:#world\_nether - Fará uma busca apenas no nether do mundo atual.\
r:#world - Fará uma busca apenas na dimensão normal do mundo atual.\
r:#Recursos - Fará uma busca apenas na dimensão recursos.\
r:#world\_the\_end - Fará uma busca apenas no end.\
r:#eventos - Fará uma busca na dimensão eventos.\
r:global - Fará uma busca no mundo todo.\
Obs.: Vale lembrar que nem todas as dimensões estão disponíveis em todos os mundos. Existem mais dimensões, mas é bem raro filtrar por dimensões.

block:\<bloco> ou b:\<bloco> ->

Use esse filtro para buscar ações de um bloco específico, ele aceita qualquer bloco. Obs.: Precisa passar o id/namespace do bloco. Ex.:\
b:diamond\_block - Irá buscar todas as interações com o bloco de diamante.\
b:dirt - Irá buscar todas as interações com terra.\
Obs.:\
O nome do item é exibido ao passar o mouse por cima do item, caso não mostre, use F3+H para habilitar. imagem de exemplo: https://prnt.sc/NbE-NuNkm-LW .\
Outra forma de encontrar o nome do item é na própria wiki do fandom do minecraft. url : https://minecraft.fandom.com/wiki/Java\_Edition\_data\_values/Pre-flattening/Block\_IDs .\
Normalmente, o nome do item é ele mesmo em inglês, substituindo os espaços por \_.\
Não é necessário colocar minecraft: antes do nome do bloco.\
É possível buscar itens usando o block.\
É possível buscar por mais de um bloco, separando com ','. Ex.: b:dirt,glass\_block nesse caso irá buscar tanto interações com terra, quanto com grama.

item:\<item>, i:\<item> ou include:\<item> ->

Use esse filtro para realizar busca de um item específico. Segue a mesma lógica do block, precisa do id do item ou namespace para realizar a busca. (Pode ser usado para consultar blocos)\
exclude:\<item|bloco|user> ou e:\<item|bloco|user> ->\
Use esse filtro para ignorar um bloco, item ou um usuário. Ex.:\
e:netherite\_axe - Ignorará todas as interações que tenham machado de netherite.\
e: - Ignorará todas as interações desse nick.\
e: - Ignorará todas as interações desse mob.\
e: - Ignorará o item específico.\
e: - Ignorará o bloco específico.\
Obs.: Lembrando que o bloco e item, precisam estar no formato de id/namespace.\
Esses são os principais filtros que podem ser usados no /co lookup \<filtros>.

\
Use /co lookup \<página>|, para configurar a quantidade de linhas que serão exibidas para você na busca atual. Ex.:\
/co l 1:5 - Serão exibidos 5 linhas da busca atual na página 1.\
/co l 2:10 - Serão exibidos 10 linhas da busca atual na página 2.\
Obs.: Padrão é 4 linhas por página. Esse comando afeta o /co near, /co i e o /co lookup.

### 4 - Exemplos praticos com /co lookup

Demostração de uso dos filtros do /co l:\
Comando: /co lookup radius:global time:5d user:Steve\
Irá buscar por todas as ações realizadas por Steve, em todo o mundo, nos últimos 5 dias.\
\
Comando: /co lookup radius:10 action:container time:1h\
-> Mostra interações com containers (baús, funis, fornalhas etc.) nos últimos 60 minutos, num raio de 10 blocos à sua volta.\
\
Comando: /co lookup radius:global action:session user:Steve\
-> Retorna registros de login e logout do Steve em todo o mundo.\
\
Comando: /co lookup radius:global action:block time:7d user:Alex,Steve\
-> Busca todas as quebras ou colocações de blocos feitas por Alex e Steve nos últimos 7 dias, em todo o mundo.\
\
Comando: /co lookup radius:5 time:10m action:place\
-> Mostra blocos colocados nos últimos 10 minutos, em um raio de 5 blocos da sua posição.\
\
Comando: /co lookup time:1d user:#creeper r:#world\
-> Mostra alterações no mapa causadas por Creepers nas últimas 24 horas, em toda a dimensão normal.\
\
Comando: /co lookup radius:world\_nether action:block user:Steve time:3h\
-> Verifica ações com blocos feitas por Steve nas últimas 3 horas, especificamente no Nether.\
\
Comando: /co lookup time:2d user:Notch,Herobrine action:container\
-> Exibe interações com containers feitas por Notch ou Herobrine nos últimos 2 dias, na área onde o comando for executado.\
\
Comando: /co lookup action:command time:30m radius:8\
-> Mostra todos os comandos enviados nos últimos 30 minutos, na área de 8 blocos em sua volta. (Recomendo usar exclude:, para ocultar a exibição de comandos executados por você, pois quando você usa o comando do core, também é registrado)\
\
Comando: /co lookup action:chat time:5d4h3m user:Steve,Alex radius:global\
-> Mostra todas as mensagens enviadas no chat nos últimos 5 dias, 4 horas e 3 minutos, em todo o mundo.\
\
Comando: /co lookup radius:global user:#tnt action:block time:10h\
-> Busca ações com blocos destruídos por dinamite nas últimas 10 horas, em todo o mundo.\
\
Comando: /co lookup radius:global user:Steve time:1d item:netherite\_pickaxe\
-> Busca todas as interações que Steve teve com picaretas de netherite no último dia.\
\
Comando: /co lookup radius:50 time:10h item:carved\_pumpkin action:pickup\
-> Busca todas as vezes que a Abóbora esculpida (No servidor, é usado esse item em alguns itens personalizados) foi pega do chão (Se for removida de moldura, também aparecerá aqui) no raio de 50 blocos nas últimas 10 horas.\
Esses são alguns exemplos de comandos.\
\
Exemplo de resultado:

```
    CoreProtect - Procurando. Por favor, aguarde...
    ----- CoreProtect |  Mostrando Resultados -----
    12.54/h atrás   + Steve   pegou x1 netherite_axe  .
                            ^ (x110/y143/z-45/world)     (a:item)
    17.76/h atrás   - Steve   largou x1 iron_block  .
                            ^ (x110/y143/z-44/world)     (a:item)
    21.76/h atrás   + Steve   colocou spawner  .
                            ^ (x178/y112/z-4/world)     (a:block)
    1.12/d atrás    - Steve   removeu x1 spawner  .
                            ^ (x178/y112/z-5/world)     (a:container)
    Pág   1/41 ▶   (1 | 2 | 3 | 4 | 5 | 6 ... 41)
```

Caso o item seja personalizado, seja pelo servidor ou pelo player, ao passar o mouse por cima do nome do item/bloco, irá aparecer o nome personalizado.\
A data e hora exata podem ser obtidas ao passar o mouse por cima da quantidade de tempo já passado.\
Após as coordenadas, aparecerá a dimensão na frente, no caso dessas logs, todas ocorreram no #world.\
Na frente das coordenadas aparecem as ações a:\<ação>.\
Na parte inferior, é possível alterar entre as páginas clicando na ▶ ou no número da página, sem a necessidade de escrever o comando /co page .

### 5 - Limitações e cuidados ao analisar logs:

O sistema não registra corretamente todos os eventos de transição ou lógica de jogo, ele apenas registra ações isoladas como quebras, colocações, mortes ou interações, por isso, em alguns casos, a ação registrada não representa exatamente com o que aconteceu.\
Ex.:\
Se um bloco é empurrado por um pistão, o core irá registrar que o bloco foi quebrado em uma posição e colocado em outra, como se fosse uma ação manual.\
Se um aldeão for transformado em um aldeão-zumbi, aparecerá apenas que o aldeão foi morto, sem qualquer indicação da conversão.\
O mesmo ocorre com areia ou cascalho que caem, registrado como quebra e nova colocação.\
As ações de venda e compra no /pshop podem não ser registradas de forma correta no core, sendo necessária uma investigação mais profunda.\
O mesmo pode ocorrer com as captações por funis, não sendo registradas no sistema.\
Por isso, alguns casos exigem uma abordagem mais cautelosa e cuidadosa, para assim evitar passar/interpretar informações de forma equivocada.\
Vamos ver alguns exemplos disso e como agir:\
\
**Exemplo 1**: Aldeão sumiu:\
Reporte do player: O player diz que um aldeão sumiu de uma determinada localização.\
Ação: Vá até o local informado e use o comando: /co lookup action:kill radius:20 time:1d\
-> Ajuste o radius conforme o tamanho da área onde o aldeão podia andar.\
-> Ajuste o time conforme a data/hora aproximada que o player informar.\
Resultado 1: Se encontrou log de morte, faça:\
-> Se o aldeão foi morto por player, informe ao jogador que o aldeão foi morto por um player que tem ou teve permissão no terreno. (/terreno confiarlista) (Evite informar o nick diretamente, exceto em alguns casos)\
-> Se o aldeão foi morto por um zumbi, verifique se há algum aldeão-zumbi por perto, se não houver, provavelmente o aldeão, não tinha nametag, em casos onde a chunk não esteja carregada, ele irá sumir.\
Resultado 2: Se não encontrou log de morte, faça:\
-> Vá até o canal de logs do /limite do discord, lá registra todos os mobs removidos pelo sistema, se encontrar coordenadas próximas, informe ao player que o sistema de /limite foi ultrapassado. (Se possível, oriente e ajude o player a organizar os aldeões para que isso não se repita)\
Resultado 3: Se não encontrou nada nas logs de morte e não encontrou nada no discord, faça:\
-> Vá para fora da estrutura onde o aldeão estava, do lado de fora, verifique se há para-raio no local, se não tiver, o aldeão provavelmente virou bruxa, mas se tiver, use /co i e clique com o botão esquerdo no para-raio e verifique se o para-raio foi colocado após a morte do aldeão.\
Obs.: Mortes por raio normalmente não aparecem no core.\
\
**Exemplo 2**: Itens sumiram do baú/barril/shulker.\
Reporte do player: player informa que uma picareta natalina desapareceu de num baú em sua base.\
Ação: Vá até o local onde o item estava e ative o modo de inspeção com /co i. Clique com o botão direito no baú e veja as logs de interações, buscando quem possa ter removido ou ao menos o nick do dono do item.\
Resultado 1: Encontrado log de remoção do item por outro player:\
-> Informe ao player que o item foi retirado por alguém que tem ou teve permissão no terreno (/terreno confiarlista).\
Obs.: Normalmente, não informamos o nick do player que removeu, exceto em casos específicos.\
Resultado 2: Encontrado log de inserção do item, mas nenhum de remoção, e o item está no baú.\
-> Informe ao player que o item continua no baú. Às vezes, foi apenas um bug visual.\
Resultado 3: Encontrado log de inserção, mas o item não está no baú e nenhuma remoção aparece.\
-> Use /co lookup radius:global time:1d user: item:netherite\_pickaxe para ver se o player teve interação com o item após adicionar ele no baú.\
-> Se não retornar nada, use /co lookup radius:100 time:1d item:netherite\_pickaxe próximo do local para ver se outro player pegou.\
-> Se ainda assim não houver log de remoção, pode ser que tenha removido para algum tipo de funil:\
-> Verifique se há funil conectado ao baú ou próximo a ele.\
-> Abra o inventário dos funis e baus próximos, talvez o item tenha ido para outro lugar via funil, não é comum, mas é possível, use também o comando /co lookup action:place radius:100 block:hopper, e verificando onde foi colocado os funis.(Não é comum, mas talvez seja interessante verificar)\
Resultado 4: Se não encontrar nada nos passos anteriores, talvez tenha usado placa de venda.\
-> Se nenhum log de remoção for encontrado, use: /co lookup action:command radius:5 time:1d e procure por comandos como quickshop-create, quickshop-buy, /pshop create, etc, também use: /co lookup action:chat radius:5 time:1d para verificar mensagens como "1", "all", "10000", que podem indicar interações com o qs.\
-> Se encontrar, verifique com /co lookup radius:global time:1d user: item:netherite\_pickaxe para confirmar que o item foi transferido. (se aparecer comandos como quickshop-create, /pshop create, esses comandos são realizados pelo criador da placa, já a mensagem "1" e "all", são realizados pelo comprador).\
-> Se não encontrar interações no mundo atual do item com o possível comprador, verifique a log do inv com /invsave history e veja se houve troca de mundo ou logout com o item, confirme também se o item foi para o ender chest.\
Resultado 5: Falha de servidor ou desconexão no momento da inserção.\
-> Se o item foi adicionado, mas não aparece mais e nenhum log de remoção ou movimentação existe, verifique: /co lookup action:-session radius:global time:1d user:\
-> Se o player caiu logo após inserir o item, e outros players também desconectaram, pode ser bug de salvamento durante instabilidade, neste caso, considere a possibilidade de devolução do item, conforme análise do contexto.(importante verificar todas as logs antes de solicitar/realizar a devolução).\
Obs.: Use outros métodos para encontrar o item, o normal é o item ter ido para em algum lugar, não sumir de repente, verifique nas logs de comando se tem uso dos comandos, /trocar, /lixo, /ah sell, entre outros, caso tenha, verifique suas respectivas logs, como /tradelog, /ah perfil, /pshop history, entre outros, sobre a log do /lixo, é um pouco mais complicado, mas se suspeita que o mesmo possa ter jogado no /lixo, pergunte-o se ele não jogou o item no /lixo, pela resposta dará para ter uma ideia.\
Obs.: Caso o bau, barril, shulker, não esteja mais no local, vá para a posição com o /tp e digite na posição exata, /co lookup radius:0 time:, o core irá te mostrar todas as transações, para saber qual shulker é, só ir acompanhando as logs, vai aparecer que colocou, abriu, quebrou, pegou, se a shulker tiver nome personalizado, irá aparecer apenas quando quebrar.

### 6 - Análise de comandos e mensagens:

A action:command retorna todos os comandos executados por um player, como /tpa, /tell, /warp, entre outros, esse recurso pode ser usado para investigar o comportamento de um player, permitindo identificar padrões estranhos, como a repetição excessiva de certos comandos ou de uma mesma sequência, essa prática, por exemplo, é usada por alguns players para tentar burlar o sistema anti-AFK, já que ao trocar de mundo, zera o tempo afk. Casos como esse devem ser alertados ao jogador, e em situações reincidentes, podem resultar em punição na Regra 13.\
Essa action também ajuda a entender o que aconteceu em casos mais delicados, como denúncias, onde é preciso reconstituir com precisão a sequência de ações, por exemplo, em um caso de tpakill, onde comandos/mensagens trocadas antes do /tpaccept ou /tpa podem confirmar a intenção do player.\
Além disso, o action:command é útil para confirmar se certas ações realmente foram executa, por exemplo, se um jogador afirma ter criado uma home, mas ela não aparece, pode ter ocorrido uma falha no servidor (como uma queda), e usando o core você poderá confirmar se o comando foi de fato executado ou se o player removeu a home manualmente, se ao ser solicitado o .ajuda, de fato foi escrito .ajuda sem nenhum comando antes.\
Outro uso importante é na ajuda de localizar itens, usando os comandos executados pelo player, é possível descobrir se o jogador colocou um item no /ah(log de adição de item no /mercado, tem no discord), fez trocas com outros players ou teleportou para alguma /go, vale lembrar que o core não registra transações feitas por placas de loja, então saber para qual /pwarp o jogador foi, pode ajudar a verificar se ele vendeu algo por lá. Em relação a trocas, já aconteceram casos onde o comando /tradelog estava limpo, mesmo o player tendo executado trocas, nesses casos, vale a pena verificar nos logs do core se o player enviou uma solicitação de troca para alguém, e então analisar as logs do outro player para encontrar possíveis pistas de onde o item está. Quanto ao /ah, mesmo havendo logs no /ah perfil, essas informações podem ser apagadas com o tempo.\
Em situações mais difíceis, especialmente com itens raros, é possível procurar pelas movimentações deles no canal de logs do discord após a data da adição, ou utilizar o core para rastrear o item pelo mundo, mas vale lembrar que isso é mais eficaz com itens únicos ou personalizados, para itens comuns, o número de interações será alto, o que dificultará encontrar o item, já que nada impede de terem 2 itens comuns com o mesmo nick. Já que estamos falando sobre encontrar itens, as mensagens enviadas pelo player, podem ajudar a entender se ele estava vendendo o item ou algo assim.\
A action:chat apenas complementa isso, podendo ser usada para validar, por exemplo, a confirmação de algo, como reivindicar um terreno, ou colocar um valor em um item para vender, além de auxiliar em denúncias e em investigações.

## 7 - Passo a passo para começar:

Primeiro passo - Vá até o local do ocorrido.\
-> Antes de qualquer comando, vá até onde o problema aconteceu (ex: onde o bloco foi quebrado, o item sumiu, ou o mob desapareceu).\
-> Isso garante que os comandos serão executados no local correto, e ajuda a você entender o contexto da situação.\
Segundo passo - Use o modo de inspeção.\
-> Use, /co i\
Com ele ativado:\
-> Clique com o botão esquerdo em um bloco - mostra quem colocou ou quebrou.\
-> Clique com o botão direito em containers (baús, shulkers etc.) - mostra quem colocou ou removeu itens.\
Para sair do modo de inspeção, use /co i novamente.\
Terceiro passo - Use comandos mais específicos.\
-> Se precisar de uma busca mais detalhada, use: /co lookup (Como explicado no tópico #3).\
Quarto passo -> Anote ações importantes.\
-> Aconselho a ir anotando tudo que for encontrando, como última interação, hora, data e o local, pois isso ajuda a manter a organização.\
-> Veja com atenção o horário, o nick de quem fez a ação e o tipo de interação (ex: quebrou, colocou, removeu, etc.).\
Lembrete final:\
-> O core mostra apenas o que foi registrado, em alguns casos (como placas de loja, funis, mortes), ele pode não mostrar tudo ou mostrar incorretamente, então é super importante cruzar informações com outros sistemas de log, como o discord, /tradelog, /ah perfil, /pshop history, /money log, /cash log, entre outros, pois isso garante um grau maior de confiabilidade.
