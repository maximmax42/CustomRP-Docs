---
description: Question posées fréquement
---

# ❓ FAQ

{% hint style="warning" %}
Cette page peut être obsolète. Veuillez consulter la [version anglaise de cette page](https://app.gitbook.com/s/5gJfBQC2iWNK0J953fo2/faq) pour obtenir les informations les plus récentes.
{% endhint %}

## Questions

### Puis-je ajouter plus de 2 boutons ?

Non, c'est une limite instaurée par Discord.

### Puis-je utiliser un autre type d'activité (Ex: écoute, regarde, diffuse) ?

Non, c'est aussi une limite instaurée par Discord.

### Pourquoi si je définis un horodatage quelques jours dans le futur, Discord n'affiche que le nombre d'heures restantes ?

Vous l'avez deviné, c'est encore une limite instaurée par Dicord.

### Y aura-t-il une version Linux/Mac ?

L'application est construite à l'aide d'une bibliothèque Windows uniquement. Par conséquent, la prise en charge de Linux et Mac signifierait la réécriture de l'application entière dans une bibliothèque/langage de codage différent. Ce que je ne prévois pas encore.

### Une fenêtre appelée "Pipe" s'est ouverte pour une raison quelconque, qu'est-ce que c'est ?

Il s'est ouvert car vous avez appuyé sur Ctrl + Maj et cliqué sur le bouton Connecter (ou sur le bouton Ctrl et Connecter ou Reconnecter dans le menu de l'icône de la barre d'état sur les anciennes versions). Laissez-le à -1 et fermez-le. Il est utilisé dans les situations où plusieurs clients Discord s'exécutent en même temps. Changer le numéro de canal choisit efficacement le client dans lequel vous souhaitez que votre présence soit.

## Dépannage

Avant d'essayer quoi que ce soit, assurez-vous d'être sur la dernière version de CustomRP !

### Quand je clique sur les boutons de présence dans mon profil, ils ne fonctionnent pas.

Les boutons ne fonctionneront pas pour vous sur le bureau avec lequel vous utilisez CustomRP, c'est une bizarrerie de Discord. Vous pouvez tester vos boutons à partir d'un téléphone ou Web, ou simplement demandez à quelqu'un d'autre à la place.

### J'ai installé CustomRP mais il ne démarre pas.

C'est probablement votre antivirus qui empêche le lancement de l'application. Ajoutez le dossier `%appdata%\CustomRP` aux exceptions.

### J'ai installé CustomRP, autorisé les analyses et l'application ne fonctionne plus.

Arrêtez l'application dans le gestionnaire de tâches, supprimez le dossier `%localappdata%\maximmax42`, redémarrez l'application et n'autorisez pas les analyses.

### L'application s'est connectée, mais je ne vois pas l'état dans mon profil

Assurez-vous d'avoir activé le statut d'activité dans les paramètres Discord :

<figure><img src="https://user-images.githubusercontent.com/112771301/196043582-9a04d91f-5c6f-4399-a705-18955e24ea04.png" alt=""><figcaption></figcaption></figure>

### L'application fonctionnait, mais maintenant elle se connecte indéfiniment.

Vous avez peut-être obtenu un délai d'attente de Discord en raison de la connexion/du changement de présence. Déconnectez-vous, attendez 5 à 10 minutes, essayez de vous reconnecter. Redémarrer Discord pourrait également aider.

### L'application indique "Mauvaise ID ?"/"Est-ce que Discord est en cours d'exécution ?" ou se connecte indéfiniment même si je suis sûr d'avoir tout fait correctement et que Discord fonctionne.

Parfois, cela est causé par BetterDiscord. Si vous l'avez installé, désinstallez-le, laissez CustomRP se connecter à Discord au moins une fois, puis réinstallez BD. Si ce n'est pas le cas, essayez d'exécuter CustomRP en tant qu'administrateur. Si cela ne vous aide pas, essayez d'ajouter `%appdata%\CustomRP` ou, si vous utilisez une version portable, le dossier dans lequel vous avez extrait CustomRP (et peut-être Discord) aux exceptions de pare-feu/antivirus, puis redémarrez votre PC (vous pouvez essayer de redémarrer uniquement Discord et CustomRP, mais dans 95% des cas, cela ne fonctionne pas). Une autre chose que vous pouvez essayer est de quitter temporairement tous les clients Discord sauf votre principal. Si cela ne vous aide pas, je n'ai jamais pu comprendre ce qui cause cela, désolé.

### L'application fonctionnait auparavant, mais maintenant elle plante et elle ne se lance plus du tout.

Vous avez peut-être inséré une longue chaîne de texte fantaisiste (ou du texte dans une langue qui utilise des lettres non latines) dans un champ et cela a planté l'application. Pour résoudre ce problème, appuyez sur Win + R, tapez `% localappdata% \ maximmax42` et supprimez ou renommez les dossiers avec CustomRP dans le nom, puis démarrez l'application. Notez que cela réinitialise complètement l'application.

### L'application n'arrête pas de planter lors de la mise à jour/de la tentative de connexion/etc.

Si vous parvenez à lancer l'application et à obtenir un rapport de plantage, et qu'il indique `System.IO.FileNotFoundException: Could not load file or assembly...`, veuillez réinstaller l'application.

Si vous ne trouvez pas de réponse à votre question/problème, envoyez un message au salon `#support` sur le serveur Discord de [CustomRP](https://www.customrp.xyz/discordserver) ou bien envoyez un message à maximmax42#5572 sur Discord ou [Ouvrir un Sujet](https://github.com/maximmax42/Discord-CustomRP/issues/new/choose).
