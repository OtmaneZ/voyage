# Gestion des voyages professionnels

**Profil :** Professeur de SES (lycée) · Data Analyst en reconversion  
**Usage :** Conférences data / IA / finance — voyages solo (frais pro) ou accompagné de votre fils (part perso)

---

## Structure

```
voyage/
├── _templates/          Modèles réutilisables (budget, checklist, note de frais)
├── _references/         Politiques, contacts, plafonds
├── voyages/             Un dossier par déplacement
│   └── YYYY-MM_DESTINATION_evenement/
└── comptabilite/        Synthèses annuelles et exports remboursement
```

## Convention de nommage des voyages

```
YYYY-MM_VILLE_type-evenement
```

Exemples :
- `2026-07_LONDRES_conference-data`
- `2026-11_PARIS-summit-ia`

## Règle pro / perso

| Poste | Qui paie | Dossier |
|-------|----------|---------|
| Billet conférence, hôtel pro, transports pro | Employeur / note de frais | `04_budget/pro/` |
| Billet fils, activités, repas perso, supplément chambre | Vous (perso) | `04_budget/perso/` |
| Part mixte (ex. chambre double) | Ventiler dans `ventilation-pro-perso.md` | `04_budget/` |

## Workflow par voyage

1. **Dupliquer** `_templates/dossier-voyage/` → `voyages/YYYY-MM_...`
2. Remplir `00_resume/fiche-voyage.md`
3. Déposer les justificatifs dans les sous-dossiers `02_` à `05_`
4. Tenir `04_budget/` à jour (pro et perso séparés)
5. Après retour : compléter `06_post-voyage/` et archiver

## Prochain voyage

→ [`voyages/2026-07_LONDRES_conference-data/`](voyages/2026-07_LONDRES_conference-data/)

---

*Dernière mise à jour : juillet 2026*
