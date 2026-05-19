# Lab — Audit Défensif d’Application Mobile (BeVigil & Yaazhini)

## 📌 Présentation

Ce laboratoire a pour objectif de réaliser un **audit défensif et légal** d’une application mobile Android ou d’un domaine autorisé, en utilisant des outils d’analyse statique et OSINT spécialisés.

L’analyse s’appuie sur deux solutions principales :

- :contentReference[oaicite:0]{index=0} — pour la collecte de signaux d’exposition publics
- :contentReference[oaicite:1]{index=1} — pour l’analyse statique approfondie de l’APK

Le but n’est **pas d’exploiter** les vulnérabilités, mais de :

- identifier des indices d’exposition,
- trier les faux positifs,
- corréler les résultats avec les standards OWASP,
- produire un rapport professionnel exploitable.

---

## 🎯 Objectifs pédagogiques

À la fin de ce lab, l’apprenant sera capable de :

- Organiser un audit défensif d’application mobile
- Collecter des signaux d’exposition avec BeVigil et Yaazhini
- Identifier et filtrer les faux positifs
- Corréler les constats avec les standards OWASP
- Produire un rapport d’analyse structuré

---

## ⚖️ Cadre légal et éthique

Ce laboratoire s’inscrit dans un cadre **strictement légal et pédagogique**.

### Autorisé uniquement sur :

- APK pédagogique fourni par l’enseignant
- Application interne explicitement autorisée
- Domaine appartenant à un périmètre documenté

### Interdit :

- Exploitation de vulnérabilités
- Tests intrusifs
- Bypass de mécanismes de sécurité
- Analyse de cibles non autorisées
- Divulgation de secrets ou données sensibles

---

## 🧱 Structure du projet

```text
lab-mobile-security/
├── 00-scope/
│   ├── scope.md
│   └── targets.txt / APK
│
├── 01-bevigil/
│   ├── bevigil_export.json
│   └── bevigil_notes.md
│
├── 02-yaazhini/
│   ├── yaazhini_report
│   └── yaazhini_notes.md
│
├── 03-triage/
│   ├── triage.csv
│   ├── owasp_mapping.md
│   └── faux_positifs.md
│
├── 04-report/
│   └── rapport_final.md
│
├── analyse_info.txt
├── commands.log
└── checklist_fin.md
🔄 Workflow du laboratoire
Préparation & Périmètre
        ↓
Analyse BeVigil
        ↓
Analyse Yaazhini
        ↓
Triage & Normalisation
        ↓
Corrélation OWASP
        ↓
Rédaction Rapport
        ↓
Clôture

🛠 Outils utilisés
1. BeVigil

Utilisé pour :

collecter des endpoints
détecter domaines/sous-domaines
identifier emails publics
cartographier assets exposés
recenser technologies utilisées


 ![Diva](./3lab8.png)

2. Yaazhini

Utilisé pour :

analyser le contenu interne de l’APK
rechercher secrets hardcodés
inspecter permissions
détecter composants exposés
relever configurations à risque


![Yaazhini](https://raw.githubusercontent.com/Odnyassmine/YOUR-REPO-NAME/main/2lab8.png)

3- diva sur emulateur


 ![BeVigil](./lab1.png)

📚 Références sécurité

Ce lab s’appuie sur les standards :

OWASP
OWASP MASVS
OWASP MASTG

Principales catégories utilisées :

MASVS-STORAGE
MASVS-NETWORK
MASVS-CRYPTO
MASVS-AUTH
MASVS-PLATFORM
MASVS-CODE
MASVS-RESILIENCE
