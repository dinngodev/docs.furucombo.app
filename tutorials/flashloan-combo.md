---
description: 'Tutoriel: Créer un Combo Flashloan sur Furucombo'
---

# Combo "Prêt Flash"

![](https://gblobscdn.gitbook.com/assets%2F-MMtyf0qXl8g_wxjxrFt%2F-MMuCpQ6BdX8NBN4KXTh%2F-MMuCyZo9s1FsfE501i5%2Fimage.png?alt=media&token=e86376e0-d1ca-4226-96ca-9f92c6738557)

## **Qu'est-ce qu'un Flashloan?** <a id="256b"></a>

Les prêts flash sont proposés par Aave, un protocole de prêt open source permettant à quiconque de déposer et d'emprunter des actifs cryptographiques. Les prêts flash permettent aux utilisateurs d'emprunter n'importe quel montant jusqu'à concurrence de la liquidité totale disponible sans aucune garantie, à condition que le prêt soit remboursé dans la même transaction. Si le prêt n'est pas remboursé, l'ensemble de la transaction sera annulé. Avec flashloan, n'importe qui peut accéder à une quantité massive de liquidités et utiliser le prêt avec d'autres protocoles comme il le souhaite. Vous pouvez devenir une «baleine» sans capital.

Au moment de la rédaction de cet article, il existe trois protocols offrant des prêts flash :

* **Aave:** 22 tokens disponibles avec des frais de 0.09% du capital emprunté
* **dYdX:** 3 tokens disponibles sans frais\*
* **Uniswap V2:** 100+ tokens disponibles avec des frais de 0.3%

```text
*Notez que flashloan sur dydx n'est pas une fonctionnalité grand public.Il est réalisé par les développeurs enchaînant les actions de retrait, d'appel et de dépôt.
```

Donc, flashloan semble être une très bonne affaire. Pour quoi exactement pouvez-vous l'utiliser? [Marc Zeller](https://twitter.com/lemiscate) d'Aave a écrit un très [bel article](https://medium.com/aave/sneak-peek-at-flash-loans-f2b28a394d62) démontrant quelques-uns des principaux cas d'utilisation du flashloan.

Résumons les cas d'utilisation :

* Transactions d'arbitrage
* ​[Swap de garantie](https://deflast.finance/) \(swap = échange\)
* Auto-couverture
* Auto-liquidation
* \(Dette\) Swap de taux d'intérêt
* \(Dette\) Swap de devises

Le cas d'utilisation le plus populaire est de loin celui des _**transactions d'arbitrage**_. Pour ceux qui ne sont pas familiers, l'arbitrage est la stratégie consistant à tirer profit des différences de prix entre les différents marchés. Pour réaliser un profit significatif, vous aurez besoin d'un capital substantiel pour démarrer. Et c'est là que la magie opère - Nous utilisons flashloan pour générer de l'argent gratuit sans coût initial.

## **Avant de commencer** <a id="avant-de-commencer"></a>

Il y a des choses importantes à comprendre :

> Pour les traders d'arbitrage, Furucombo abaisse les barrières à l'entrée pour la construction de legos d'argent, en fournissant tous les éléments nécessaires pour créer des stratégies d'arbitrage, y compris les prêts flash uniquement pour les codeurs. Mais gardez à l'esprit que Furucombo ne trouve **PAS** d'opportunités d'arbitrage pour vous. Vous devrez le trouver vous-même. ✊🏻

Passons cette clause d'utilisation et vérifions les données. 👇🏻

```text
Trouvez une opportunité d'arbitrage >0,09% pour couvrir les frais de prêt flash Ayez suffisamment d'ETH dans votre portefeuille pour payer les frais de transaction (gas fee).
```

L'exemple que nous utilisons ci-dessous est une opportunité d'arbitrage trouvée entre KyberSwap et Uniswap V1, il y a quelques mois.

```text
Différence de taux : + de 20% 1 DAI = 1,2411 sUSD sur Uniswap1 sUSD = 0,9927 DAI sur Kyberswap👉🏻 Achetez bas vendez haut : achetez sUSD sur Uniswap et vendez-le sur Kyberswap
```

Maintenant que vous avez trouvé la différence de taux, commençons à créer le combo. Le combo complet devrait ressembler à ceci :

```text
Emprunter 100 DAI en FlashloanSwap 100 DAI à 122.83649 sUSD sur UniswapSwap 122.83649 sUSD à 122.83429 DAI sur KyberswapRembourser 100.09 DAI à FlashloanVous conservez un bénéfice de 22.74429 DAI.
```

## Pas à pas <a id="29f4"></a>

### 2. Ajoutez un cube Uniswap V1 <a id="126f"></a>

![](https://gblobscdn.gitbook.com/assets%2F-MMtyf0qXl8g_wxjxrFt%2F-MMtymN5VcPSi8VM1Gny%2F-MMu9UQpr2Zad4R2l0GN%2Funi%20v1.png?alt=media&token=1596c153-82fe-4ed1-b787-5be4eaa1023e)

Cube Uniswap v1 "Swap token"

```text
1️⃣ Cliquez sur le cube avec le symbole '+' 2️⃣ Choisissez 'Swap Token' dans la section Uniswap V1 3️⃣ Entrez l'entrée : 100 DAI4️⃣ Sortie générée à partir d'Uniswap : 122.83649 sUSD5️⃣ Cliquez sur 'Set'
```

### 3. Ajoutez un cube Kyberswap <a id="dcdb"></a>

![](https://gblobscdn.gitbook.com/assets%2F-MMtyf0qXl8g_wxjxrFt%2F-MMtymN5VcPSi8VM1Gny%2F-MMu9vH5c6mfTPZUnwuE%2Fkyber.png?alt=media&token=bed21568-c95d-4093-aedf-a7745d2c8b7d)

Cube Kyberswap "Swap token"

```text
1️⃣ Cliquez sur le cube avec le symbole '+' 2️⃣ Choisissez 'Swap Token' dans la section Kyberswap 3️⃣ Entrez l'entrée : 122.83649 sUSD4️⃣ Sortie générée à partir de Kyberswap : 122.83429 DAI5️⃣ Cliquez sur 'Set'
```

💡 **Astuces** : Si votre entrée est conforme à la sortie du cube précédent, entrez un montant légèrement inférieur au lieu du montant exact. De cette façon, vous pouvez éviter l'échec du combo en raison de la différence de taux.

### 4. Ajoutez un cube Flashloan <a id="de6a"></a>

![](https://gblobscdn.gitbook.com/assets%2F-MMtyf0qXl8g_wxjxrFt%2F-MMtymN5VcPSi8VM1Gny%2F-MMuAVjg2mRBwRlXZzor%2Fflashloan.png?alt=media&token=75e74131-d441-4bdd-b830-66ad8b7906a4)

Cube Aave "Flashloan"

```text
1️⃣ Cliquez sur le cube avec le symbole '+' 2️⃣ Choisissez 'flashloan' dans la section Aave 3️⃣ Entrez le montant: 100 DAI4️⃣ Cliquez sur 'Set'5️⃣ Deux cubes apparaissent. Le 1er cube est un emprunt de 100 DAI et le 2è cube est un remboursement de 100,09 DAI.
```

### 5. Faites glisser le premier cube de flashloan vers le haut <a id="81e4"></a>

Il s'agit simplement d'ajuster l'ordre d'exécution. Vous souhaitez emprunter un flashloan au tout début pour avoir le capital initial. Donc, il suffit de cliquer et de faire glisser le cube d'emprunt vers le haut et de conserver le cube de remboursement en bas.

Le combo final ressemblerait à ça...

![](https://gblobscdn.gitbook.com/assets%2F-MMtyf0qXl8g_wxjxrFt%2F-MMtymN5VcPSi8VM1Gny%2F-MMuArpAvGYcjqpySW3s%2Farb.png?alt=media&token=533ff85e-e24a-48af-8e02-c741896c6396)

Combo pour une transaction d'arbitrage

### 6. Connectez votre wallet \(portefeuille\) <a id="72ba"></a>

### 7. Cliquez sur "Send" \(Envoyer\) <a id="a283"></a>

🎉 Bravo! Vous avez gagné de l’argent sans capital.

_N'oubliez pas de partager votre résultat sur Twitter_.🎉

![](https://gblobscdn.gitbook.com/assets%2F-MMtyf0qXl8g_wxjxrFt%2F-MMuCpQ6BdX8NBN4KXTh%2F-MMuD6DszSbhVjpIdKLQ%2F0_Kfym6hUWLOi4tXxA.gif?alt=media&token=eac27213-4ca4-4a2a-8c3b-86f91ad3ff7a)



🧊 Special thanks to Juxx for translating this page.

