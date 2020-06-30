# Tournament Assistant
Suite de scripts python3 pour aider à manager un *single elimination tournament.*
## Sommaire
- [Tournament Assistant](#tournament-assistant)
	- [Sommaire](#sommaire)
	- [À propos](#à-propos)
		- [Contexte](#contexte)
		- [Règles](#règles)
		- [Structure du projet](#structure-du-projet)
## À propos
L'objectif est de réaliser un tournoi 1vs1 ou 3vs3 avec élimination qui répond à des règles spécifiques.
### Contexte
Le tournoi en question est une compétition PvP entre participants du mmorpg [Dofus®](https://www.dofus.com/) sur le serveur *Merkator*. Il opposera deux adversaires (ou deux équipes de 3) dans un duel à mort, le perdant étant éliminé, et le gagnant accédant au match suivant.
### Règles
Les règles seront inspirés de la [Dofus Cup 2019](https://dofus.jeuxonline.info/actualite/56994/introduction-dofus-cup-2019). Pour le moment, elles sont définies comme ceci :
- L'équipe perdante est éliminée, l'équipe gagnante est qualifié pour le match suivant
- Chaque équipe s'il y a doit posséder 3 membres de 3 classes différentes. Leur composition devra rester la même tout au long de la compétition. A cause de leur synergie trop importante, les combinaisons suivantes sont interdites :
  - Osamodas / Sadida
  - Eniripsa / Xelor
  - Eniripsa / Sacrieur
  - Zobal / Huppermage
  - Zobal / Sacrieur
  - Sacrieur / Xelor
  - Eniripsa / Osamodas
  - Steamer / Osamodas
  - Eniripsa / Steamer
- Chaque **personnage** ne pourra participer qu'une fois au tournoi
- Les matchs essayeront dans la mesure du possible d'assurer des matchs équitables en comparant le niveau moyen de chaque équipe
### Structure du projet
Le projet sera divisé en plusieurs sous programmes articulés par un programme principal. Parmis ces sous-programmes :
- Le premier sera chargé de l'inscription des participants
- Le second s'occupera de vérifier que les règles de participation unique et de compositions sont bien respectées pendant le processus d'inscription
- Le troisième gèrera la plannification des matchs, avant et pendant le tournoi au fil des victoires
