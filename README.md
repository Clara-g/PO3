# PO3 — Guide d'entraînement Power‑Of‑3 (NASDAQ futures)

Bienvenue dans le dépôt PO3. Ce repo est conçu comme un espace pédagogique et pratique pour apprendre et s'entraîner à la stratégie Power‑Of‑3 (PO3) appliquée aux futures NASDAQ (NQ / MNQ). Il contient les supports de cours, définitions, méthodes (STDV, PD arrays, OTE, CSD…), un plan pédagogique structuré et des modèles pour documenter tes exercices et backtests.

Important : ce dépôt est un support d'apprentissage — pas un conseil financier. Tu es responsable de ton trading et de la gestion du risque.

## Objectifs
- Comprendre et repérer les phases PO3 : accumulation, manipulation, distribution.
- Savoir identifier et tracer les PD arrays : FVG, iFVG, OB, BB.
- Maîtriser l'utilisation des Standard Deviations (STDV) et de l'OTE.
- S'entraîner avec TradingView (chart‑marking, Bar Replay si Pro) et backtester manuellement.
- Préparer une validation PropFirm sur compte 50 000 $ (risk par trade 0.5%).

## Contenu principal du dépôt
- `1% formation.md` — rappel synthétique du workflow PO3 et timeframes.
- `Power of 3.md` — théorie PO3, exemples.
- `PD Arrays.md` — FVG, iFVG, OB, BB expliqués.
- `Standard Deviations (STDV).md` — méthode et exemples d'utilisation.
- `Optimal Trade Entry (OTE).md` — réglages et dessins OTE.
- `change in the state of delivery (CSD).md` — CSD/CISD et utilisation pour LTF.
- `Vocabulary and terms.md` — lexique et définitions.
- `docs_trader_instructions_PO3_Version9.md` — questionnaire/specs pour formaliser règles de trading.
- `plan_pedagogique.md` — plan pédagogique (8 semaines) pour t'entraîner pas à pas.
- `input.md`, `OHLC and OLHC.md`, `PD Arrays.md` — compléments et images référencées.

## Structure recommandée (suggestion)
Crée ces dossiers dans le repo pour organiser ton travail :
- `exercises/` — captures d'écran annotées et exports TradingView par exercice.
- `backtests/` — fichiers CSV/Google Sheets du trade journal et rapports métriques.
- `pine/` — scripts Pine (v4/v5) à corriger / tester.
- `templates/` — captures des réglages TradingView (fib OTE/STDV), JSON rules, checklist.

Exemple nommage des fichiers d'exercice :
- `exercises/week1_accumulation_2026-01-12.png`
- `backtests/backtest_100_trades_2026-02.csv`
- `pine/strategy_ote_ob_stdv_v1.pine`

## Démarrage rapide
1. Lire `1% formation.md`, `Power of 3.md`, `PD Arrays.md`, `Standard Deviations (STDV).md`.
2. Ouvrir TradingView et créer un layout `PO3_NQ` (H4 / H1 / M15 / M5‑M1). Sauvegarde le template.
3. Créer et sauvegarder deux Fibonacci templates :
   - OTE : levels 0.0, 0.5, 0.618, 0.786, 1.0 (golden zone 0.618–0.786).
   - STDV : niveaux personnalisés négatifs −1.0, −2.0, −2.5, −4.0, −4.5 (et 0, 0.5).
4. Commencer le plan pédagogique dans `plan_pedagogique.md` (synchronise ton avancement en ajoutant tes captures dans `exercises/` et ton trade journal dans `backtests/`).

## Comment demander de l'aide / workflow "Corrige mon Pine"
- Pour une correction Pine : place ton script dans `pine/` puis ouvre une issue ou colle le code ici en indiquant la version Pine visée (v4 ou v5).  
- Indique précisément l'erreur rencontrée (logs) et le comportement attendu. Un exemple minimal reproductible accélère la correction.

## Trade journal — modèle
Utilise le modèle recommandé dans `plan_pedagogique.md` ou crée un CSV avec ces champs :
tradeId, date, instrument, timeframe(s), direction, entry price, entry method, SL price, TP price(s), position size, risk €, RR, outcome, pnl €, drawdown %, screenshot_url, notes, spread, slippage.

## Contribuer
- Ajoute tes exercices et captures dans `exercises/` (nommage clair).
- Propose des corrections ou améliorations de contenu via pull requests (README/Docs/Pine).
- Pour demandes spécifiques (script Pine → PR), indique la branche cible et ouvre une issue avant PR si tu veux coordination.

## Limitations & avertissement
- Les fichiers ici décrivent une méthode pédagogique et des règles basées sur le concept PO3. Ils ne garantissent pas la performance future.
- Les backtests manuels et paper trading ne reproduisent pas toujours les conditions réelles (slippage, exécution).
- Vérifie toujours les règles et T&C de la PropFirm visée avant d'engager des fonds.

## Ressources & outils recommandés
- TradingView (compte Pro recommandé pour Bar Replay / multi‑chart).
- Google Sheets / Excel pour le trade journal et les métriques.
- Broker fournissant accès NQ / MNQ (vérifier tick size et tick value pour sizing).

