# Page Combo

## ● Cubes Uniswap V2  <a id="uniswap-v2-cubes"></a>

### Je ne trouve pas le token/pool que je veux. <a id="je-ne-trouve-pas-le-token-pool-que-je-veux"></a>

Il existe une fonction d'importation de token sur les cubes Uniswap V2. Il suffit de coller l'adresse du token ou l’adresse de la pool du token dans la barre de recherche.

![](https://gblobscdn.gitbook.com/assets%2Ffurucombo-flashloan%2F-MNdGHzfaSwPoiGiwSSx%2F-MNdH20BKH2LNBLpu4dm%2Fimage.png?alt=media)

### Puis-je échanger directement des WETH ? <a id="puis-je-echanger-directement-des-weth"></a>

Malheureusement, l'utilisation de WETH comme entrée/sortie dans les cubes Uniswap V2 n'est pas disponible sur Furucombo. Vous pouvez, cependant, utiliser le cube WETH sous l'utilitaire pour wrap vos ETH en WETH ou l’inverse\(unwrap\).

### Quel est le slippage mis en place sur Uniswap ? <a id="quel-est-le-slippage-mis-en-place-sur-uniswap"></a>

Le slippage par défaut est fixé à 3 %.

## ● Cubes Aave  <a id="aave-cubes"></a>

### Comment utiliser le flashloan ? <a id="how-to-use-flashloan"></a>

Nous disposons d'un tutoriel complet pour vous guider dans la création d'un combo flashloan. Lire [ici](https://juxx.gitbook.io/furucombo-flashloan/)​

### Pourquoi j’ai une erreur "something's wrong inside the flashloan cubes" ? <a id="why-does-it-say-somethings-wrong-inside-the-flashloan-cubes"></a>

Lorsque vous appuyez sur le bouton d'envoi, Furucombo effectue une estimation de votre combo dans l'ordre de la configuration de vos cubes. Lorsque vous voyez le message d'erreur "something's wrong inside the flashloan", cela signifie que la transaction échouera lors de l'exécution de la paire de cubes « flashloan ».

L'erreur la plus courante est que le prix a changé dans la paire de cubes flashloan. Dans ce cas, appuyez sur le bouton "Actualiser le prix".

Vous pouvez également essayer de supprimer les cubes du flash loans et appuyer à nouveau sur "Envoyer" pour voir quel cube est en erreur.

### Pourquoi dois-je payer 0,09% de frais ? <a id="why-do-i-have-to-pay-0-09-fee"></a>

Les frais de 0,09% sont payés directement à Aave pour l'utilisation du flashloan. Furucombo ne facture aucune redevance sous quelque forme que ce soit.

### Pourquoi ne puis-je pas mettre les cubes Aave dans le flashloan ? <a id="why-cant-i-put-aave-cubes-inside-flashloan"></a>

Il s'agit d'une limitation mise en place par Aave. Lorsque vous utilisez le flashloan, vous prenez les liquidités d'Aave. Cela n'a pas de sens d'utiliser les fonds empruntés sur la pool d’ou proviennent ces derniers, n’est-ce pas ?

## ● CubesMaker  <a id="maker-cubes"></a>

### Qu'est-ce qu'un Vault ? <a id="what-is-a-vault"></a>

Le _Vault_ \(coffre-fort\) est un élément essentiel du protocole Maker, qui facilite la génération de DAI contre des garanties verrouillées. Tous les DAI en circulation sont créés par des Vaults. L'utilisation des Vaults modifie collectivement l'offre totale de DAI.

Les utilisateurs créent des DAI en les générant contre leur garantie et, à leur tour, détruisent les DAI lorsqu'ils remboursent le solde de leurs DAI générés.

L'utilisation des Vaults n'est pas gratuite et comporte des risques inhérents. La génération de DAI nécessite le paiement de frais de stabilité \(SF\). Les SF sont à taux variable et peuvent être modifiées en fonction des décisions prises par vote par les détenteurs de jetons MKR.

Pour récupérer les garanties, les utilisateurs doivent rembourser les DAI précédemment généré et les SF accumulées. Les Vault doivent être « sous garanties » et avoir un ratio de liquidation que les propriétaires de Vault doivent respecter pour éviter leur liquidation.

Lorsqu'un Vault est liquidé, une pénalité de liquidation est appliquée et la garantie est vendue pour rembourser le solde DAI du Vault. En outre, un plafond de dette est imposé globalement au protocole Maker, ainsi qu'individuellement à chaque type de Vault

### Où puis-je obtenir mon numéro de Vault ? <a id="where-do-i-get-my-vault-number"></a>

Si vous avez déjà un Vault, connectez d'abord votre portefeuille et choisissez ensuite n'importe quel Maker cube \(sauf « New Vault »\). Vous verrez votre numéro de Vault s'afficher lorsque vous cliquerez sur la parti vide \(là où est censé s’écrire votre numéro de Vault\).

Si vous utilisez « New Vault» pour créer une chambre forte. Vous obtiendrez son numéro une fois que le combo aura été effectué avec succès. Ensuite, vous pourrez revenir sur la page de création de combo et choisir n'importe quel cube Maker, sauf "New Vault", pour voir votre numéro de Vault.

![](https://gblobscdn.gitbook.com/assets%2Ffurucombo-flashloan%2F-MNdGHzfaSwPoiGiwSSx%2F-MNdHQPpetrDxnG49m7d%2Fimage%281%29.png?alt=media)

Vous pouvez également consulter le site [oasis.app](https://oasis.app/) pour connaître le numéro de votre Vault.

### Qu'est-ce qu'Oasis Trade ? <a id="what-is-oasis-trade"></a>

Oasis Trade a été créé par par Maker. Il s'agit d'un pool de liquidités sur la blockchain Ethereum. Les _Smart Contracts_ "Simple Market" et "Matching Market" permettent l'échange immédiat de jetons ERC20 sans tiers de confiance.

Pour en savoir plus cliquez ici \([https://oasis.app/support](https://oasis.app/support)\)

### Comment tirer profit du passage du CDP\* Maker vers Compound ? <a id="how-to-profit-from-moving-cdp-to-compound"></a>

Il s'agit d'un combo pour les utilisateurs qui ont déjà un coffre-fort \(_Vault_\) sur Maker pour les aider à déplacer facilement leurs jetons vers Compound. Ce n'est pas nécessairement un combo rentable. Il s'agit plutôt d'un combo de gestion d'actifs placés sur Maker…

```text
* CDP = Collateralized Debt Position (Position de Dette Garantie)
```

## ● Cubes Curve  <a id="curve-cubes"></a>

### Puis-je choisir le pool pour mon échange ? <a id="can-i-choose-the-pool-to-swap"></a>

Vous ne pouvez pas choisir la pool sur Curve. Lorsque vous utilisez le cube de token d'échange de Curve, Curve choisit automatiquement la meilleure pool pour vous.

### Quel est le slippage mis en place sur Curve ? <a id="what-is-the-slippage-set-up-on-curve"></a>

Le slippage par défaut est fixé à 3 %.

### Le combo de réclamation CRV ne fonctionne pas... <a id="le-combo-de-reclamation-crv-ne-fonctionne-pas"></a>

Lorsque vous utilisez Claim CRV, le token réclamé va directement dans votre portefeuille. Donc, si vous voulez utiliser les jetons CRV dans les cubes suivants, vous devez insérer un cube "Add Funds" comme cube suivant avec CRV comme entrée.

## ● Cubes 1inch  <a id="1inch-cube"></a>

### Je ne trouve pas le token que je veux, mais je peux le trouver sur 1inch <a id="i-cant-find-the-token-i-want-but-i-can-find-it-on-1inch"></a>

Les tokens sur Furucombo sont sélectionnés par l'équipe de Furucombo. Si vous ne trouvez pas le token que vous voulez, veuillez le faire savoir à l'équipe sur le canal Discord \#feedback.

### Quel est le slippage mis en place sur 1inch ? <a id="what-is-the-slippage-set-up-on-1inch-cube"></a>

Le slippage par défaut est fixé à 3%.

### J'utilise 1inch dans mon combo mais il continue à dire qu'il va échouer <a id="i-use-1inch-in-my-combo-but-it-keeps-saying-it-will-fail"></a>

Il y a un problème connu d'incohérence pour l'utilisation de 1inch :

* Allez sur 1inch.exchange pour voir quel service d'échange ils utilisent sur le trajet pour votre paire d'échange. Supposons que vous voyez qu'il passe par Uniswap V2
* Revenir à Furucombo et remplacer le cube de 1inch par Uniswap V2.

## ● Cubes Compound  <a id="compound-cubes"></a>

### Comment puis-je emprunter auprès de Compound ? <a id="how-do-i-borrow-from-compound"></a>

Malheureusement, la fonction d'emprunt de Compound n'est pas prise en charge sur Furucombo. Mais il s'agit d'un travail en cours.

### Comment puis-je m'auto-liquider sur Compound ? <a id="how-can-i-self-liquidate-on-compound"></a>

Nous avons un [combo pré-construit](https://furucombo.app/combo/bt49ulfm1503gp5r5keg?refreshPrice=1) pour vous, que vous pouvez également trouver sur notre [Page Explore](https://furucombo.app/explore/combo_compound_00004) lors de votre prochaine visite.

![](https://gblobscdn.gitbook.com/assets%2Ffurucombo-flashloan%2F-MNdGHzfaSwPoiGiwSSx%2F-MNdHQPnqcC_DDBXdFQG%2Fcompound%20self-liq.png?alt=media)

Utilisez le tag _Compound_ pour trouver plus facilement le combo

## ● Cube Kyberswap  <a id="kyberswap-cube"></a>

### Je ne trouve pas le token que je veux, mais je peux le trouver sur Kyberswap <a id="i-cant-find-the-token-i-want-but-i-can-find-it-on-kyberswap"></a>

Les tokens sur Furucombo sont sélectionnés par l'équipe de Furucombo. Si vous ne trouvez pas le jeton que vous voulez, veuillez le faire savoir à l'équipe sur le canal Discord \#feedback.

### Quelle est le taux de slippage sur Kyberswap ? <a id="whats-the-slippage-setup-on-kyberswap"></a>

Le slippage par défaut est fixé à 3%.

## ● Cubes Balancer  <a id="balancer-cubes"></a>

### Je ne trouve pas le token/pool que je veux… <a id="i-cant-find-the-token-pool-i-want-1"></a>

Les tokens sur Furucombo sont sélectionnés par l'équipe de Furucombo. Si vous ne trouvez pas le jeton que vous voulez, veuillez le faire savoir à l'équipe sur le canal Discord \#feedback.

### Comment puis-je faire une contre-examination avec Balancer ? <a id="how-do-i-cross-examine-the-pool-with-balancer"></a>

1️⃣ Vérifiez les six premiers chiffres de l'adresse du pool.

![](https://gblobscdn.gitbook.com/assets%2Ffurucombo-flashloan%2F-MNdGHzfaSwPoiGiwSSx%2F-MNdHQPqsDi7pxoZC_RE%2Fimage%282%29.png?alt=media)

2️⃣ Vérifiez le poids des actifs dans le pool

![](https://gblobscdn.gitbook.com/assets%2Ffurucombo-flashloan%2F-MNdGHzfaSwPoiGiwSSx%2F-MNdHQPr3XGCYtKOvO82%2Fimage%283%29.png?alt=media)

### Qu'est-ce que les options "_Single-Asset_" \(actif unique\) et "_All-Assets_" \(tous les actifs\) ? <a id="what-is-single-asset-and-all-assets-options"></a>

Lorsque vous ajoutez ou retirez des liquidités à Balancer, vous verrez les options "Tous les actifs" et "Actif unique" en haut de la page. Prenons l'exemple du pool WETH 50%/WBTC 50% :

![](https://gblobscdn.gitbook.com/assets%2Ffurucombo-flashloan%2F-MNdGHzfaSwPoiGiwSSx%2F-MNdHQPs5sR0k1_w5f7z%2Fimage%284%29.png?alt=media)

* Ajouter de la liquidité - **Tous les actifs** : Vous fournissez tous les actifs du pool proportionnellement aux poids du pool.
  * ​👉 Vous envoyez 1 WETH et 0,0285 WBTC à Balancer et vous recevez un token de 0,02283 BPT.
* Ajouter de la liquidité - **Actif unique** : Vous ne fournissez qu'un seul type de token au pool. Balancer échangera le token que vous avez fourni proportionnellement pour ajouter de la liquidité dans le pool.
  * ​👉 Vous envoyez 1 WETH à Balancer et vous recevez un jeton de 0,01105 BPT.

## ● Cubes Utility  <a id="utility-cubes"></a>

### Qu'est-ce que "Send Token" ? <a id="what-is-send-token"></a>

Comme il est dit, le cube Send Token vous permet d'envoyer un token à l'adresse que vous avez indiquée. Certains cas d'utilisation peuvent être :

* Envoyer un jeton à plusieurs adresses
* Envoyer plusieurs jetons à une même adresse
* Déplacez tous vos jetons de poussière dans un autre portefeuille

### Qu'est-ce que WETH ? <a id="what-is-weth"></a>

Lorsque vous "enveloppez" de l’ETH, vous n'enveloppez pas vraiment mais vous échangez via un smart contract contre un jeton égal appelé WETH. Si vous voulez récupérer ETH, vous devez le "déballer". C'est-à-dire l'échanger contre de l'ETH ordinaire.

Pour en savoir plus sur WETH, visitez le site [weth.io](https://weth.io/)​

### Qu'est-ce que l'ajout de fonds ? <a id="what-is-add-funds"></a>

Le cube _Add Funds_ est utilisé lorsque vous devez envoyer de l'ETH ou des tokens à Furucombo **pendant l'exécution** d'un combo.

Par exemple, lorsque vous voulez réclamer vos CRV et les vendre contre des DAI, vous devez utiliser "Add Funds" pour compléter le combo. En effet, lorsque vous réclamez votre CRV, les jetons réclamés vont directement dans votre portefeuille mais pas dans celui de Furucombo. Afin de continuer à envoyer ces CRV à Uniswap, vous devez d'abord envoyer les CRV à Furucombo. Voir la configuration correcte ci-dessous.

![](https://gblobscdn.gitbook.com/assets%2Ffurucombo-flashloan%2F-MNdGHzfaSwPoiGiwSSx%2F-MNdHQPtBq6_73M83Nna%2Fimage%285%29.png?alt=media)

### Qu'est-ce que les fonds en retour ? <a id="what-is-return-funds"></a>

Le cube _Return Funds_ est utilisé lorsque vous souhaitez renvoyer des ETH ou des tokens à votre portefeuille **pendant l'exécution** du combo. Bien que Furucombo renvoie tous les fonds aux utilisateurs à la fin de l'exécution du combo, dans certains cas, des fonds de retour doivent être ajoutés pour exécuter le combo avec succès.

Par exemple \(voir l'image ci-dessous\), vous voulez échanger vos garanties sur Compound, disons cDAI -&gt; cETH. Lorsque vous empruntez de l’ETH via un flashloan et que vous fournissez l’ETH à Compound, le cETH que vous voyez dans le deuxième cube est en fait envoyé au mandataire de Furucombo. Vos cDAI sont bloqués jusqu'à ce que vous ayez assez de cETH pour couvrir votre dette, donc ici nous avons besoin du cube "_Return Funds_" qui transfère les cETH du mandataire de Furucombo vers votre portefeuille. Et dans le cube suivant, vous déplacez votre cDAI vers le proxy Furucombo par le cube "_Add Funds_" !

![](https://gblobscdn.gitbook.com/assets%2Ffurucombo-flashloan%2F-MNdGHzfaSwPoiGiwSSx%2F-MNdHQPuDKewVBrjGGQD%2Fimage%286%29.png?alt=media)

### Qu'est-ce que l'économiseur de gas ? <a id="what-is-gas-saver"></a>

Le cube Gas Saver est utilisé lorsque vous avez des jetons CHI ou GST2 dans votre portefeuille. Lorsque vous les brûlez \(surtout si le prix de l'essence est élevé\), vous obtenez un remboursement pour rendre l'essence beaucoup moins chère comparé à la même transaction qui n'utilise pas de GasToken.

Pour en savoir plus sur les jetons de gaz, consultez les liens ci-dessous :

* * 
## 🧠 Stratégies d'arbitrage <a id="arbitrage-strategies"></a>

### Qu'est-ce que l'arbitrage ? <a id="what-is-arbitrage"></a>

À bien des égards, l'arbitrage crypto est comme l'arbitrage fiat ou sportif. L'idée principale est simple : vous essayez de profiter des différences de prix pour un même actif sur différents marchés ou bourses. Investopedia décrit l'arbitrage comme "l'achat et la vente simultanés d'un actif pour profiter d'un déséquilibre dans le prix. Il s'agit d'un commerce qui profite de l'exploitation des différences de prix d'instruments financiers identiques ou similaires sur différents marchés ou sous différentes formes".

En d'autres termes, **achetez à bas prix et vendez à haut prix** !

Lectures connexes :

* L'arbitrage dans le DeFi par le bloc

### À quoi ressemble un combo rentable ? <a id="what-does-a-profitable-combo-look-like"></a>

![](https://gblobscdn.gitbook.com/assets%2Ffurucombo-flashloan%2F-MNdGHzfaSwPoiGiwSSx%2F-MNdHQPy59XLvDfkKK5P%2Fprofitable.png?alt=media)

* Il **n'y a pas** de fonds initiaux

Si vous voyez apparaître la section des fonds initiaux, cela signifie que ce n'est pas une combinaison rentable. Dans le pire des cas, vous perdez les fonds initiaux et ne recevez rien en retour.

* Vous recevrez
  * Les actifs indiqués dans cette section sont les bénéfices de la combinaison.

### Comment faire un combo rentable ? <a id="how-to-make-a-profitable-combo"></a>

* Avant tout, vous devez trouver une opportunité d'arbitrage.
* En tenant compte du coût du gas, les combos d'arbitrage coûtent plus cher que les combos moyens en raison de la complexité des actions. C'est un facteur de coût essentiel qui influence la rentabilité de l’échange.
* N'oubliez pas qu'il y a toujours de nombreux bots qui essayeront de "_front-run_" \(devancer\) vos transactions. Il est donc possible que votre combo soit en tête de liste des bots.
* Les combos d'arbitrage ont plus de chances d'échouer car la configuration du combo dépend généralement beaucoup des sorties de chaque cube. Cela étant dit, une fois l'occasion passée, votre combo échoue et vous perdez les frais de gaz que vous venez de payer.

## 👛 Portefeuille <a id="wallet"></a>

Si vous ne voyez pas Coinbase Wallet, cliquez sur Wallet Connect et scannez le code QR avec votre application Coinbase Wallet.

Suivez [ce tutoriel](https://www.loom.com/share/bee83b1e0d724779aa4d22c9d8a242c0) pour permettre à Furucombo de connecter votre MetaMask à Brave.

La raison en est que Brave vient de mettre à jour ses paramètres sur la façon de connecter "Web3 provider for using Dapps".

Nous continuerons à enquêter sur cette question et nous nous assurerons qu'elle est à jour.

### Je ne peux pas me connecter à la plateforme <a id="i-can-not-connect-to-the-platform"></a>

* Assurez-vous de sélectionner le bon réseau \(Ethereum Mainnet\), normalement sur le fournisseur de portefeuille vous pouvez changer le réseau sur les options de réglages.
* Sur Ledger ou sur Metamask :
  * Assurez-vous de déverrouiller et de sélectionner l'application Ethereum.
  * Assurez-vous que les données du contrat sont autorisées dans les paramètres de l'application Ethereum.
* Coinbase :
  * Utilisez le code QR de balayage pour vous connecter.
* Wallet connect
  * Utilisez le code QR de balayage pour vous connecter
* Fortmatic
  * Assurez-vous de passer sur Ethereum Mainnet.

## ⛽️ Gas <a id="gas"></a>

### Pourquoi le prix du gas est-il si élevé ? <a id="why-is-the-gas-fee-so-high"></a>

Cela dépend du nombre de cubes que vous utilisez et de la congestion du réseau Ethereum. Vous pouvez cliquer sur le bouton "Envoyer" pour estimer le coût du gaz. Votre portefeuille \(par exemple, MetaMask\) apparaîtra et vous indiquera le montant que vous devez dépenser pour couvrir les frais de gas.

### Puis-je savoir combien de gaz va me couter ma transaction avant de l’envoyer ? <a id="can-i-know-how-much-gas-before-send"></a>

Malheureusement, vous ne pouvez pas obtenir l'estimation du prix de l'essence avant d'appuyer sur le bouton "Envoyer".

### Comment puis-je connaître le prix du gaz ? <a id="how-can-i-set-up-the-gas-price"></a>

Vous pouvez ajuster le prix du gaz et la limite de gaz en utilisant le portefeuille MetaMask. En appuyant sur le bouton d'envoi, vous verrez apparaître une fenêtre contextuelle MetaMask. Cliquez sur "EDIT", puis vous verrez des choix de vitesse.

Pour personnaliser les frais de transaction, sélectionnez "Options avancées" :

Vous pouvez saisir manuellement le prix de l'essence \(GWEI\) et la limite de l'essence. Vous pouvez également cliquer sur le graphique des prédictions de gaz en direct.

![](https://gblobscdn.gitbook.com/assets%2Ffurucombo-flashloan%2F-MNdGHzfaSwPoiGiwSSx%2F-MNdHQPvC-7Q2JqHFt10%2Fimage%287%29.png?alt=media)

### Dois-je réduire la limite de gaz ? <a id="should-i-reduce-gas-limit"></a>

Non, vous ne devriez pas. La limite de gaz est le budget de la transaction. Le gaz non utilisé sera remboursé à votre porte-monnaie. Cependant, si le gaz coûte plus cher que votre limite de gaz, tout sera remboursé mais le gaz ne sera PAS restitué.

## 📖 Autres FAQs <a id="other-faqs"></a>

### Comment ajuster les fonds initiaux ? <a id="how-do-i-adjust-initial-funds"></a>

Le montant des fonds initiaux est mis à jour automatiquement. Il vous suffit d'ajuster les chiffres dans les cubes, puis le montant requis de fonds initiaux sera mis à jour en conséquence.

### Pourquoi dois-je signer deux fois ? <a id="why-do-i-need-to-sign-two-times"></a>

Normalement, vous devez envoyer deux transactions pour traiter un transfert de token non ETH.

Par exemple, si vous souhaitez échanger des DAI contre des COMP, vous devez signer deux fois sur votre portefeuille :

1. Approuver : pour autoriser Furucombo à déplacer vos jetons.
2. Envoyer : pour exécuter votre transaction. Dans cet exemple, pour échanger votre DAI contre un COMP.

### Combien de fois dois-je approuver ? <a id="how-many-times-do-i-have-to-approve"></a>

Cela dépend des tokens que vous avez et des cubes que vous allez utiliser. Dans certains cas, il est possible que vous n'ayez pas besoin d'approuver. Le nombre de fois où vous devez donner votre accord dépend du nombre de conditions ci-dessous qui sont remplies.

* Première utilisation d'un jeton ERC20 comme fonds initial
* Première utilisation d'un des cubes ci-dessous
  * _**Maker**_ _withdraw_
  * _**Maker**_ _Generate_
  * _**Curve**_ _Stake_
  * _**Curve**_ _Claim_

Exemples:

* Le premier combo d'Alice : Echange ETH contre DAI
  * Pas besoin d'approbation
* Premier combo de Bob : Echange DAI contre ETH, Echangez AAVE contre ETH
  * Doit être approuvé deux fois. \(Une fois pour DAI, une fois pour AAVE\)
* Le 2ème combo de Bob : Echange AAVE contre DAI
  * Pas besoin d'approbation
* Le 3ème combo de Bob : Déposer WBTC pour créer et générer du DAI
  * Doit être approuvé deux fois \(une fois pour WBTC, une fois pour Maker Generate\)

### Pourquoi il est écrit que ma transaction va échouer ? <a id="why-does-it-keep-saying-my-transaction-will-fail"></a>

Dans la plupart des cas, c'est parce que le prix a changé et que vous devez mettre à jour les chiffres.

Si vous utilisez des cubes de prêt flash et que vous voyez le message d'erreur, cela signifie que vous devez mettre à jour les numéros des cubes dans la paire du flashloan.

### Pourquoi ma transaction a-t-elle échoué ? <a id="why-did-my-transaction-fail"></a>

Dans la plupart des cas, c'est parce que le prix a changé, ce qui a rendu votre combinaison trop éloignée de votre configuration original. Vous pouvez éviter ce genre de problème en laissant plus de place au slippage :

Par exemple, vous voulez échanger 1 ETH contre DAI, puis ajouter DAI au pool de courbes en tant que fournisseur de liquidités \(LP\) :

Bonne combinaison :

* Cube 1: échangez 1 ETH contre 400 DAI
* Cube 2: ajouter 380 DAI au pool Curve

Mauvais combo:

* Cube 1: échange 1 ETH contre 400 DAI
* Cube 2: ajouter 400 DAI au pool Curve

Lorsque vous saisissez 400DAI dans le Cube 2, votre transaction échouera dès que le résultat de l'échange dans le Cube 1 vous donnera moins de 400DAI, ce qui n'est pas rare.

Laisser une différence dans la saisie du 2e cube peut augmenter considérablement les chances de succès. Dans l'exemple du "bon combo", la transaction n'échouera que si le prix de l'ETH descend en dessous de 380 $ \(&gt; 5 %\) entre le moment où vous définissez le combo et l'envoi.

### Pourquoi ne puis-je pas envoyer, même si je sais que cela va échouer ? <a id="why-cant-i-send-even-i-know-it-will-fail"></a>

C'est un mécanisme qui vous permet d'éviter de perdre inutilement de l'argent.

### Comment puis-je annuler ma transaction en cours ? <a id="how-do-i-cancel-my-pending-transaction"></a>

Vous pouvez utiliser le bouton "annuler" dans l'application si vous utilisez MetaMask ou Trust. Pour les autres portefeuilles, vous pouvez consulter leurs sites web officiels pour plus de détails. Vous pouvez également envoyer une autre transaction avec le même portefeuille et **le même nonce** \(numéro de transaction\) avec un prix de l'essence plus élevé.

### Ma transaction est bloquée dans l'attente d'une confirmation. <a id="my-transaction-is-stuck-pending-confirmation"></a>

Dans cette situation, veillez à ne pas continuer à envoyer des transactions. Chaque nouvelle transaction sera bloquée en attendant que la plus ancienne soit confirmée. Vous pouvez vous débarrasser de la transaction bloquée en l'accélérant ou en l'annulant, selon que le portefeuille que vous utilisez possède ou non cette option.

Par exemple, les portefeuilles _Metamask_ ou _Trust Wallet_ offrent tous deux la possibilité d'annuler ou d'accélérer les transactions.

Par ailleurs, si votre fournisseur de portefeuille ne dispose pas d'une option d'accélération ou d'annulation, vous pouvez toujours annuler la transaction bloquée en envoyant une transaction 0 ETH à votre adresse \(à vous-même\) en utilisant le même numéro d'identification \(nonce\).

Vous pouvez inspecter le nonce de votre transaction sur [Etherscan](https://etherscan.io/) et utiliser des services comme [MEW](https://www.myetherwallet.com/) ou [MyCrypto](https://mycrypto.com/) pour envoyer cette transaction avec un coût d'essence plus élevé et remplacer celle qui est bloquée.

### Je ne peux pas appuyer sur le bouton d'envoi <a id="i-can-not-press-the-send-button"></a>

Essayez de déconnecter puis reconnecter votre portefeuille.

### Je ne sais pas quoi construire, y a-t-il un exemple de combo ? <a id="i-dont-know-what-to-build-is-there-any-example-combo"></a>

Visitez [la page _Explore_](https://furucombo.app/explore) pour vous inspirer.

### Comment sauvegarder mon combo ? <a id="how-do-i-save-my-combo"></a>

Lorsque vous créez un combo, cliquez sur l'icône en forme de chaîne située sous le bouton d'envoi. Vous obtiendrez un lien vers le combo en cours.

![](https://gblobscdn.gitbook.com/assets%2Ffurucombo-flashloan%2F-MNdGHzfaSwPoiGiwSSx%2F-MNdHQPwM2H180VGU7gi%2Fimage%288%29.png?alt=media)

Lorsque vous créez un combo, il y aura un lien "partager" en bas, cliquez sur l'icône de la chaîne pour obtenir le lien ou cliquez sur l'icône Twitter pour le partager sur Twitter.

![](https://gblobscdn.gitbook.com/assets%2Ffurucombo-flashloan%2F-MNdGHzfaSwPoiGiwSSx%2F-MNdHQPxZgu7vBtliBpK%2Fimage%289%29.png?alt=media)

### Je rafraîchis le prix et il est toujours indiqué que le combo échouera. <a id="i-refresh-price-and-it-still-says-it-will-fail"></a>

Dans la plupart des cas, c'est parce que le prix a encore changé et que vous devez mettre à jour les chiffres.

De plus, si vous utilisez un cube 1inch et que vous voyez ce message d'erreur plusieurs fois, essayez d'utiliser un autre cube d'échange pour obtenir un prix plus stable.

### Le site ne charge pas. <a id="the-site-does-not-load"></a>

Les étapes suivantes peuvent résoudre vos problèmes :

* Si vous utilisez le navigateur Brave, passez à un autre navigateur pour éliminer les problèmes du navigateur. Si le problème est lié au navigateur Brave, voici quelques mesures à prendre qui peuvent vous aider :

  * Effacer les données du cache et les cookies du site
  * Rafraîchissement forcé avec contrôle + F5 \(ou cmd + r\)
  * Désactiver le portefeuille Brave
  * Ou tout autres extensions qui pourraient interférer avec votre portefeuille

  ​

Si, après avoir essayé toutes les étapes ci-dessus, elle continue d'échouer. Malheureusement, nous vous suggérons d'accéder à Furucombo en utilisant un autre navigateur car ces incompatibilités proviennent du navigateur Brave.

* Assurez-vous que votre connexion Internet fonctionne et est stable
* Redémarrez le navigateur et essayez de vous connecter à nouveau
* Essayez de rafraîchir le site avec contrôle + F5
* Vérifiez s'il existe une mise à jour pour votre navigateur ou le fournisseur de portefeuille utilisé, si c'est le cas, mettez-le à jour avec la dernière version.



🧊 Special thanks to Manu for translating this page and Juxx for editing. 

