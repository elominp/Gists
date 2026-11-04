<< Quel est l'historique de la méthodologie Intent-Driven-Development ? (ie chronologiquement quand a-t-elle été conçue, sur quels principes historique se base-t-elle et quelles sont ses évolutions)

AI >>
## Historique de l'Intent-Driven Development

L'IDD n'est pas une invention soudaine : c'est la convergence de plusieurs courants historiques qui ont progressivement déplacé le centre de gravité du développement logiciel de **l'exécution** vers **l'intention**.

### Racines philosophiques et industrielles

- **1805** — Les *Portsmouth Block Mills* de Brunel et Maudslay déléguent pour la première fois l'exécution à la machine à grande échelle. Le principe sous-jacent : *« first get a clear notion of what you desire to accomplish »* — l'intention précède et gouverne l'exécution.
- **1968** — La conférence NATO de génie logiciel nomme la **« crise du logiciel »** : l'écart entre ce qu'on veut construire et ce qui est effectivement construit devient le problème central.
- **1969** — Tony Hoare publie sa logique (précondition / action / postcondition), fondement formel de toute spécification d'intention.
- **1986** — Bertrand Meyer introduit le **Design by Contract** avec le langage Eiffel : l'intention est encodée directement dans le code.
- **1987** — Michael Bratman formalise l'architecture **BDI** (Belief–Desire–Intention) : un agent rationnel maintient des croyances, des désirs et des intentions distinctes. Ce modèle devient la référence pour les agents autonomes.

### L'ancêtre direct : Intentional Programming

- **1995** — Charles Simonyi propose **Intentional Programming** à Microsoft Research : le programmeur capture l'intention de l'utilisateur et le code n'est qu'un rendu de cette intention. Il construit un IDE de démonstration d'ici mars 1995.
- **2002** — Microsoft décide de ne pas productiser le paradigme. Simonyi quitte Microsoft Research et fonde Intentional Software Corporation avec Gregor Kiczales. L'entreprise développe des outils (language workbenches, séparation fonction/implémentation) mais ne parvient pas à imposer le paradigme à l'industrie.

### Le terreau méthodologique

- **2003–2008** — Émergence du **BDD** (Behavior-Driven Development) avec Dan North, Cucumber/Gherkin : l'intention est exprimée en langage naturel et devient exécutable.
- **2004** — Première publication du terme *« specification-driven development »* (Ostroff, Paige, Makalsky, conférence XP).
- **2011** — *Specification by Example* (Gojko Adzic) consolide l'idée que les exemples *sont* la spécification.

### L'accélération IA

| Période | Événement | Effet |
|---|---|---|
| 2021 | OpenAI Codex | Première génération de code depuis le langage naturel ; révèle l'écart entre code plausible et intention réelle |
| 2022 | GitHub Copilot GA ; ReAct (Yao et al.) | L'assistant IA devient courant ; le pattern raisonnement + action structure les agents |
| 2023 | BabyAGI, AutoGPT | Explosion des agents autonomes LLM ; la boucle *objectif → plan → exécution → réévaluation* se démocratise |
| 2024 | « Vibe coding » ; MCP (Anthropic) | Les développeurs itèrent avec l'IA de façon informelle ; la qualité de l'intention devient le goulot d'étranglement |
| 2025 | Ongle d'outils spec-driven (Auto, Kiro, Intent…) ; Gartner prévoit 60 % de code généré par IA d'ici fin 2026 | La spécification explicite réapparait comme mécanisme de contrôle |
| 2026 | **IDD formalisé** (ebook *Intent-Driven Development*, janvier 2026) ; « Software Engineering 3.0 » | Le paradigme est nommé, structuré et enseigné : **Intention → Implémentation (IA) → Vérification** |

### En résumé

L'IDD est la **réunification** de trois fils historiques :
1. Le fil **spécification** (Hoare → Meyer → BDD → SDD) : dire *quoi* avant de dire *comment*.
2. Le fil **agentique** (BDI → ReAct → agents LLM) : déléguer l'exécution à un système autonome.
3. Le fil **intentionnel** (Simonyi → Intentional Programming) : faire de l'intention l'artefact premier, le code n'étant qu'un rendu.

Ce qui était académique et prématuré en 1995 est devenu opérationnel en 2025-2026, porté par la maturité des agents LLM capables d'exécuter autonomément des tâches de 5 à 7 heures. Le goulot d'étranglement n'est plus l'implémentation mais **la qualité de l'intention spécifiée**.

<< Quel est le taux de diffusion, d'adoption et de rejet de cette méthodologie ? (Ie quelle plage de la population en a entendu parler et comment et parmi cette population quelle est la partie qui l'utilise et surtout quelle est la partie qui ne l'utilise pas et pourquoi)

AI >>
## Diffusion, adoption et rejet de l'IDD

### Mise en garde méthodologique

L'IDD en tant que **méthodologie nommée** est extrêmement récente (formalisée début 2026). Aucune enquête n'a encore mesuré sa notoriété sous ce label précis. Les données disponibles concernent la **pratique sous-jacente** — spec-driven development, intent-based workflows, vibe coding structuré — qui constitue le socle opérationnel de l'IDD.

---

### 1. Notoriété (awareness)

| Indicateur | Chiffre | Source |
|---|---|---|
| Développeurs ayant entendu parler d'outils IA de code | **84–91 %** | Stack Overflow 2025, JetBrains 2026 |
| Utilisent au moins un outil IA | **83 %** | Stack Overflow 2026 |
| Utilisent des agents IA | **59 %** | Stack Overflow pulse, avril 2026 |
| Recherches mensuelles « spec-driven development » (US) | **17 380** (mars 2026) vs 53 (juin 2025) | Ahrefs |
| Repos GitHub publics contenant des fichiers de spécification | **73 000+** | Étude arXiv 2026 |
| Notoriété du terme « Intent-Driven Development » spécifiquement | **Inconnue** — trop récent pour être mesuré | — |

