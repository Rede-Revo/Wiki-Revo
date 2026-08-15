---
icon: bolt
cover: ../../.gitbook/assets/Inserir_um_titulo_3.png
coverY: 0
---

# Redstone

## Introdução

O uso de redstone é permitido no servidor, podendo criar sistemas automáticos, entretanto, sistemas muito rápidos ou com grande quantidade de componentes de redstone funcionando de forma simultânea podem afetar o desempenho do servidor.

Para manter a estabilidade, os sistemas de redstone são monitorados e possuem limites de funcionamento. Sistemas comuns devem funcionar normalmente, mas sistemas grandes que geram uma quantidade excessiva de ativações poderão não funcionar como o esperado.

## Funcionamento

O servidor contabiliza quantas vezes os componentes de redstone são ativados durante um certo espaço de tempo, essa verificação acontece por bloco, por chunk e por região.&#x20;

Essas verificações funcionam simultaneamente, por isso, mesmo que nenhum componente ultrapasse o limite individual, o sistema de redstone ainda poderá não funcionar como o esperado, caso a soma das ativações da chunk ou da região seja muito elevada.

Quanto mais componentes de redstone estiverem funcionando de forma simultânea, maior deverá ser o intervalo entre as ativações. Na prática, sistemas maiores precisam funcionar mais devagar para que não ultrapassem nenhum limite.

## Limitação

Quando algum limite de ativação é ultrapassado, novas ativações são impedidas, de forma temporária ou de forma definitiva.

Nenhum componente de redstone é removido automaticamente, mas se o sistema continuar ultrapassando os limites de ativações, o servidor poderá bloquear o funcionamento do seu sistema, caso isso aconteça, basta desligar o sistema e iniciar novamente, corrigindo o tempo entre ativações.

## Recomendações

* Evite temporizadores de redstone extremamente rápidos.
* Quanto maior for o seu sistema, maior deverá ser o tempo entre ativações.
* Adicione uma forma de ligar e desligar o seu sistema de redstone.
* Evite deixar sistemas de redstone funcionando sem necessidade.
* Evite deixar muitos sistemas em uma área pequena.
* Teste bem o funcionamento do limitador de ativações de redstone antes de aumentar o seu sistema de redstone.
* Diminua o intervalo de ativações, caso o servidor esteja desligando o seu sistema de redstone.

{% hint style="warning" %}
Dividir o sistema de redstone entre diferentes chuncks não garante que ele deixará de ser limitado, pois o servidor analisa também as atividades em uma determinada região.
{% endhint %}

{% hint style="info" %}
Esse limitador de redstone só está ativo nos mundos Verde e Vermelho, nos outros segue apenas o limite de blocos, não de ativação.
{% endhint %}
