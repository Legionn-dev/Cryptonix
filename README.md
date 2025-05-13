#  Cryptonix — Moderná a bezpečná aplikácia na správu hesiel

Cryptonix je aplikácia postavená na modernom frameworku **Tauri** (frontend v **HTML/CSS/JavaScript**, backend v **Rust**), ktorá umožňuje **generovať**, **analyzovať** a **bezpečne ukladať** heslá.
---

##  Hlavné funkcie

### 1. Generovanie silných hesiel
- Možnosť nastaviť dĺžku hesla
- Voliteľné komponenty: veľké písmená, čísla, špeciálne znaky
- Vygenerované heslo je ihneď dostupné na kopírovanie

### 2. Kontrola sily hesiel
- Algoritmus vyhodnotí heslo podľa dĺžky, diverzity znakov, opakovania vzorov
- Skóre bezpečnosti: slabé / priemerné / silné

###  3. Bezpečné ukladanie hesiel
- Heslá sa ukladajú lokálne na disk 
- Prístup k uloženým heslám je chránený **hlavným heslom**
- Uložené záznamy je možné v aplikácii spravovať (pridať, upraviť, vymazať)

###  4. Organizácia
- Heslá sú uložené pod názvami služieb (napr. Gmail, Discord, Binance...)

###  5. Používateľský zážitok
- Jednoduché a elegantné UI v modernom štýle
- Responzívny dizajn, vhodný pre desktop aj menšie obrazovky
---

###  Štruktúra projektu
Cryptonix/
├── src-tauri/         # Rust backend (Tauri)
│   ├── main.rs        # Hlavný súbor aplikácie
│   └── lib.rs         # Šifrovanie, ukladanie, čítanie
├── src/               # Frontend
│   ├── index.html     # UI rozhranie
│   ├── style.css      # Štýly
│   └── main.js        # JavaScript logika 
└── package.json

##  Technológie

| Vrstva           | Technológia                                                   |
|------------------|---------------------------------------------------------------|
| **Frontend**     | HTML, CSS, JavaScript                                         |
| **Backend**      | Rust (Tauri command API)                                      |
| **UI Framework** | Vanilla JS                                                    |
| **Bezpečnosť**   | šifrovanie pomocou Rust knižníc (`aes-gcm`, `argon2`, `rand`) |
| **Úložisko**     | Lokálny súbor                                                 |
| **Platforma**    | Tauri (Windows)                                               |
---

##  Inštalácia



---

###  Lokálne spustenie

```bash

git clone https://github.com/kubo-toto-si-zmen/spravca-hesiel.git
cd spravca-hesiel


npm install


npm run tauri dev
