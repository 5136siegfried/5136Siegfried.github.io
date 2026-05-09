# 5136.fr — Portfolio DevOps / SRE

Vitrine personnelle de [Siegfried Sekkai](https://5136.fr) — ingénieur DevOps / SRE.

→ **[5136.fr](https://5136.fr)**

---

## Stack

Site statique en HTML/CSS pur. Aucun framework, aucune dépendance, aucun build step.
Un `git push` suffit à déployer via GitHub Pages.

```
index.html     — page principale
CNAME          — 5136.fr
.nojekyll      — désactive le build Jekyll de GitHub Pages
```

## Architecture

```
DNS (5136.fr)
├── 5136.fr / www        → GitHub Pages (ce repo)
├── maraude.5136.fr      → VPS OVH (nginx + docker)
├── chrono.5136.fr       → VPS OVH (nginx + docker)
└── csor.fr              → site asso indépendant
```

## Projets référencés

**Infrastructure & SRE**
- [SRE Good Practice](https://github.com/5136siegfried/SRE-good-practice) — référentiel SLO/runbooks/post-mortems
- [VPS GitOps OVH](https://github.com/5136siegfried/vps-gitops-ovh) — runbook sécurisation VPS nginx/docker
- [Distributed JMeter Ansible](https://github.com/5136siegfried/distributed-jmeter-ansible) — cluster de charge automatisé
- [Malus Maladat](https://github.com/5136siegfried/malus-maladat) — inventaire et audit AWS

**Outils**
- [CV Terminal](https://github.com/5136siegfried/cv-terminal) — CV interactif en invite de commande
- [LaTeX CV](https://github.com/5136siegfried/latex-cv) — générateur de CV PDF modulaire
- [Job Tracker DevOps](https://github.com/5136siegfried/jobtracker-devops) — suivi de prospection CDI/freelance
- [Chrono](https://chrono.5136.fr) — timer sport / productivité

**Action sociale**
- [Come Together](https://github.com/5136siegfried/come-together) — app React/MongoDB gestion de maraudes
- [Maraude Dashboard](https://maraude.5136.fr) — dashboard de pilotage terrain
- [CSOR](https://csor.fr) — site de l'association
- [CSOR Gestion](https://github.com/5136siegfried/csor-gestion) — gouvernance horizontale
- [Hestia](https://github.com/5136siegfried/hestia) — ressources droit au logement

**Expérimental**
- [Chess-py](https://github.com/5136siegfried/chess-py) — serveur d'échecs Python/WebSocket

## Déploiement

```bash
# Modifier index.html, puis :
git add index.html
git commit -m "feat: ..."
git push
# → en ligne en < 60s
```

## Licence

Code source : [MIT](LICENSE)