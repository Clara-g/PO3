Règles de base du plan

Marché cible : NASDAQ futures (NQ / MNQ).
Timeframes selon "1% formation.md" : HTF pour bias = H1–H4 ; PO3 et structure M15 ; exécution LTF = M5–M1.
Risk management cible : 0.5% du capital par trade (sur 50k€ → 250€ max par trade).
Outils : TradingView (compte gratuit au départ ; upgrade Pro recommandé pour Bar Replay / multi‑chart / plus d’indicateurs). Je t’indique quand Pro devient utile.
Exigences de reporting : tenir un trade journal structuré (modèle fourni ci‑dessous). Vise au minimum 100 trades pour backtest initial.
Semaine 0 — Préparation & configuration (1–3 jours) Objectifs : configurer TradingView, templates, outils de marquage, et comprendre fichiers fournis. Tâches :

Créer un layout « PO3_NQ » sur TradingView (pile : H4, H1, M15, M5/M1). Sauvegarder comme template.
Apprendre où modifier un Fibonacci (clic droit → settings → Levels) et sauvegarder un Fib template pour OTE et un autre pour STDV.
Paramètres recommandés à entrer (à créer dans TradingView):
OTE Fib (pour retracement): levels visibles 0.0, 0.5, 0.618, 0.786, 1.0 ; golden zone = 0.618–0.786 (ou 62%–78.6%).
STDV Fib (déviations) : créer niveaux personnalisés négatifs : -1.0, -2.0, -2.5, -4.0, -4.5 (et 0, 0.5). Sauvegarder.
Si tu as des images de réglages (fichiers fournis), reproduis-les et prends screenshot.
Livrable semaine 0 : template TradingView avec 2 fibs sauvegardés + capture d’écran des réglages.

Semaine 1 — Théorie ciblée et reconnaissance visuelle (3–4 jours) Objectifs : connaître les définitions (PO3, OB, FVG/iFVG, BB, CSD, OTE, STDV). Tâches & exercices :

Lire et résumer (en 5–8 lignes chacun) : PO3, PD arrays, STDV et OTE (se servir des fichiers fournis). Envoie-moi tes résumés pour correction.
Exercice visuel (30 charts historiques) : sur H1 et M15, identifier et marquer 10 exemples d’accumulation, 10 de manipulation (sweep) et 10 de distribution ; prends screenshots annotés. But : apprendre à repérer la forme.
Quiz rapide : je te donne 10 extraits de chandeliers (images) et tu dis si c’est accumulation/manipulation/distribution + justification en 1 phrase (je corrige).
Livrable semaine 1 : 30 captures annotées + résumés.

Semaine 2 — PD arrays (FVG / iFVG / OB / BB) — Identification & règles (4–5 jours) Objectifs : savoir tracer et interpréter FVG, iFVG, OB, BB et leur rôle en confluence. Tâches & exercices :

Exercice 1 (marking) : sur M15/M5, trouver et marquer 15 FVG (bull & bear) et 5 iFVG ; pour chaque indiquer la zone exacte (wick→wick) et la zone cible.
Exercice 2 (OB & BB) : repérer 10 order blocks HTF (H1/H4) et 10 LTF OBs ; noter si un OB est devenu BB (candle close past OB).
Règle pratique : pour chaque marque, noter TF, date, instrument, zone coordinate (prix), et pourquoi c’est valide (template match).
Mini‑correction : envoie 5 exemples (captures) ; je corrige et explique.
Livrable semaine 2 : 30 marqueurs PD arrays + notes.

Semaine 3 — Standard Deviations (STDV) — réglages & interprétation (4–5 jours) Objectifs : maîtriser la méthode STDV (wick→body / wick→wick), comprendre zones -1 / -2 / -2.5 / -4 / -4.5. Tâches & exercices :

