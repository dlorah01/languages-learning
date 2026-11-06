---
layout: default
title: "Lesson 91: Deep Dive 11 - Technical Writing and Documentation"
---

# Lesson 91 — Deep Dive 11: Technical Writing and Documentation in French
### Phase 5: Mastery & Maintenance — Optional Deep Dive

**Competency axes trained:** ✍️ Writing (primary) · 📚 Lexicon · 🎭 Register · 🧱 Discourse · 💼 Professional communication
**Prerequisites:** Lesson 32 (business French), Lesson 33 (academic and technical French), Lesson 53 (your field's vocabulary), Lesson 66 (professional mastery), Lesson 90 (writing studio)
**Time investment:** One read, then a four-week deep-dive cycle (Lesson 80, Section 7).

---

## 1. What Makes Technical Writing Different

Technical writing is not literary writing with technical words. Its goal is **action and accuracy**: the reader must be able to *do* something or *decide* something, without misunderstanding. The qualities that matter:

| Quality | Meaning |
|---|---|
| **Précision** | one term, one meaning; no ambiguity |
| **Concision** | no padding; every sentence earns its place |
| **Cohérence** | same term for the same concept throughout |
| **Structure** | headings, lists, numbering, tables so the reader can scan |
| **Neutrality** | impersonal tone, few adjectives, no rhetoric |
| **Vérifiabilité** | claims backed by data, sources, or tests |

**Mental model: documentation is an interface.** Just as an API must be predictable, a document must be predictable: the reader should know where to look and what each part means.

Your systems-oriented mind is an advantage here: technical French rewards consistent structure and rigorous vocabulary.

---

## 2. Instructions and Procedures: Verb Forms

French has several conventions for instructions. Choose one per document and stay consistent.

| Form | Example | Typical use |
|---|---|---|
| **Infinitive** | *Cliquer sur « Enregistrer ».* | printed manuals, labels, impersonal procedures, recipes |
| **Imperative (vous)** | *Cliquez sur « Enregistrer ».* | software UIs, user guides, tutorials addressed directly to the reader |
| **Imperative (tu)** | *Clique sur « Enregistrer ».* | informal tutorials, community docs, developer blogs |
| **Present, impersonal** | *L'utilisateur clique sur « Enregistrer ».* | descriptions of how a system works |
| **Obligation verbs** | *Il faut redémarrer le service.* | warnings, requirements |

### 2.1 Numbered steps
Each step = one action, starting with a verb, one sentence.

> 1. Ouvrez le terminal.
> 2. Placez-vous dans le dossier du projet.
> 3. Lancez la commande d'installation.
> 4. Vérifiez que le service démarre sans erreur.

Put **conditions before actions**: *Si le fichier n'existe pas, créez-le.* Put **results after actions**: *Cliquez sur « Valider ». Un message de confirmation s'affiche.*

### 2.2 Warnings
| Level | Typical wording |
|---|---|
| **Information** | *Remarque : …* / *Note : …* |
| **Recommandation** | *Il est recommandé de …* |
| **Attention** | *Attention : cette opération est irréversible.* |
| **Danger** | *Danger : risque de perte de données.* |

---

## 3. Requirements and Specifications

Specifications distinguish **obligation, recommendation, and permission** precisely (like the keywords MUST / SHOULD / MAY used in many technical standards). French writers use:

| Strength | French | Example |
|---|---|---|
| **Obligation** | *doit / doivent*, *il est obligatoire de*, *est tenu de* | *Le système doit chiffrer les données.* |
| **Prohibition** | *ne doit pas*, *il est interdit de* | *Le mot de passe ne doit pas être enregistré en clair.* |
| **Recommendation** | *devrait*, *il est recommandé de* | *Le service devrait répondre en moins de 200 ms.* |
| **Permission / option** | *peut*, *est autorisé à*, *il est possible de* | *L'utilisateur peut exporter les résultats.* |
| **Capability** | *permet de*, *est capable de* | *L'outil permet de générer un rapport.* |

> **Care:** *il ne doit pas* (prohibition) differs from *il n'est pas obligé de* (not required). Check the negation: *Il ne doit pas* ≠ *Il ne doit pas nécessairement*.

### 3.1 Structure of a requirement
**Subject + modal + verb + object + measurable criterion.**

> *L'application doit afficher la page d'accueil en moins de deux secondes pour 95 % des requêtes.*

Avoid vague words: *rapide, convivial, robuste, souple* unless defined.

---

## 4. Typical Documents and Their Structures

### 4.1 README / user guide (*guide d'utilisation*)
1. **Titre et description** (what the project is)
2. **Prérequis**
3. **Installation**
4. **Utilisation** (examples)
5. **Configuration**
6. **Contribuer**
7. **Licence**
8. **Contact / support**

### 4.2 Report (*rapport technique*)
1. **Résumé** (executive summary, short and self-contained)
2. **Contexte et objectifs**
3. **Méthodologie**
4. **Résultats**
5. **Analyse / discussion**
6. **Limites**
7. **Recommandations**
8. **Annexes**

### 4.3 Incident analysis (*analyse a posteriori*, post-mortem; in France also *retour d'expérience* or **REX**)
Chronologie → impact → cause(s) racine(s) → ce qui a bien fonctionné → ce qui doit être amélioré → actions correctives (avec responsable et date).

### 4.4 Meeting minutes (*compte rendu*)
Participants → ordre du jour → décisions → actions (qui, quoi, quand).

### 4.5 Commit messages, tickets, and code comments
Conventions vary by team. In French-speaking teams, some write in French, others in English; follow your team's rule. Typical French style for a commit or ticket title: short, in the **infinitive** or **present**, no final period:

> *Corriger le calcul de la TVA*
> *Ajoute la validation des champs obligatoires*

(Choose one convention: infinitive or present, and use it consistently.)

---

## 5. Technical Vocabulary (France and Québec)

French has official terminology recommendations (in France, the *FranceTerme* database; in Québec, the *Grand dictionnaire terminologique* of the OQLF). In practice, French-speaking engineers often use English terms, so you need both.

### 5.1 Software and computing
| English | French (common) | Notes |
|---|---|---|
| software | *logiciel* (m.) | |
| computer | *ordinateur* (m.) | in Québec also *ordinateur* |
| application / app | *application* (f.) | |
| file / folder | *fichier* (m.) / *dossier* (m.) | |
| database | *base de données* (f.) | |
| data | *données* (f. pl.) | *une donnée* |
| library | *bibliothèque* (f.) | **not** *librairie* (bookshop) |
| bug | *bogue* (m.), *anomalie* (f.), *bug* | *bogue* is the recommended form; *bug* is common in speech |
| to debug | *déboguer* | |
| to deploy | *déployer* | |
| to download / upload | *télécharger* / *téléverser* (*téléverser* is the recommended form; Québec uses it widely) | |
| cloud | *nuage*, *informatique en nuage*; *infonuagique* (Québec) | |
| server | *serveur* (m.) | |
| request | *requête* (f.) | |
| response | *réponse* (f.) | |
| browser | *navigateur* (m.) | |
| settings | *paramètres* (m. pl.), *réglages* | |
| user | *utilisateur* (m.) | |
| password | *mot de passe* (m.) | |
| email | *courriel* (m., recommended), *e-mail*, *mail* | *courriel* is standard in Québec |
| version | *version* (f.) | |
| update | *mise à jour* (f.) | |
| interface | *interface* (f.) | |
| API | *API* (f.), *interface de programmation* | |
| repository | *dépôt* (m.) | |
| branch | *branche* (f.) | |
| commit | *commit* (m.), *validation* (f.) | usage varies |
| pull / merge request | *demande de fusion* | varies by tool |
| test | *test* (m.) | *tests unitaires*, *tests d'intégration* |
| pipeline | *chaîne d'intégration continue* / *pipeline* | |

> **Honesty note:** the "official" term and the term actually used on a team often differ. Learn both and follow your team's usage.

### 5.2 Data and AI
| English | French |
|---|---|
| dataset | *jeu de données* |
| machine learning | *apprentissage automatique* |
| deep learning | *apprentissage profond* |
| neural network | *réseau de neurones* |
| training / to train | *entraînement* / *entraîner* |
| model | *modèle* (m.) |
| feature | *variable explicative*, *caractéristique* |
| prediction | *prédiction* (f.) |
| accuracy | *exactitude*, *précision* (be careful: in statistics *précision* has a distinct meaning from "accuracy") |
| overfitting | *surapprentissage*, *surajustement* |
| outlier | *valeur aberrante* |
| mean / median | *moyenne* / *médiane* |
| standard deviation | *écart type* |
| confidence interval | *intervalle de confiance* |
| sample | *échantillon* (m.) |

### 5.3 Engineering and general technical
*cahier des charges* (specifications document), *conception* (design), *mise en œuvre* (implementation), *essai* / *test*, *maintenance*, *fiabilité*, *contrainte*, *tolérance*, *marge d'erreur*, *rendement* (efficiency), *débit* (throughput/flow), *charge* (load), *panne* (failure), *défaillance*, *dépannage* (troubleshooting).

### 5.4 Gender and spelling traps
*un logiciel, un code, un fichier, un serveur, un algorithme, un paramètre, un programme, un système*; *une donnée, une variable, une fonction, une requête, une bibliothèque, une application, une interface, une base*. Remember: *une API*, *un bug*, *une URL*, *un pixel*, *une mémoire*.

### 5.5 Units and numbers
- Decimal **comma**: *3,5 s*; thousands separated by a space: *12 000*.
- A (non-breaking) space between number and unit: *5 Mo*, *200 ms*, *95 %*.
- French uses **octet** (symbol *o*): *Mo, Go, To* (Mo = megaoctet). The word *byte* appears in English texts; in French use *octet* unless you mean a non-8-bit byte.
- Dates: *le 6 novembre 2026*; numeric day/month/year order: *06/11/2026* (or ISO: *2026-11-06* in technical contexts).

---

## 6. Describing Data, Graphs, and Trends

### 6.1 Movement verbs and nouns
| Direction | Verbs | Nouns |
|---|---|---|
| **Up** | *augmenter, croître, progresser, grimper* | *une hausse, une augmentation, une progression, une croissance* |
| **Down** | *diminuer, baisser, reculer, chuter* | *une baisse, une diminution, un recul, une chute* |
| **Stable** | *stagner, se stabiliser, rester stable* | *une stagnation, un plateau* |
| **Peak / trough** | *atteindre un pic / un minimum* | *un pic, un maximum, un minimum, un creux* |
| **Fluctuate** | *fluctuer, osciller* | *une fluctuation* |

### 6.2 Quantifying
- *Le chiffre d'affaires a augmenté **de** 12 % (the amount of change) **pour atteindre** 3,4 M€ (the result).*
- *Le temps de réponse est **passé de** 450 ms **à** 180 ms.*
- *Une hausse **de** 5 points* (percentage points) ≠ *une hausse **de** 5 %* (relative change).
- *Environ, près de, plus de, moins de, de l'ordre de.*
- *La majorité, la moitié, un tiers, un quart, trois quarts.*

### 6.3 Describing a figure or table
*La figure 2 montre l'évolution de… / Le tableau 3 présente… / On observe que… / Il ressort de ces données que… / Ce résultat s'explique par… / Les écarts sont significatifs (p < 0,05)…*

### 6.4 Careful claims (hedging in analysis)
| Strength | Example |
|---|---|
| **Established** | *Les résultats démontrent que…* |
| **Supported** | *Les résultats montrent / indiquent que…* |
| **Suggested** | *Les résultats suggèrent que…* |
| **Possible** | *Il est possible que…* / *Il se peut que…* (both + subjunctive) |

Use *corrélation* vs. *causalité* with care: *Une corrélation n'implique pas une relation de cause à effet.*

---

## 7. Style Rules for Technical French

1. **One idea per sentence**; aim for 15–25 words on average.
2. **Prefer the active voice** and a concrete subject: *Le serveur renvoie une erreur* rather than *Une erreur est renvoyée*. Use the passive only when the agent is unknown or irrelevant.
3. **Use the same term for the same thing.** In technical writing, repetition is a feature: do not alternate *fichier, document, donnée* for the same object.
4. **Define abbreviations** at first use: *interface de programmation (API)*.
5. **Avoid ambiguous pronouns**: if *il* could refer to two nouns, repeat the noun.
6. **Avoid metaphor and rhetorical flourishes.**
7. **Use lists** for parallel items, with parallel grammar (all infinitives, or all noun phrases).
8. **Put the important information first** (the result before the method, the action before the explanation).
9. **Use tables** for comparisons, **code blocks** for commands, **figures** with captions.
10. **Be careful with false friends in technical contexts**: *library*/*bibliothèque*, *actual*/*actuel*, *eventually*/*éventuellement*, *precise*/*précis*, *sensible*/*sensible*, *application* (to apply vs. app), *to support* vs. *prendre en charge* (to support a feature = *prendre en charge*).

### 7.1 Before / after examples
| Before | After |
|---|---|
| *Il est possible de procéder à la réalisation d'une sauvegarde des données.* | *Vous pouvez sauvegarder les données.* |
| *Les erreurs doivent être gérées par le système.* | *Le système doit gérer les erreurs.* |
| *Il faudrait faire en sorte que la requête soit validée.* | *Validez la requête.* |
| *Cet outil est très performant et facile à utiliser.* | *Cet outil traite 10 000 lignes par seconde et ne demande aucune configuration.* (if true) |

---

## 8. Anglicisms and Code-Switching in Technical Contexts

French-speaking technical communities mix English and French. It is normal to see *un push, pusher, un merge, un deploy, un sprint, un backlog, un ticket, un feedback*. The question for you is **register and audience**:

| Context | Recommendation |
|---|---|
| **Internal team chat** | follow the team's habits; mixing is normal |
| **Formal documentation / public sector / Québec** | prefer French terms where well established (*téléverser, courriel, logiciel*) |
| **Academic writing** | French terms plus the English term in parentheses at first use: *apprentissage automatique (machine learning)* |
| **International teams** | English may be the working language; ask the team |

Adapt French verbs from English with the *-er* ending when the team does (*commiter, déployer, merger*), but avoid inventing new ones in formal writing. Lesson 76 discusses the wider debate on Anglicisms; here the rule is practical: **match your audience**.

---

## 9. Common Mistakes

**Spanish speakers:**
- *Librería* → *librairie* (bookshop) instead of *bibliothèque* for code libraries.
- *Aplicar* → *appliquer* in the sense of *poser sa candidature* (*postuler*).
- *Informática* → *informatique* (the field); *un ordenador* → *un ordinateur*.
- *Realizar* → *réaliser* used where *effectuer* or *exécuter* is more natural for tasks and commands.
- Using the Spanish gerund for continuous actions in procedures; in French use the present or infinitive.
- *Datos* as masculine; *les données* is feminine.
- Using comma/period inversely in numbers.

**English speakers:**
- *Actually* → *actuellement* (currently) and *eventually* → *éventuellement* (possibly).
- Noun stacks (*database connection error message*) copied without prepositions; French needs *message d'erreur de connexion à la base de données*.
- Overusing the passive.

**Both:**
- Inconsistent terms.
- Missing spaces before units and `: ; ? !`.
- Mixing *tu* and *vous* in instructions.
- Vague quantifiers instead of data.

---

## 10. Four-Week Deep-Dive Plan

| Week | Focus | Activities |
|---|---|---|
| **1. Vocabulary map** | field terms | build a glossary of 60 terms from your field with gender, French and English forms, and the official equivalent; add 5 team-usage notes |
| **2. Procedures** | instruction writing | write a 10-step procedure (installation or workflow) in the infinitive and in the *vous* imperative; compare; choose one |
| **3. Specification and report** | structure | write 8 requirements using *doit / devrait / peut*; write a one-page report using the structure in Section 4.2 |
| **4. Data narration and review** | analysis | describe two charts in 150 words; revise your week 2 and 3 documents with the checklist; get feedback |

**Checklist (tick each):** audience defined? one term per concept? imperative/infinitive consistent? numbers and units formatted correctly? warnings marked? requirements measurable? abbreviations defined? passive voice minimized? false friends checked? read aloud for clarity?

---

## 11. Progressively Harder Practice

1. **Translate vocabulary (10 min):** give the French for *dataset, to deploy, outlier, overfitting, repository, throughput, to debug, confidence interval*.
2. **Fix the instruction:** rewrite in clear numbered steps: *Il faudrait d'abord que vous alliez dans les paramètres, ensuite il y a un onglet sécurité, et là vous devez activer l'option.*
3. **Requirement rewrite:** make this measurable: *Le site doit être rapide.*
4. **Describe a trend:** write three sentences describing a rise, a drop, and a plateau in monthly active users.
5. **README:** write a French README (150 words) for a small project of your own.
6. **Incident analysis:** write a half-page *analyse a posteriori* for a hypothetical outage.
7. **Terminology audit:** take one of your English documents and list 20 terms; decide which French terms you would use in formal vs. team contexts.

---

## 12. Mini Quiz (active recall)

1. What are the two common verb forms for written procedures, and when would you use each?
2. How do you express obligation, recommendation, and permission in a specification?
3. What is the difference between *une hausse de 5 %* and *une hausse de 5 points* ?
4. Translate: *library, dataset, byte, upload, outlier*.
5. Why is *librairie* a false friend?
6. Name three style rules for technical French.

<details>
<summary>Answers</summary>

1. The infinitive (manuals, impersonal procedures) and the imperative with *vous* (software guides, tutorials addressed to the reader). 2. *doit*, *devrait / il est recommandé de*, *peut / est autorisé à*. 3. 5 % is a relative change; 5 points is an absolute change in percentage points (e.g., from 20 % to 25 %). 4. *bibliothèque; jeu de données; octet; téléverser; valeur aberrante.* 5. It means "bookshop," not "library." 6. E.g., one idea per sentence; one term per concept; active voice; important information first; define abbreviations.

**Practice 2 (sample):** 1. Ouvrez les paramètres. 2. Cliquez sur l'onglet « Sécurité ». 3. Activez l'option demandée. **Practice 3 (sample):** *Le site doit afficher la page d'accueil en moins de deux secondes pour 95 % des requêtes.*
</details>

---

## 13. Spaced Repetition Flag

- From **Lesson 53**: merge your field glossary with this lesson's tables.
- From **Lesson 66**: reuse your meeting and negotiation phrases in minutes and reports.
- From **Lesson 76**: revisit the Anglicisms debate when choosing terms.
- From **Lesson 90**: apply the revision pipeline to your technical drafts.
- Revisit the vocabulary tables and checklist on **day 2**, **day 7**, and **day 21**.

---

## Next Up

**Lesson 92: Deep Dive 12 — Your Personal Capstone Project.** Choose and complete a real project in French (a talk, an article, a documented side project, or a community contribution) that brings together everything you've built, and design your long-term practice around it. (Prefer another deep dive from the menu in Lesson 80? Tell me its name when you say "next".)

Say "next" to continue.
