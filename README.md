# Reddit-Testing-Project

Projekt: Testování webové aplikace Reddit.com
Autor: Tomáš Svobodník 
Datum: 28. 02. 2026
Předmět: Testování softwaru 
Hierarchie testovacích sad a případů:
Sada 1: Horní lišta a vyhledávání (TS-RED-010)
•	TC-RED-100: Kontrola loga Reddit – návrat na Home.
•	TC-RED-101: Kontrola interakce "Najít cokoli" (aktivace pole).
•	TC-RED-102: Vyhledání existujícího subredditu (např. "r/Czech").
•	TC-RED-103: Vyhledání obecného slova (např. "gaming").
•	TC-RED-104: Vyhledání neexistujícího výrazu (kontrola hlášky "No results").
•	TC-RED-105: Smazání textu ve vyhledávání pomocí křížku.
•	TC-RED-106: Kontrola historie vyhledávání po kliknutí do pole.
•	TC-RED-107: Kontrola tlačítka "Popular" v navigaci.
•	TC-RED-108: Kontrola tlačítka "All" v navigaci.
•	TC-RED-109: Kliknutí na ikonu oznámení (Notification bell).
•	TC-RED-110: Kliknutí na ikonu chatu.
•	TC-RED-111: Kontrola tlačítka "Get App" (QR kód).
•	TC-RED-112: Kontrola tlačítka "Log In" – otevření okna.
•	TC-RED-113: Kontrola tlačítka "Advertise".
•	TC-RED-114: Rozbalení menu uživatelského profilu (vpravo nahoře).
Sada 2: Feed a interakce s příspěvky (TS-RED-020)
•	TC-RED-200: Kontrola zobrazení názvu příspěvku.
•	TC-RED-201: Hlasování „Upvote“ (změna barvy/skóre).
•	TC-RED-202: Hlasování „Downvote“.
•	TC-RED-203: Otevření sekce komentářů.
•	TC-RED-204: Tlačítko Share – zobrazení možností.
•	TC-RED-205: Tlačítko Share – kopírování odkazu (Copy Link).
•	TC-RED-206: Uložení příspěvku (Save).
•	TC-RED-207: Skrytí příspěvku (Hide).
•	TC-RED-208: Reportování příspěvku (otevření menu).
•	TC-RED-209: Přepnutí náhledu na "Card".
•	TC-RED-210: Přepnutí náhledu na "Compact".
•	TC-RED-211: Nekonečné scrollování (Infinite scroll).
•	TC-RED-212: Kontrola zobrazení autora příspěvku.
•	TC-RED-213: Proklik na jméno autora (profil).
•	TC-RED-214: Rozbalení dlouhého textu ("See more").
Sada 3: Stránka Komunity / Subredditu (TS-RED-030)
•	TC-RED-300: Zobrazení počtu členů (Members).
•	TC-RED-301: Tlačítko "Join/Leave" (ověření akce).
•	TC-RED-302: Zobrazení pravidel subredditu (Rules).
•	TC-RED-303: Filtrování podle "Flairu".
•	TC-RED-304: Řazení postů podle "Hot".
•	TC-RED-305: Řazení postů podle "New".
•	TC-RED-306: Řazení postů podle "Top".
•	TC-RED-307: Zobrazení seznamu moderátorů.
•	TC-RED-308: Kontrola názvu komunity (r/název).
•	TC-RED-309: Zobrazení online uživatelů.
•	TC-RED-310: Vyhledávání v rámci subredditu.
•	TC-RED-311: Kontrola "About Community" widgetu.
Sada 4: Sidebar a navigace (TS-RED-040)
•	TC-RED-400: Sidebar – Rozbalení/Sbalení sekce "Recent".
•	TC-RED-401: Sidebar – Kliknutí na položku v historii.
•	TC-RED-402: Sidebar – Rozbalení sekce "Communities".
•	TC-RED-403: Sidebar – Kontrola odkazu na "Home".
•	TC-RED-404: Sidebar – Kontrola odkazu na "Popular".
•	TC-RED-405: Sidebar – Tlačítko "Create Post".
•	TC-RED-406: Sidebar – Kontrola odkazu na "Resources".
•	TC-RED-407: Sbalení celého levého panelu.
Sada 5: Nastavení, UI a responzivita (TS-RED-050)
•	TC-RED-500: Přepnutí do Dark Mode.
•	TC-RED-501: Přepnutí do Light Mode.
•	TC-RED-502: Změna jazyka rozhraní.
•	TC-RED-503: Kontrola patičky (Footer) – Privacy Policy.
•	TC-RED-504: Kontrola patičky – User Agreement.
•	TC-RED-505: Responzivita – změna šířky okna.
•	TC-RED-506: Kontrola tlačítka "Back to Top".
•	TC-RED-507: Otevření nastavení oznámení.
•	TC-RED-508: Kontrola stránky "User Settings" UI.
•	TC-RED-509: Simulace 404 chyby.