Configure ton Fib STDV (si pas déjà fait).
Exercice 1 : sur H1 & H4, identifie 10 manipulations (phase 2) et trace STDV de la manipulation (debut wick → body end) ; note réactions price aux zones -2/-2.5 et -4/-4.5 (retracement vs reversal).
Exercice 2 : comparaison méthode 1 et 2 (wick→body vs wick→wick) sur 6 cas ; noter quelle méthode collerait mieux et pourquoi (PD arrays présents aux zones ?).
Règle de validation : pour valider un pull STDV, vérifie présence de PD arrays (FVG/OB/BB) au -2/-2.5 et au -4/-4.5 sur un TF au moins égal ou supérieur (M15/H1).
Livrable semaine 3 : 16 captures STDV (avec annotations) + tableau résumé réactions.

Semaine 4 — OTE & CSD / Order Blocks pour entrées LTF (4–5 jours) Objectifs : maîtriser dessin OTE et entrées via CSD/OB en LTF. Tâches & exercices :

Exercice 1 : dessiner OTE (FT 0.618–0.786) sur 20 impulsions (H1→M5) ; pour chaque, noter si éventuelle entrée possible (confluence FVG/OB/CSD) et la gestion SL/TP.
Exercice 2 : pratiquer CSD sur M5 : repérer fermeture de la leg de manipulation par le corps (CISD) → box OB → attendre retracement → entrée. Faire 10 exemples.
Checklist entrée mini (voir plus bas) : appliquer à chaque trade simulé et noter accept/reject.
Livrable semaine 4 : 20 OTE/CSD captures + checklist complétées.

Semaine 5 — Replay & exécution (TradingView) (4–7 jours) Objectifs : apprendre à temporiser et exécuter entrées (imitation du live). Notes sur TradingView Free vs Pro :

Bar Replay (replay de marché) est disponible seulement sur Pro et supérieurs. C’est un outil extrêmement utile pour s’entraîner en situation réelle (timing d’entrée).
Alternatives si tu restes sur Free : navigation manuelle historique (moins fluide), ou utiliser des extraits importés + plateforme alternative avec replay. Pour un apprentissage sérieux, je recommande un essai Pro 1 mois (coût justifié) pour Bar Replay et multi‑chart.
Tâches & exercices :
Si Pro : utiliser Bar Replay sur M5/M1, simuler 20 sessions de 1–2 heures chacune, exécuter trades en réel (paper). Noter chaque trade dans trade journal.
Si Free : sélectionner périodes historiques, avancer bougie par bougie manuellement et exécuter les mêmes 20 sessions mais en qualité réduite.
Exercice de finesse : 50 entrées simulées (M1/M5) avec ordre limit vs market, mesurer remplissage et slippage.
Livrable semaine 5 : 50 trades simulés avec journal complet.

Semaine 6 — Backtest manuel & premiers KPI (1 semaine) Objectifs : apprendre à backtester manuellement et calculer metrics. Tâches & exercices :

Définir règles d’entrée (checklist), SL (sous wick de sweep / OB), TP (structure opposite / STDV / Fib ext 1.27).
Backtest manuel 100 trades (ou 3–4 semaines historiques) avec carnet (spread, slippage estimé). Remplir log : entry, SL, TP, size, RR, outcome, rationale.
Calculer métriques : winrate, avg RR, expectancy, max DD, profit factor.
KPI de validation initiale (à viser) :
Winrate cible : 40–60% (selon RR)
RR médian : ≥ 1.5
Expectancy positive : > 0 (idéal 0.2–0.5% du capital/trade)
Profit factor > 1.2
Drawdown test : < 5% sur période d’échantillonnage
Livrable semaine 6 : Backtest 100 trades + rapport métriques.

Semaine 7 — Amélioration, rules refinement & automatisation basique (1 semaine) Objectifs : stabiliser la checklist, corriger biais, préparer Pine. Tâches & exercices :

Revue des 100 trades : extraire 10 faux signaux récurrents → ajuster la checklist.
Rédiger règles machine‑readable (JSON simple) des conditions d’entrée/sortie (je peux t’aider à transformer en Pine).
Si tu veux automatiser : colle ton Pine Script (ou je t’en fournis un starter). Je corrige et je fournis un strategy() minimal pour backtest.
Livrable semaine 7 : checklist finale + JSON rules + Pine starter (optionnel).

