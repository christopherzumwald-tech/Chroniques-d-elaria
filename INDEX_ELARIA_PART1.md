# INDEX ELARIA - PARTIE 1/3
## Analyse Complète des 40 Fichiers Final

---

## TABLE DES MATIERES

### BLOC 1 - CREATURES
- Final_1: Créatures - Niveaux de dangerosité
- Final_5: Créatures et XP

### BLOC 2 - SYSTEME DE BASE
- Final_2: Système de base (Stats, Jets)
- Final_3: Combat (Structure tour)
- Final_4: Équipement et États
- Final_6: Systèmes MJ et Addons
- Final_7: Moteur de combat (Variante)

### BLOC 3 - CREATION ET COMBAT
- Final_8: Création de personnage
- Final_9: Système de combat (Variante 2)
- Final_10: Armes

### BLOC 4+ - SYSTEMES AVANCES ET COMPILATIONS
- Final_11-19: Blocs avancés
- Final_20-38: Compilations modulaires
- Final_39-40: Mises à jour et règles

---

## BLOC 1 - CREATURES

### Final_1.txt - Bloc 1: Créatures
**Contenu:**
- Niveaux de dangerosité: Normal, Vétéran, Supérieur, Élite, Boss
- Classes spéciales: 
  - Apex: prédateur ultime d'un biome, très rare, puissance = Boss
  - Légendaire: créature unique par continent, plus puissante qu'Apex
  - Créatures majestueuses: léviathans, méduses célestes, raies

**Capacités selon niveau:**
- Normal: 2 capacités
- Vétéran: 3 capacités (dont 1 niveau 1)
- Supérieur: 4 capacités (max niveau 1, min 1 niveau 0)
- Élite: 1 niv 2 + 2 niv 1 + 1 niv 0
- Boss: 2 niv 2 + 1 niv 1 + 1 niv 0

**Équipement créatures semi-intelligentes:**
- Normal: armes simples corps à corps
- Vétéran: armes distance simples (arc, fronde)
- Supérieur: magitek non magique (fusils, pistolets)
- Élite: artefacts magiques possibles
- Boss: accès complet magie, artefacts, magitek

### Final_5.txt - Bloc 2.4: Créatures et XP
**Contenu:**
- Rangs: Normal, Vétéran, Supérieur, Élite, Boss
- Classes spéciales: Apex, Légendaire, Majestueux

**Formule XP:**
```
XP = Grade × Niveau de base
Normal=1, Vétéran=2, Supérieur=3, Élite=5, Boss=8
```

---

## BLOC 2 - SYSTEME DE BASE

### Final_2.txt - Bloc 2.1: Système de base

**10 Statistiques principales:**
- FOR (Force): puissance physique, blocage, armes lourdes
- AGI (Agilité): esquive, initiative, déplacement
- END (Endurance): résistance physique, encaissement
- INT (Intelligence): analyse, connaissances, raisonnement
- SAG (Sagesse): perception, jugement, intuition
- PRE (Précision): tir, visée, armes distance
- TEC (Technique): maîtrise technique, armes flexibles
- VOL (Volonté): résistance mentale, détermination
- CHA (Charisme): influence sociale, présence
- MAG (Magie): usage et défense magique

**Chance:**
- Valeur fixe obtenue à la création (1d20)

**Jet standard:**
- Formule: 1d20 + statistique + bonus
- Comparé à une difficulté ou jet opposé

**Difficultés standards:**
- Facile: 8
- Standard: 12
- Difficile: 16
- Très difficile: 20

**Critiques:**
- 1 naturel: échec critique
- 20 naturel: réussite critique

**Points de Vie:**
```
PV = 5 + END + floor(FOR / 2)
```

**Initiative:**
```
Initiative = AGI + bonus
En cas d'égalité: comparer AGI, puis Chance
```

### Final_3.txt - Bloc 2.2: Combat

**Structure d'un tour:**
1. Déplacement
2. Action
3. Réaction

**Déplacement:**
- Distance: AGI / 2 mètres
- Utilisé AVANT l'action
- Le déplacement restant conservé pour réactions

**Réactions possibles:**
- Esquive (AGI)
- Encaisser (END)
- Bloquer (FOR)
- Défense magique (MAG)
- Interception (conditions spéciales)

**Interception:**
- Utilise la réaction
- 1 fois par combat SEULEMENT
- Nécessite AU MOINS 1 m de déplacement restant

**Attaques:**
- Jet: 1d20 + statistique appropriée
- Comparé au jet de défense

### Final_4.txt - Bloc 2.3: Équipement et États

**Dégâts d'armes:**
- Dague: 1d2
- Arme une main: 1d4
- Arme lourde: 1d8
- Arme distance: 1d4

**Armures:**
- Aucune: dégâts complets
- Armure légère: -1 dégât
- Armure lourde: -2 dégâts

**Poids des armes:**
- Dague: 0
- Arme distance: 1
- Arme une main: 2
- Arme lourde: 3

**États majeurs:**
- Gelé
- Sonné
- Immobilisé
- Aveuglé

**États mineurs:**
- Enflammé
- Empoisonné
- Enfumé
- Affaibli
- Ralenti

### Final_6.txt - Bloc 2.5: Systèmes MJ et Addons

**Rumeurs et enquêtes:**
- Actions visibles joueurs = rumeurs possibles
- Traces laissées = enquêtes possibles

**Réputation:**
- 6 coches positives = +1 réputation
- 6 coches négatives = -1 réputation
- Échelle: -5 à +5

**Addons tactiques optionnels:**
- Flanc: +2 attaque si cible entre deux ennemis
- Attaque coordonnée: +1 attaque pour 2e attaquant
- Terrain avantageux: +1 attaque ou défense
- Pression: jet AGI (12) pour désengager si encerclé

### Final_7.txt - Bloc 2: Moteur de combat (VARIANTE)

**Structure d'un tour:**
- Mouvement: AGI / 2 cases
- Action: une seule par tour
- Réaction: esquive, blocage, encaissement ou interception

**Initiative:**
```
Initiative = AGI + bonus
Égalité joueurs: discussion ou jet
Égalité joueur/ennemi: joueur prioritaire
```

**Engagement:**
- Personnage engagé = portée d'arme ET attaqué

**Désengagement:**
- Peut utiliser action ou réaction
- Permet quitter combat SANS attaque d'opportunité

**Interception:**
- Nécessite réaction ET être désengagé
- Test de force possible pour prendre place de cible

---

## OBSERVATIONS PARTIE 1

**Redondances détectées:**
- Final_2 vs Final_3: Chevauchement structure (stats + combat)
- Final_3 vs Final_7: Deux versions du système combat (variation mineure)

**Cohérence:**
✓ Système stats unifié
✓ Formules PV cohérentes
✓ Initiative compatible
✓ Dégâts d'armes constants

---

**FIN PARTIE 1/3**
*Partie 2 arrive dans 1 minute...*