Popis Testovacích sad (TS)
TS-RED-010 - Horní navigační lišta (Top Bar)
•	Stručný popis: Testovací sada se zaměřuje na funkčnost a přítomnost prvků v horní liště webu Reddit.com, která slouží k vyhledávání a přístupu k účtu. 
•	Pre-conditions:
1.	Prohlížeč: Chrome/Edge (aktuální verze).
2.	Hlavní stránka https://www.reddit.com/ je načtená.
3.	Web je v „Dark Mode“ (tmavý režim).
4.	Rozlišení monitoru: FullHD (1920x1080), Zoom 100 %.
•	Post-conditions:
o	Po každém TC pořídit screenshot pro manuální ověření (zejména interakce vyhledávacího pole).
o	Reload stránky pro návrat do výchozího stavu.
TS-RED-020 - Sidebar (Levý navigační panel)
•	Stručný popis: Testovací sada určená k ověření funkčnosti bočního menu, historie navštívených komunit (sekce NEDÁVNÉ) a odkazů na zdroje informací.
•	Pre-conditions:
1.	Uživatel se nachází na hlavní stránce.
2.	Levý panel je vysunutý (viditelný).
3.	V sekci „NEDÁVNÉ“ je historie (např. r/TeamfightTactics).
•	Post-conditions:
o	Ověření, že kliknutí na položku v sidebaru správně přesměruje uživatele.
o	Screenshot levého panelu pro kontrolu UI prvků.

Popis vybraných Testovacích případů (TC)
TC-RED-101 - Kontrola interakce "Najít cokoli"
•	Autor: Tomáš Svobodník
•	Priorita: Smoke testy (Vysoká)
•	Typ: Manuální
•	Očekávaný výsledek: Vyhledávací pole korektně přijímá vstup a po potvrzení zobrazí relevantní výsledky.
•	Pre-conditions: Uživatel vidí v horní černé liště pole s textem „Najít cokoli“.
•	Testovací kroky:
1.	Kliknout do pole „Najít cokoli“ -> Pole se aktivuje, kurzor bliká.
2.	Zadat text „r/TeamfightTactics“.
3.	Stisknout klávesu Enter.
•	Výsledek: Stránka se přesměruje na výsledky vyhledávání pro danou komunitu.
TC-RED-201 - Hlasování „Upvote“
•	Autor: Tomáš Svobodník
•	Priorita: Vysoká
•	Typ: Manuální
•	Očekávaný výsledek: Ikona šipky změní barvu na oranžovou a skóre postu se zvýší.
•	Testovací kroky:
1.	Najít první příspěvek ve feedu (např. „Hledání práce“).
2.	Kliknout na ikonu šipky nahoru (Upvote).
•	Výsledek: Ikona se zbarví oranžově, skóre u příspěvku se zvýší o 1.
TC-RED-209 - Přepnutí náhledu (Card vs. Compact)
•	Autor: Tomáš Svobodník
•	Priorita: Nízká 
•	Typ: Manuální
•	Očekávaný výsledek: Změní se hustota zobrazení příspěvků na stránce.
•	Testovací kroky:
1.	Kliknout na ikonu pro změnu zobrazení (vedle řazení „Česká Republika“).
2.	Vybrat možnost „Kompaktní zobrazení“.
•	Výsledek: Příspěvky se vizuálně smrsknou do úzkých řádků, zmizí velké náhledy obrázků.
TC-RED-400 - Přepnutí do „Dark Mode“
•	Autor: Tomáš Svobodník
•	Priorita: Střední
•	Typ: Manuální
•	Očekávaný výsledek: Celé barevné schéma webu se přepne mezi světlým a tmavým režimem.
•	Testovací kroky:
1.	Kliknout na uživatelské menu vpravo nahoře (ikona profilu).
2.	Kliknout na přepínač „Dark Mode“.
•	Výsledek: Barva pozadí a textu se okamžitě změní (např. z černé na bílou).
TC-RED-403 – Sidebar (Kontrola postranního menu)
•	Autor: Tomáš Svobodník
•	Priorita: Střední
•	Typ: Manuální
•	Očekávaný výsledek: Boční menu je plně interaktivní a obsahuje historii prohlížení.
•	Testovací kroky:
1.	Podívat se do levého panelu do sekce „NEDÁVNÉ“.
2.	Kliknout na položku „r/TeamfightTactics“.
•	Výsledek: Uživatel je okamžitě přesměrován na subreddit r/TeamfightTactics.

