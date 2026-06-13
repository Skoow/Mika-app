# Mika-app — Programme de musculation de Michael

## ⚠️ Règle de travail (consigne du propriétaire)

**TOUT se fait sur la branche `main`. C'est la seule branche du dépôt.**

- Développe directement sur `main`.
- À chaque mise à jour demandée par le propriétaire, commit puis **push automatiquement sur `main`** (`git push origin main`) — sans créer de Pull Request et sans demander confirmation pour la branche.
- **Ne crée jamais** de branche `claude/*` ni aucune autre branche de travail.
- Pas de Pull Request sauf demande explicite.

## Contenu du dépôt

- `index.html` — application web autonome (PWA) du programme de musculation de Michael.
  - Single-file : HTML + CSS + JS inline, icônes SVG générées, aucune dépendance.
  - Stockage local (`localStorage`) : poids saisis, historique, cases cochées.

## Le programme

- **Split 4 jours** (niveau débutant/intermédiaire), basé sur le programme d'Anthony :
  - **LUN** — Haut du corps A
  - **MAR** — Bas du corps A
  - **JEU** — Haut du corps B
  - **VEN** — Bas du corps B
- **Format 4×12**, **6 exercices par jour** (hors bonus).
- **Bonus un jour sur deux** : Abdos 4×12 (Lun/Jeu), Pompes 4×12 (Mar/Ven).
- Exercices durs aux haltères convertis en machines guidées ; haltères gardés uniquement pour les mouvements faciles (curl, élévations latérales).

## Fonctionnalités de l'app

- Cocher / décocher chaque exercice (progression X/6 + barre).
- Saisie du poids en **kg** avec mémorisation et suggestion de progression (+2,5 kg après 3 séances réussies).
- Fuseau horaire **Europe/Paris**.
- **Réinitialisation hebdomadaire** des cases cochées au changement de semaine ISO (nuit dimanche→lundi). Les poids enregistrés sont conservés.
- Compteur **J–XX** (révision du programme) qui se décompte automatiquement. Programme calé sur ~2 mois (révision au 13 août 2026).