**En résumé** : la *pratique* (spécifier l'intention avant de coder avec l'IA) est connue de l'immense majorité des développeurs. Le *nom* « IDD » lui-même est encore cantonné à une petite minorité (auteurs, conférenciers, early adopters).

---

### 2. Adoption effective

| Indicateur | Chiffre | Source |
|---|---|---|
| Développeurs utilisant des outils IA **régulièrement** | **85 %** | JetBrains, janv. 2026 |
| Utilisation quotidienne | **51 %** | Stack Overflow 2025 |
| « Vibe coding » (création de projets majoritairement générés par IA) | **48 %** | SonarSource 2026 |
| Développeurs disant que l'IA écrit **50 %+** de leur code | **42 %** | BairesDev, T3 2026 |
| Prêts à déléguer l'écriture de la logique applicative à l'IA | **50 %** (vs 18 % en mai 2025) | JetBrains, mai–juil. 2026 |
| Adoption de workflows spec-driven (outils dédiés : Spec Kit, Kiro, OpenSpec…) | **~18 %** des développeurs (Claude Code, le plus représentatif) ; 10 000+ repos par outil | JetBrains, arXiv 2026 |
| Gain de productivité mesuré avec workflows structurés | **3,6 h/semaine** d'économie | DX Research |
| Taux de succès au premier passage (agents + specs) | **3 à 10×** supérieur sans specs | DevToolLab 2026 |

**En résumé** : la pratique informelle (décrire l'intention en langage naturel, laisser l'IA coder) est quasi universelle. L'adoption **formelle et outillée** de l'IDD (fichiers de spécification structurés, outils dédiés, vérification systématique) reste à **~15–25 %** de la population active.

---

### 3. Rejet et résistance

C'est le segment le plus documenté et le plus nuancé. On distingue **trois strates de rejet** :

#### a) Rejet de l'approche « vibe coding » non structurée

- **72 %** des développeurs rejettent le vibe coding pour le travail professionnel (Stack Overflow 2025).
- **66 %** citent comme frustration n°1 le code « presque juste, mais pas tout à fait ».
- **38 %** disent que réviser du code IA prend **plus d'effort** que réviser du code humain (Sonar 2026).

→ Ces développeurs ne rejettent pas l'IDD *en soi* ; ils rejettent son **absence** (coder sans intention structurée). Ils constituent en réalité la **demande latente** de l'IDD.

#### b) Rejet de la délégation à l'IA (même avec spécification)

| Raison | Données |
|---|---|
| **Manque de confiance** | **96 %** ne font pas pleinement confiance au code IA (Sonar 2026) ; **46 %** font activement défiance ; seulement **3 %** déclarent une « confiance élevée » |
| **Défauts de qualité** | 1,7× plus de défauts par PR ; 2,74× plus de vulnérabilités (CodeRabbit) ; +41 % de bugs |
| **Illusion de productivité** | Étude METR : développeurs expérimentés **19 % plus lents** avec l'IA, tout en croyant être 20 % plus rapides |
| **Perte de maîtrise / de craft** | Vidéo virale « I'm done with AI » : **900 000+ vues** ; raisons : érosion du savoir-faire, perte d'identité professionnelle, coûts psychologiques |
| **Spécification comme dette** | « Mettre à jour la spec est plus dur que mettre à jour le code » → dette documentaire déguisée en discipline (DEV Community) |
| **Intention « presque juste »** | « Un fichier d'intention presque juste est pire qu'un fichier absent, car tout en aval l'hérite avec confiance » (agenticaiarch.com) |
| **Skepticisme des seniors** | Les développeurs les plus expérimentés sont les plus méfiants : taux de « confiance élevée » de **2,6 %** vs 3 % en moyenne |

#### c) Rejet du paradigme lui-même

- Une partie des développeurs rejette la **prémisse même** de l'IDD : l'idée que l'intention peut être formalisée suffisamment pour que l'IA l'exécute correctement.
- Argument récurrent : l'intention logicielle est **incomplète par nature** — elle ne capture pas les invariants implicites, les contraintes contextuelles, les trade-offs non explicitables.
- Sur Hacker News (oct. 2026) : « *For me it breaks the rule of "Network of trust". Software works because someone is accountable for it.* »
- Certains voient l'IDD comme une **rebranding** du waterfall (« écrire la spec avant de coder ») déguisé en innovation.

---

### 4. Synthèse en entonnoir

```
~90 %  →  ont entendu parler d'outils IA / du principe « décrire l'intention »
 ~85 %  →  utilisent des outils IA régulièrement (pratique informelle)
 ~50 %  →  prêts à déléguer la logique applicative à l'IA
 ~20 %  →  utilisent des workflows spec-driven / IDD formels (outils dédiés)
 ~15 %  →  pratiquent l'IDD de manière systématique et mesurée
 ~70 %  →  rejettent le vibe coding non structuré (demande latente pour l'IDD)
 ~96 %  →  ne font pas confiance au code IA sans vérification
  ~3 %   →  déclarent une confiance élevée dans le code IA
```

**Le paradoxe central de 2026** : la majorité des développeurs *veut* l'IDD (rejet du vibe coding, appel à la gouvernance) mais *ne le pratique pas encore* formellement, faute de confiance dans l'exécution IA et par inertie méthodologique. Le goulot d'étranglement n'est pas la volonté de spécifier l'intention, c'est la **confiance dans la capacité de l'IA à l'exécuter fidèlement**.

