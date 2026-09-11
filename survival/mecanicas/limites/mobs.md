---
icon: cow
cover: ../../../.gitbook/assets/Inserir_um_titulo_3.png
coverY: 0
---

# Mobs

## Introdução

Para ajudar a manter a estabilidade e desempenho do servidor, existem um limite para cada criatura(mob) que podem permanecer em um determinado raio de blocos.

Os limites de forma geral são definidos pelo seu tipo, mas pode conter variações.

<table><thead><tr><th width="219">Categoria</th><th>Limite</th><th data-type="content-ref">Lista</th></tr></thead><tbody><tr><td>Aldeões</td><td>8 a cada 30 blocos</td><td><a href="mobs.md#aldeao">#aldeao</a></td></tr><tr><td>Aquáticos</td><td>3 a cada 10 blocos</td><td><a href="mobs.md#aquaticos">#aquaticos</a></td></tr><tr><td>Pacíficos</td><td>4 a cada 10 blocos</td><td><a href="mobs.md#pacificos">#pacificos</a></td></tr><tr><td>Pacíficos 2</td><td>5 a cada 10 blocos</td><td><a href="mobs.md#pacificos-2">#pacificos-2</a></td></tr><tr><td>Hostis </td><td>8 a cada 10 blocos</td><td><a href="mobs.md#hostis">#hostis</a></td></tr><tr><td>Especiais</td><td>2 a cada 20 blocos</td><td><a href="mobs.md#especiais">#especiais</a></td></tr></tbody></table>

{% hint style="info" %}
Os Limites a todos os mobs, independentemente da forma como foram gerados, seja gerados naturalmente, por geradores(spawners), pelo McMMO ou pelo sistema do /pets.
{% endhint %}

Cada mob tem um limite máximo e uma distância de verificação, quando determinado limite é atingido, os mobs que excedem esse limite serão removidos pelo sistema de limite do servidor.

## Funcionamento

Os limites são aplicados individualmente para cada tipo de mob, e não pela categoria em que ele está listado.&#x20;

Todas as variações de um mesmo mob compartilham o mesmo limite, por exemplo, diferentes variantes de lobo são contabilizadas juntas, assim como, os aldeões de diferentes profissões continuam sendo considerados apenas como aldeões para a contagem do sistema de limites.

{% hint style="danger" %}
Caso um mob seja removido automaticamente pelo sistema por ultrapassar o limite permitido, não será possível recuperar ele, incluindo quaisquer características, equipamentos ou itens associados a ele, sendo a perda permanente.
{% endhint %}

## Lista de mobs por categoria

### Aldeão

Os mobs classificados como aldeões possuem limite de 8 a cada 30 blocos.

* Aldeão
* Aldeão Zumbi
* Vendedor Ambulante

### Aquáticos

Os mobs classificados como aquáticos possuem limite de 3 a cada 10 blocos.

* Bacalhau
* Baiacu
* Girino
* Golfinho
* Lobo
* Lula
* Lula-Brilhante
* Náutilo
* Náutilo-Zumbi
* Peixe Tropical
* Salmão

### Pacíficos

Os mobs classificados como pacíficos possuem limite de 4 a cada 10 blocos.

* Allay
* Axolote
* Burro
* Cabra
* Camelo
* Camelo-Múmia
* Cavalo
* Cavalo-Esqueleto
* Cavalo-Zumbi
* Farejador
* Gato
* Golem de Cobre
* Golem de Ferro
* Golem de Neve
* Jaguatirica
* Lavagante
* Lhama
* Lhama do Vendedor
* Morcego
* Mula
* Panda
* Papagaio
* Raposa
* Sapo
* Tartaruga
* Tatu
* Urso-Polar

{% hint style="warning" %}
### **ATENÇÃO**

Os limites também é aplicado aos burros e mulas que possuem itens armazenados em baús, caso o limite removam esses animais, os itens armazenados não poderão ser recuperados.&#x20;
{% endhint %}

{% hint style="info" %}
Os papagaios que estiverem no ombro do jogador não entram na contagem do limite.
{% endhint %}

### Pacíficos 2

Os mobs classificados como pacíficos 2 possuem limite de 5 a cada 10 blocos.(O número 2 só representa a exceção aplicada)

* Abelha
* Coelho
* Galinha
* Mooshroom
* Ovelha
* Porco
* Vaca

{% hint style="info" %}
As abelhas que estiverem dentro da colmeia não são removidas pelo sistema de limites.
{% endhint %}

### Hostis

Os mobs classificados como hostis possuem limite de 8 a cada 10 blocos.

* Afogado
* Aranha
* Aranha das Cavernas
* Blaze
* Bruxa
* Creeper
* Cubo de Magma
* Devastador
* Enderman
* Endermite
* Errante
* Espectro
* Esqueleto
* Esqueleto Wither
* Ghast
* Guardião
* Guardião-Mestre
* Hoglin
* Invocador
* Pantanoso
* Piglin
* Piglin Bárbaro
* Piglin-Zumbi
* Rangente
* Ressecado
* Saqueador
* Shulker
* Slime
* Traça
* Vex
* Vingador
* Vórtice
* Zoglin
* Zumbi
* Zumbi-Múmia

### Especiais

Os mobs classificados como especiais possuem limite de 2 a cada 20 blocos.

* Defensor
* Ghast Feliz
* Wither

### Outros

Alguns mobs não utilizam atualmente um dos limites apresentados acima.

* Dragão do Fim (Não aplicável)
* Cubo de Enxofre (Ainda não disponível no servidor)
