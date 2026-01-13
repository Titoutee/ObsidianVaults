# Théorème de Zermolo
Soit un jeu:
- 2 joueurs
- Tour par tour
- Information complète
- Déterministe
- Sans match nul
- Sans cycle

***Alors un joueur possède une stratégie gagnante.***

---
*Soit `s` un état du jeu, on note `p(s)` sa profondeur, càd la longueur de la plus longue partie depuis s. 
On va montrer que tout état `s` est gagnant pour un joueur, par récurrence sur `p(s)`.
**Init**: `p(s)=0` donc `s` est terminal. Comme le jeu n'a pas de match nul, l'état ` s ` est gagnant pour 1 joueur. 

***Hérédité**: tous les successeurs de `s` ont une profondeur `<= p(s)-1`.
Par **HR**, tous les successeurs sont gagnants pour un joueur.*