# Vote anonyme

Application de vote pour une **élection interne**. Chaque personne est à la fois
électeur et candidat : elle choisit **exactement 3 personnes** (jamais elle-même),
une seule fois, à l'aide d'un **code personnel** qui lui est remis.

## Anonymat garanti

Deux registres séparés dans un Google Sheet :

- **Participants** — qui a voté (émargement)
- **Urne** — les bulletins seuls, mélangés

Les deux ne sont jamais reliés : l'administrateur voit **qui** a voté, jamais
**pour qui**.

## Composition

- `Code.gs` — le moteur (Google Apps Script)
- `Admin.html` — le tableau de bord de l'administrateur
- `index.html` — l'application de vote des électeurs

## Déroulement

L'administrateur ajoute les participants, distribue les codes, ouvre le vote.
Chacun vote depuis son téléphone. À la clôture, les résultats s'affichent et les
3 personnes les plus votées sont élues.