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
```

---

## 📸 Captures d’écran

### 1. BeVigil
Utilisé pour :
- collecter des endpoints
- détecter domaines/sous-domaines
- identifier emails publics
- cartographier assets exposés
- recenser technologies utilisées

![BeVigil](./lab1.png)

---

### 2. Yaazhini
Utilisé pour :
- analyser le contenu interne de l’APK
- rechercher secrets hardcodés
- inspecter permissions
- détecter composants exposés
- relever configurations à risque

![Yaazhini](./2lab8.png)

---

### 3. Diva sur émulateur

![Diva](./3lab8.png)
