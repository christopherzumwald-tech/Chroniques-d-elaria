# ELARIA-JDR

Ce dossier est la **source de vérité** pour toutes les règles du jeu de rôle Élaria.  
Chaque sous-dossier regroupe les blocs de règles par thème ; chaque fichier suit une convention de nommage stable pour faciliter la navigation, y compris sur mobile.

---

## Structure

- **`00_CORE_SYSTEM/`** — Socle du système : statistiques, jets de dés, tour de jeu, états et mécaniques de base.
- **`01_CREATION_PERSONNAGE/`** — Création et progression des personnages : races, métiers, compétences et équipement de départ.
- **`02_COMBAT_ET_CAPACITES/`** — Moteur de combat complet : actions, réactions, interception, armes, armures et capacités spéciales.
- **`03_ECONOMIE_ET_CRAFT/`** — Économie, artisanat et objets : fabrication, coûts, améliorations et commerce.
- **`04_BESTIAIRE/`** — Créatures et adversaires : statistiques, comportements, récompenses XP et règles de dressage.
- **`05_LORE_MONDE/`** — Lore et univers : géographie, factions, histoire et éléments de contexte narratif.
- **`06_SYSTEMES_MJ/`** — Outils pour le Maître de Jeu : gestion des rencontres, aide de jeu, tables aléatoires et modules tactiques.
- **`07_MODULES_OPTIONNELS/`** — Règles optionnelles et extensions : technomagie, règles de réputation, systèmes avancés à activer à la carte.
- **`08_TEST_ET_EQUILIBRAGE/`** — Fiches de test et d'équilibrage : données de playtest, courbes de puissance et ajustements en cours.
- **`09_ARCHIVES/`** — Versions antérieures et brouillons consolidés. Le sous-dossier **`brouillons/`** contient des versions alternatives ou compilations (ex. versions "moteur complet") conservées pour référence.

---

## Convention de nommage

Tous les fichiers de règles suivent le schéma :

```
BLOC_<XX[_Y]>_<Titre>.txt
```

| Partie | Signification |
|--------|---------------|
| `BLOC` | Préfixe fixe identifiant un bloc de règles |
| `XX` | Numéro de bloc sur deux chiffres (ex. `02`) |
| `_Y` | *(Optionnel)* Sous-numéro pour les variantes ou parties d'un même bloc (ex. `_1`, `_2`) |
| `Titre` | Titre descriptif en mots séparés par des underscores, sans accents (ex. `Moteur_de_combat`) |

**Exemples :**
- `BLOC_00_Statistiques_et_Jets.txt`
- `BLOC_02_1_Actions_et_Reactions.txt`
- `BLOC_02_2_Armes_et_Armures.txt`
