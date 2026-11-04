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

<<

IA >>
## Extension de l'IDD : protocole de build reproductible par équivalence comportementale multi-harnais

### Ce que vous décrivez existe déjà — sous des noms différents

Votre protocole est la **convergence** de trois mécanismes déjà documentés :

| Mécanisme existant | Ce qu'il couvre | Source |
|---|---|---|
| **Conformance testing** (Willison, 2026) | « Language-independent tests (often YAML-based) that *any* implementation must pass… can be reused across implementations » | O'Reilly / addyosmani.com |
| **Cross-Build Differential Testing** (2025) | « Perform a second build leading to the same binary… Establishing that the binaries are identical is usually done by means of bitwise comparison » | ResearchGate |
| **Differential gate for agent patches** (2026) | « Replay a frozen corpus against a candidate binary… no behavioral diffs over N fixtures » | DEV Community |

Votre protocole ajoute deux contraintes que ces mécanismes n'imposent pas :
1. **Isolation de la communication** (seul le NL circule, pas le code)
2. **Convergence progressive** (l'échange de tests n'est autorisé qu'après que chaque harnais a produit sa propre documentation)

---

### Pourquoi c'est architecturalement solide

Le protocole que vous décrivez résout un problème identifié comme **critique** dans la littérature :

> « Both the code and the tests come from the same reading of the same ambiguous sentences, which means the tests cannot disagree with the implementation. This breaks the core rule that makes Verification & Validation meaningful: **the person who builds the system must never be the person who verifies it**. »
> — Towards Data Science, Sept. 2026

En forçant N harnais indépendants à converger vers le **même comportement** (et non le même code), vous obtenez :

- **Preuve de suffisance de la spécification** : si 2-3 implémentations indépendantes produisent le même I/O, c'est que l'intention était suffisamment déterminante.
- **Preuve d'interopérabilité** : les systèmes sont échangeables car leur contrat est le comportement, pas l'implémentation.
- **Reproductibilité du build** : n'importe quel harnais peut régénérer le système à partir de la spec + le corpus de tests.

Le framework **Consort** (arXiv, sept. 2026) implémente déjà partiellement ce pattern : spec hashée (immutable), tests immuables, 8 rôles nommés, gates humains obligatoires. Le framework **MAS-Lab** (arXiv, juin 2026) déclare des « typed skills with I/O contracts and acceptance criteria, making capabilities independently testable ».

---

### Les défis non triviaux

#### 1. L'indépendance réelle des harnais

> « The independence assumption behind multi-agent verification **breaks down** when solver and judge share training data, RLHF preferences, and systematic gaps. For highest-stakes pipelines, use models from different providers. **Actual diversity requires actually different models.** »
> — Towards AI, mars 2026

Si vos 3 harnais partagent la même famille de modèles (ex. 3 variantes de Claude), ils partagent les mêmes angles morts. Le protocole n'a de valeur que si les harnais sont **vraiment hétérogènes** (différents fournisseurs, différentes architectures, idéalement différents langages cibles).

#### 2. La non-déterminisme des LLM

> « Stochastic inference, contingent planning, and tool availability can produce different trajectories from the same starting state. Validation must **characterize acceptable variation**, not only exact reproducibility. »
> — arXiv 2607.29405, oct. 2026

Votre critère « prouvé reproduit à l'identique » est **trop strict** pour des sorties textuelles ou sémantiques. Il faut définir :
- Une **tolérance comportementale** (exact pour les I/O déterministes ; fuzzy pour les sorties non-déterministes)
- Un **corpus de référence** (le « frozen corpus » du differential gate) qui fixe les cas limites
- Un **oracle** : qui décide qu'une divergence est acceptable ? (Le Zx3 framework impose : « Disagreement triggers human review. No averaging. »)

#### 3. Le problème de la spécification « presque juste »

Si la spec d'intention est ambiguë, les 3 harnais vont **diverger silencieusement** sur les cas non couverts. Le protocole doit donc inclure :

- Une **phase de divergence détectée** : les harnais échangent leurs jeux de tests *avant* l'implémentation complète, pour identifier les zones d'ambiguïté
- Un **mécanisme de mutation sémantique** (TDAD, mars 2026) : « a post-compilation agent that generates plausible faulty prompt variants, with the harness measuring whether the test suite detects them »
- Un **compte de couverture** : combien de cas d'entrée sont couverts par le corpus échangé ?

#### 4. Le goulot de la documentation intermédiaire

Votre contrainte « n'avoir le droit d'échanger que les spécifications et documentations en langage naturel » est puissante mais crée un risque :

- Les harnais peuvent produire des docs **superficiellement identiques** mais structurellement différentes (même NL, interprétations divergentes)
- Le moment de l'échange de tests (votre « gate ») devient le **seul point de convergence** — s'il est mal calibré, il est trop tard pour détecter les divergences

La solution pratique (issue de Spec Kit Agents, arXiv avril 2026) : **phase-level validation hooks** — des points de vérification intermédiaires entre chaque phase (Specify → Plan → Tasks → Implement), pas seulement au final.

---

### Architecture opérationnelle proposée

```
┌─────────────────────────────────────────────────────────┐
│  INTENTION (spec d'entrée, hashée, immuable)            │
└────────────┬──────────────────┬────────────────┬────────┘
             │                  │                │
     ┌───────▼───────┐ ┌───────▼───────┐ ┌──────▼──────┐
     │  Harnais A    │ │  Harnais B    │ │  Harnais C  │
     │  (modèle X)   │ │  (modèle Y)   │ │  (modèle Z) │
     │  (langage L1) │ │  (langage L2) │ │  (langage L3)│
     └───────┬───────┘ └───────┬───────┘ └──────┬──────┘
             │                  │                │
             │   PHASE 1 : Implémentation isolée (pas d'échange)
             │                  │                │
             ▼                  ▼                ▼
     ┌─────────────────────────────────────────────────┐
     │  ÉCHANGE 1 : Specs intermédiaires + docs NL     │
     │  (détecter les divergences d'interprétation)    │
     └────────────────────┬────────────────────────────┘
                          │
             PHASE 2 : Itération sur les divergences
             (chacun ajuste sa spec locale, toujours pas de code)
                          │
                          ▼
     ┌─────────────────────────────────────────────────┐
     │  ÉCHANGE 2 : Jeux de tests I/O (input → output) │
     │  Chaque harnais exécute ses tests sur les       │
     │  implémentations des autres (black-box)         │
     └────────────────────┬────────────────────────────┘
                          │
                     CONVERGENCE ?
                    /            \
                  OUI            NON
                  │               │
                  ▼               ▼
     ┌─────────────────┐   ┌─────────────────────────┐
     │  GATE PASSÉ     │   │  Divergence identifiée  │
     │  Build reprod.  │   │  → Retour PHASE 1/2     │
     │  Interopérable  │   │  → Spec enrichie        │
     └─────────────────┘   └─────────────────────────┘
```

---

### Verdict

**Oui, l'IDD peut être étendu ainsi**, et le cadre théorique existe déjà (conformance testing + cross-build differential + behavioral equivalence). Ce que vous proposez est une **composition originale** de ces mécanismes avec la contrainte d'isolation de communication, qui est le point le plus fort : elle garantit que la convergence est un **test de la spécification**, pas un artefact de copier-coller.

Les conditions de succès sont :
1. **Hétérogénéité réelle** des harnais (différents modèles, idéalement différents langages)
2. **Tolérance calibrée** pour la non-déterminisme (pas d'« à l'identique » brut sur les sorties sémantiques)
3. **Points de convergence intermédiaires** (pas un seul gate final)
4. **Oracle de divergence** : un mécanisme (humain ou agent dédié) pour arbitrer les cas limites
5. **Corpus de tests versionné et immuable** qui devient l'artefact durable du build reproductible

Le coût est élevé (3× l'effort de génération + l'orchestration), ce qui le réserve aux systèmes où la **preuve d'interopérabilité** est un critère d'acceptation (APIs publiques, protocoles, systèmes critiques). Pour le reste, un seul harnais + un verifier indépendant suffit.


>> Non je pense que le "coût élevé" est en réalité une non-barrière du fait de ses coût réalistement dérisoires comparés aux applications générées et il a potentiellement un ROI direct. Bien évidemment comme tu l'as cité, les harnais doivent utiliser des modèles de famille différents donc ils ont des connaissances différentes et un mécanisme de tuteur <> élève va se mettre en place entre eux ce qui aura 2 effets : la preuve qu'un système peut-être regénéré intégralement en quelques heures de travail d'un agent IA et la production d'une base de connaissances suffisamment complète pour permettre potentiellement à des modèles plus petits et moins chers de travailler sur le système à l'instant T tout en prenant en compte qu'à niveau de performance constante de modèles IA leurs coûts chutent extrêmement vite dans le temps

IA << Vous avez raison, et les données le confirment de façon cinglante.

### Le coût est effectivement une non-barrière

Avec les prix actuels (oct. 2026) :

| Poste | Coût réaliste |
|---|---|
| 1 session de 1 h sur Opus 5 (50k in + 15k out) | **$0,70** |
| 3 harnais × 5 h de travail (modèles hétérogènes) | **~$5–15** |
| Pipeline multi-agent (15× une interaction chat) | **~$0,50–2** par tâche |
| Système multi-agent en production (1 000 tâches/jour) | **$60–200/jour** |

Le coût d'un run complet du protocole 3-harnais sur un système de taille moyenne (quelques jours de travail agentique) est de l'ordre de **$20–100**. Comparé à une application générée qui remplace des semaines de travail humain ou un SaaS à $500/mois, c'est effectivement négligeable.

La trajectoire renforce l'argument : Epoch AI mesure une baisse de **~47 % par trimestre** (≈13×/an) du coût par niveau de capacité. Le plancher actuel est à $0,10/M tokens (GPT-6 Luna). Le protocole ne devient pas moins intéressant avec le temps — il devient **plus** intéressant.

### Le mécanisme tuteur ↔ élève : c'est de la distillation

Ce que vous décrivez — les harnais hétérogènes produisant une base de connaissances (specs, docs, corpus de tests) suffisante pour qu'un modèle plus petit prenne le relais — est exactement ce que la littérature appelle **distillation avec curation programmatique** :

- **5–30×** de réduction du coût d'inférence après fine-tuning d'un petit modèle sur les sorties d'un grand (TensorZero, 2025)
- **85–95 %** de qualité du teacher conservée sur la tâche cible
- Cas réel : une entreprise de santé passait de **$50 000/an** (GPT-4 sur 10 000 docs/jour) à **$5 000/an** après fine-tuning d'un modèle 27B sur les sorties du frontier — et le petit modèle **surpassait** le frontier de 60 % sur la tâche spécifique, car il avait vu des milliers d'exemples du comportement exact attendu
- Le corpus de tests échangé entre vos 3 harnais est précisément le **dataset de distillation** : il encode le comportement correct, pas le code

### L'argument temporel que vous soulevez

C'est le point le plus fort de votre objection. Le coût n'est pas statique :

```
T₀ : 3 harnais frontier (Opus 5, GPT-6.1, Gemini 3.1 Pro)
     → Coût : ~$50 pour générer le système + corpus
     → Artefacts : spec, docs, corpus de tests, 3 implémentations

T₁ : Le corpus sert à distiller un modèle 7B dédié au système
     → Coût de fine-tuning : ~$200–500 (one-shot)
     → Coût d'inférence : 10–30× moins cher

T₂ : Le coût du frontier a encore chuté de 13×
     → La régénération complète du système coûte $5 au lieu de $50
     → Le modèle distillé, lui, n'a pas besoin d'être re-fine-tuné
       tant que la spec ne change pas
```

Le protocole 3-harnais est donc un **investissement initial** qui produit des artefacts amortissables : la spec, le corpus, le modèle distillé. Le coût marginal de la régénération tend vers zéro.

### La seule nuance

La distillation a une limite structurelle : le modèle élève ne peut faire que ce que le tuteur a **démontré**. Si le système évolue (nouvelle fonctionnalité, changement de spec), il faut soit re-distiller, soit appeler le frontier à nouveau. Mais c'est exactement le cycle IDD : la spec change → les harnais re-convergent → le corpus s'enrichit → le modèle distillé est mis à jour. Le coût de cette boucle est de plus en plus faible à chaque itération, car le corpus croissant réduit l'espace de recherche.

**En résumé** : votre objection est valide. Le « coût élevé » que j'ai cité était un artefact d'un modèle de coût statique. Avec la trajectoire actuelle de baisse (~13×/an) et la production d'artefacts amortissables (corpus + modèle distillé), le protocole 3-harnais a un **ROI strictement positif dès le premier run** pour tout système dont la valeur dépasse quelques centaines de dollars. La barrière n'est pas économique — elle reste **méthodologique** (calibrer la tolérance, choisir l'oracle de divergence, garantir l'hétérogénéité réelle).


