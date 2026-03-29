# XMBA 201 Macroeconomics - Final Exam Prep

A single-page study app for the UC Berkeley Haas Executive MBA macroeconomics final. Covers 9 core models with structured reviews, interactive practice, and a full exam simulator.

**Live app:** [rohitmishrajan18.github.io/macro-study](https://rohitmishrajan18.github.io/macro-study/)

## What's inside

**Topic Review** - Walk through all 9 macro models with SVG diagrams, key equations, and real-world examples before testing yourself.

**6 Practice Modes:**
- Flashcards (20 concept cards with spaced repetition)
- Lightning Quiz (60-second rapid-fire MC)
- True/False Myth Buster (15 common exam traps)
- Numerical Challenge (10 plug-and-chug problems)
- Policy Scenarios (10 real-world case applications)
- Exam Simulator (25 MC questions, 90-min timer, scored by topic)

## Topics covered

| Model | Key concepts |
|---|---|
| IS-MP | Goods market equilibrium, monetary policy rule, fiscal expansion, crowding out |
| AD-IA | Inflation-output dynamics, demand shocks, supply shocks, self-correction |
| Phillips Curve | SRPC/LRPC, NAIRU, expectations shifts, sacrifice ratio |
| Solow Growth | Steady state, convergence, Golden Rule, TFP and growth accounting |
| Monetary Policy | Transmission mechanism, Taylor Rule, ZLB, QE, forward guidance |
| Fiscal Policy | Multipliers, automatic stabilizers, crowding out, Ricardian equivalence |
| Exchange Rates | UIP, PPP, J-curve, capital flows, fixed vs floating |
| Inflation Expectations | Adaptive vs rational, anchored vs unanchored, Fisher equation |
| Open Economy | Mundell-Fleming trilemma, balance of payments, twin deficits, currency crises |

## Architecture

```
index.html          Single-file app. No build step, no dependencies.
```

The entire app is one self-contained HTML file with inline CSS and vanilla JavaScript. No frameworks, no bundler, no server required. Open the file in a browser or deploy to any static host.

**State management:** localStorage persists progress across sessions (topic accuracy, flashcard position, exam history).

**Adaptive learning:** Questions are sorted by topic weakness. The app surfaces your weakest topics first across all practice modes.

**Data structure:**
- `TOPICS` - 9 macro model identifiers and display names
- `topicReviews` - Structured content with diagrams (inline SVG) and examples per topic
- `flashcards`, `lightningQuiz`, `tfQuestions`, `numericalQs`, `policyScenarios`, `examPool` - 80+ questions across all formats
- `state` - User progress tracked in localStorage

**Study plan:** The app recommends a 4-hour structured flow: Topic Review (40 min) > Flashcards (20 min) > Lightning Quiz (25 min) > True/False (20 min) > Break > Numerical (30 min) > Policy Scenarios (30 min) > Exam Simulator (70 min).

## Running locally

Open `index.html` in any browser. That's it.

## Deployment

Hosted on GitHub Pages from the `main` branch. Any push to `main` auto-deploys.