Semaine 8 — Validation finale & préparation PropFirm (1 semaine) Objectifs : simuler conditions PropFirm et mettre en place routine journalière. Tâches :

Simulation challenge sur paper account : appliquer règles (risk 0.5%), viser objectif T (propre à la propfirm).
Préparer dossier de preuve (trade log, screenshots, métriques).
Routine journalière avant ouverture marché (HTF bias, news check, templates prêts).
Livrable semaine 8 : Simulation challenge résumée + readiness checklist.

Check‑list d’entrée (à appliquer strictement) Pré‑checks (HTF → LTF)
HTF bias (H4/H1) : aligné avec trade direction ? (OUI/NON)
Pas de news high-impact dans la fenêtre (15 min avant/après) ? (OUI/NON)
PD arrays confluents au niveau d’entrée (FVG/OB/BB) ? (OUI/NON)
STDV zones validées (si utilisées) ? (OUI/NON)
OTE retracement dans 61.8–78.6% si entrée via OTE ? (OUI/NON)
Spread acceptable (≤ ticks tolérés) ? (OUI/NON)
Entrée

Type d’ordre (limit si possible) + raison (CSD retest / FVG fill / OTE)
SL placé sous/au-dessus wick d’OB / sweep ; taille SL en ticks et en € (pour calcul sizing)
Taille position = risk 0.5% / (SL in €) → nb contrats calculés
Sortie / gestion

TP1 = 50% position à structure opposite / STDV -2 ; TP2 = 100%/remaining to next liquidity / fib ext 1.27
Trailing/shift SL : après TP1 déplacer SL to breakeven + X ticks.
Cancel trade if structure HTF change or PD arrays invalidated.
Modèle de trade‑journal (à copier dans Google Sheets / CSV) Champs recommandés :
tradeId, date, instrument, timeframe(s), direction (long/short), entry price, entry method (OTE/FVG/OB/CSD/STDV), SL price, TP price(s), position size (contracts), risk € and %, RR, outcome (win/loss), pnl €, drawdown %, screenshot_url, notes (rationale), replay_speed, spread observed, slippage observed.
Backtest manuel — méthode simple & métrique à calculer
Méthode manuelle : pour chaque trade noter entry/SL/TP, résultat, durée. Après N trades calcule :
Winrate = wins / total
Avg win, avg loss
Expectancy = (winrate * avg_win) − ((1−winrate) * avg_loss)
Profit factor = gross_profit / gross_loss
Max drawdown (peak to trough)
Objectif : après 100 trades, avoir expectancy positive et profit factor >1.2.
Pine Script — dépannage rapide (tips) Les erreurs courantes que tu as vues :
Virgules vs points : Pine exige le point décimal (ex. 0.618) et des virgules pour séparer arguments ; une virgule française (,) ne pose pas pb mais attention aux espaces invisibles.
Parenthèses non fermées, noms de variables identiques, indentation.
Lorsque tu utilises arrays de niveaux (levels), vérifie le format : pour version v4/v5 la syntaxe diffère.
Si tu veux, colle ton script ici ; je le corrige et je te fournis une version strategy() minimale pour backtester OTE/OB/STDv.
Recommandation TradingView Free vs Pro
Free : suffisant pour commencer théorie et identification visuelle, marquage manuel et backtest sur petit échantillon.
Pro (ou Pro+) : recommandé si tu veux utiliser Bar Replay, multi‑chart simultané, plus d’indicateurs sauvegardés, et une expérience de backtest plus fluide. Pour une formation intensive (replay et exécution simulée) : 1 mois d’essai Pro est un bon investissement.
Objectifs chiffrés et timeline condensée (résumé)
Durée recommandée : 8 semaines (adaptable).
Milestones : Semaine 3 = maîtrise identification PD arrays & STDV ; Semaine 5 = exécution simulée ; Semaine 6 = 100 trades backtest manuel ; Semaine 8 = readiness PropFirm simulation.
KPI minimal pour envisager challenge propfirm : expectancy > 0, RR médian ≥1.5, profit factor >1.2, drawdown contrôlé.