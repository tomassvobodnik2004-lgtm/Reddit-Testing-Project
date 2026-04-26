# Reddit-Testing-Project

# Projekt: QA Testovací plán pro Reddit.com

**Autor:** Tomáš Svobodník  
**Datum:** 28. 02. 2026  
**Předmět:** Testování softwaru (FAI UTB)

---

## 📋 Hierarchie testovacích sad

### Sada 1: Horní lišta a vyhledávání (TS-RED-010)
* **TC-RED-100:** Kontrola loga Reddit – návrat na Home.
* **TC-RED-101:** Kontrola interakce "Najít cokoli" (aktivace pole).
* **TC-RED-102:** Vyhledání existujícího subredditu (např. "r/Czech").
* **TC-RED-103:** Vyhledání obecného slova (např. "gaming").
* **TC-RED-104:** Vyhledání neexistujícího výrazu (kontrola hlášky "No results").
* **TC-RED-105-114:** *Detailní kontrola prvků (historie, oznámení, chat, login atd.)*

### Sada 2: Feed a interakce s příspěvky (TS-RED-020)
* **TC-RED-200:** Kontrola zobrazení názvu příspěvku.
* **TC-RED-201:** Hlasování „Upvote“ (změna barvy/skóre).
* **TC-RED-202:** Hlasování „Downvote“.
* **TC-RED-203-214:** *Komentáře, Share, Save, Hide, nekonečné scrollování, náhledy (Card/Compact).*

### Sada 3: Stránka Komunity / Subredditu (TS-RED-030)
* **TC-RED-300-311:** Počet členů, Join/Leave, pravidla subredditu, filtrování flairů, řazení postů (Hot/New/Top).

### Sada 4: Sidebar a navigace (TS-RED-040)
* **TC-RED-400-407:** Recent sekce, Communities, Create Post, Resources, sbalení panelu.

### Sada 5: Nastavení a UI (TS-RED-050)
* **TC-RED-500-509:** Dark/Light mode, změna jazyka, responzivita, simulace 404 chyby.

---

## 🔍 Detailní popis testovacích sad (TS)

### TS-RED-010 - Horní navigační lišta
* **Popis:** Zaměřeno na funkčnost a přítomnost prvků v Top Baru.
* **Pre-conditions:** Prohlížeč Chrome/Edge, načtená home page, Dark Mode.
* **Post-conditions:** Screenshot po každém kroku, reload stránky.

### TS-RED-020 - Sidebar
* **Popis:** Ověření historie (Nedávné) a odkazů v levém panelu.
* **Pre-conditions:** Vysunutý levý panel, existující historie prohlížení.

---

## 🛠️ Ukázka konkrétních testovacích případů (TC)

### TC-RED-101: Kontrola interakce "Najít cokoli"
* **Priorita:** Smoke test (Vysoká)
* **Kroky:**
  1. Kliknout do pole „Najít cokoli“.
  2. Zadat „r/TeamfightTactics“.
  3. Enter.
* **Očekávaný výsledek:** Přesměrování na výsledky pro danou komunitu.

### TC-RED-201: Hlasování „Upvote“
* **Priorita:** Vysoká
* **Kroky:**
  1. Kliknout na šipku nahoru u příspěvku.
* **Očekávaný výsledek:** Šipka zoranžoví, skóre se zvýší o 1.

### TC-RED-500: Přepnutí do „Dark Mode“
* **Priorita:** Střední
* **Kroky:**
  1. Otevřít uživatelské menu.
  2. Přepnout „Dark Mode“.
* **Očekávaný výsledek:** Okamžitá změna barevného schématu webu.

---

> **Poznámka:** Tento projekt slouží jako podklad pro automatizaci v **Robot Frameworku**.
