# Guide du débutant

![](../.gitbook/assets/image%20%2817%29.png)

Bienvenue à Furucombo. Dans ce guide, nous allons passer en revue toutes les bases que vous devez connaître pour réussir à créer un combo. Avant de commencer, parlons de «qu'est-ce que Furucombo?».

Furucombo est un outil conçu pour que les utilisateurs finaux optimisent leur stratégie DeFi simplement par glisser-déposer. Tout comme créer vos propres legos DeFi, mais vous n'avez pas besoin de savoir coder. Il visualise les protocoles DeFi complexes en cubes. Les utilisateurs doivent juste entrer les entrées / sorties et configurer les commandes des cubes \(nous appelons cela un «combo»\), puis Furucombo regroupera tous les cubes en une seule transaction et les enverra. C'est un excellent outil pour les personnes qui souhaitent effectuer des actions sur différents protocoles, en particulier celles qui souhaitent tirer parti du prêt flash. \(Nous couvrons flashloan dans l'article ici .\)

Maintenant que vous avez l'idée de ce qu'est Furucombo, commençons!

## Guide de l'interface Furucombo

### ・Menu DeFi <a id="e7c5"></a>

![](../.gitbook/assets/image%20%2829%29.png)

Pour commencer à créer un combo, vous devez d'abord sélectionner un protocole DeFi. Cliquez sur le cube «＋», puis un menu de protocoles DeFi apparaîtra. Ici, vous pouvez choisir le protocole DeFi que vous souhaitez mettre dans votre combo. Chaque bouton représente un cube à configurer. Chaque cube signifie une action à exécuter. La fonction de recherche en haut vous permet de rechercher par nom par defi, par action par defi \(par exemple swap, ajouter de la liquidité, etc.\) ou par nom du jeton pris en charge sous certains defi.

### ・Fonds initiaux <a id="1bcf"></a>

![](../.gitbook/assets/image%20%2830%29.png)

Lorsque vous commencez à configurer des cubes, vous pouvez voir une section en haut à gauche intitulée «Fonds initiaux». Cela signifie les fonds que vous devez fournir au début du combo pour lancer la transaction.

Les fonds initiaux sont envoyés directement depuis **votre portefeuille**. Cela dit, vous devez avoir un solde suffisant du ou des jetons dans votre portefeuille, sinon la transaction **ne sera PAS** exécutée. Lorsque votre portefeuille est connecté, le solde du portefeuille de chaque jeton sera affiché ici afin que vous puissiez toujours vérifier avant d'envoyer le combo.

### ・Vous allez recevoir <a id="5cd0"></a>

![](../.gitbook/assets/image%20%281%29.png)



Sur la gauche, vous voyez une section « **Vous recevrez** ». Ce sont les fonds à retourner dans votre portefeuille à la fin de la transaction. C'est le résultat de toutes les entrées et sorties que vous avez construites sur la droite, qui sont mises à jour chaque fois que vous modifiez un cube.

```text
👩🏻‍🏫 Pense juste que 
Les «fonds initiaux» correspondent au montant que vous mettez et, 
«Vous recevrez» est ce que vous obtenez à la fin.
```

## Pas à pas

### Étape 1: Configuration des cubes ⚙️ <a id="0903"></a>

![](../.gitbook/assets/image%20%2831%29.png)

Lorsque vous sélectionnez un protocole, vous êtes amené à saisir les détails du cube. Ici, vous verrez fréquemment les termes «entrée» et «sortie».

```text
L'entrée signifie combien de jeton vous dépenserez pour exécuter cette action.
La sortie signifie la quantité de jeton que vous recevrez lors de l'exécution de cette action.
```

La source d'entrée peut être des jetons que vous avez dans votre portefeuille ou des sorties de cubes précédents. Une fois que vous avez configuré le cube, vous pouvez toujours le modifier / le supprimer en cliquant sur l'icône stylo / poubelle en haut à droite de chaque ensemble.

### Étape 2: Faites glisser et déposez 🖱 ✋🏻 📦 <a id="5853"></a>

![](../.gitbook/assets/1_ioy6idmu4smf-3gcuoebmw.gif)

Tous les cubes que vous configurez peuvent être déplacés. Faites- les simplement **glisser** dans l'ordre que vous souhaitez. Lorsque le combo est envoyé, les actions sont exécutées selon l'ordre des cubes.

> Exemple: lorsque vous créez flashloan, vous verrez une paire de deux cubes apparaître. \(Le premier cube signifie «emprunter» et le deuxième cube signifie «récupération».\) La prochaine chose que vous devez faire est d'ajouter plus de cubes \(actions que vous voulez faire avec les jetons empruntés\) et de les faire glisser entre la paire de prêt flash.

### Étape 3: connectez votre portefeuille 👛 <a id="f5ac"></a>

![](../.gitbook/assets/1_oqusodpu0ues59xxpalg0q.gif)

Vous pouvez créer un combo sans vous connecter à votre portefeuille. Mais si vous souhaitez envoyer le combo, vous devez connecter votre portefeuille. Cliquez simplement sur le cube avec une icône de portefeuille. Ensuite, choisissez votre portefeuille à connecter.

### Étape 4: Envoi d'un combo 🔗 🎉 🎁 <a id="bafb"></a>

![](../.gitbook/assets/1_n7ovqm9e2xx-z8vawws52a.gif)

Le flux complet d'envoi d'un combo serait:

1️⃣ Cliquez sur « **Approuver** » lorsque vos fonds initiaux sont des jetons ERC20. Vous ne devez le faire qu'une fois par jeton.

2️⃣ Cliquez sur « **Envoyer** », puis Furucombo exécutera une estimation de votre combo. Si la transaction échoue, un message apparaîtra comme un rappel afin que vous puissiez modifier votre combo. Inversement, vous verrez une fenêtre contextuelle de demande sur votre portefeuille pour signer la transaction.

3️⃣ Une fois votre combo envoyé avec succès, le bouton se transforme en « **Nouveau Combo** » et un message avec le lien de transaction apparaît. Quand vous voyez ces changements, félicitations!

Vous avez terminé un combo! N'oubliez pas de partager votre résultat sur Twitter en cliquant simplement sur l'icône Twitter.

Nous avons également réalisé un didacticiel vidéo de ce guide. Vérifiez-le 👇🏻

{% embed url="https://www.youtube.com/watch?v=wCfMm2a91qs" %}



🧊 Special thanks to Kib for translating this page.

