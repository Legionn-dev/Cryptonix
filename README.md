#  Správca Hesiel — Moderná a bezpečná aplikácia na správu hesiel

Správca hesiel je multiplatformová aplikácia postavená na modernom stacku **Tauri** (frontend v **HTML/CSS/JavaScript**, backend v **Rust**), ktorá umožňuje **generovať**, **analyzovať silu** a **bezpečne ukladať** heslá.
---

##  Hlavné funkcie

### 1. Generovanie silných hesiel
- Možnosť nastaviť dĺžku hesla
- Voliteľné komponenty: malé a veľké písmená, čísla, špeciálne znaky
- Vygenerované heslo je ihneď dostupné na kopírovanie

### 2. Kontrola sily hesiel
- Algoritmus vyhodnotí heslo podľa dĺžky, diverzity znakov, opakovania vzorov
- Skóre bezpečnosti: slabé / priemerné / silné / veľmi silné
- Odporúčania na zlepšenie slabého hesla

###  3. Bezpečné ukladanie hesiel
- Heslá sa ukladajú lokálne na disk 
- Prístup k uloženým heslám je chránený **hlavným heslom**
- Uložené záznamy je možné spravovať (pridať, upraviť, vymazať)

###  4. Organizácia
- Heslá sú uložené pod názvami služieb (napr. Gmail, Discord, Binance...)
- Možnosť triediť, filtrovať a vyhľadávať
- Zálohovanie/export a import hesiel 

###  5. Používateľský zážitok
- Jednoduché a elegantné UI v modernom štýle (svetlý a tmavý režim)
- Responzívny dizajn, vhodný pre desktop aj menšie obrazovky

---


###  Štruktúra projektu
spravca-hesiel/
├── src-tauri/         # Rust backend (Tauri)
│   ├── main.rs        # Hlavný súbor aplikácie
│   └── utils.rs       # Šifrovanie, ukladanie, čítanie
├── src/               # Frontend
│   ├── index.html     # UI rozhranie
│   ├── style.css      # Štýly
│   └── main.js        # JavaScript logika 
├── README.md
└── package.json


##  Technológie

| Vrstva        | Technológia           |
|---------------|------------------------|
| **Frontend**  | HTML, CSS, JavaScript |
| **Backend**   | Rust (Tauri command API) |
| **UI Framework** | Vanilla JS / Svelte / Vue / React |
| **Bezpečnosť** | šifrovanie pomocou Rust knižníc (`aes-gcm`, `argon2`, `rand`) |
| **Úložisko**  | Lokálny súbor |
| **Platforma** | Tauri (cross-platform: Windows, macOS, Linux) |

---

##  Inštalácia

###  Predpoklady
- [Node.js](https://nodejs.org/)
- [Rust](https://www.rust-lang.org/)
- [Tauri CLI](https://tauri.app/v1/guides/getting-started/prerequisites)

---

###  Lokálne spustenie

```bash

git clone https://github.com/kubo-toto-si-zmen/spravca-hesiel.git
cd spravca-hesiel


npm install


npm run tauri dev
