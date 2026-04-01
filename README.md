# Never Again Paradox — Research Prototype

## מחקר: פרדוקס ה-"Never Again"
### האם חשיפה לדימויי שואה מגבירה ציות לסמכות?

**חוקר:** ניר | **מנחה:** דנה  
**אוניברסיטת חיפה — החוג לפסיכולוגיה**  
**סמינריון: המוח הרגשי**

---

### Flow
1. Informed consent
2. Photo exposure (8 Holocaust images, 10s each, randomized)
3. DEQ — Discrete Emotions Questionnaire (fear, anger, disgust, sadness)
4. Filler task (word completion)
5. HR obedience simulation (10 escalating steps)
6. Manipulation check
7. Demographics
8. Debriefing
9. JSON data export

### Deployment
This is a single self-contained HTML file. All images are embedded as base64.

**GitHub Pages:**
1. Create a new repo
2. Push this folder
3. Go to Settings → Pages → Source: main branch
4. Your study will be live at `https://[username].github.io/never-again-paradox/`

### Data Output
Each participant generates a JSON object containing all measures:
- `deq.subscales` — mean scores per emotion subscale
- `simulation.compliance_score` — 0-10 obedience score
- `simulation.steps[]` — per-step decisions with reaction times
- `manipulation_check` — demand characteristics assessment
- `demographics` — participant background

### Design
- **IV:** Holocaust image exposure (experimental) vs. neutral images (control)
- **Mediator:** Differential emotional arousal (DEQ subscales)
- **DV:** Administrative obedience (compliance score 0-10)
- **Analysis:** PROCESS Model 4 (simple mediation)
- **Target N:** 120
