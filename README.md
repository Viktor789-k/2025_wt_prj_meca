# Webová aplikace
Vznikla v předmětu Webové technologie na Gymnáziu Arabská ve školním roce 2025/2026.

## Local development

Aplikace používá Python Virtual Environment, před spuštěním je potřeba vytvořit venv (pokud neexistuje):

```bash
# Linux
python3 -m venv venv

# Windows
py -3 -m venv venv
```

Dále je třeba venv aktivovat:

```bash
# [Linux]
source ./venv/bin/activate

# Windows - Bash
source ./venv/Scripts/activate

# Windows - Power shell
.\venv\Scripts\Activate.ps1
```


Je třeba ujistit se, že jsou nainstalovány všechny závislosti:

```bash
# (venv)$
pip install -r requirements.txt

# ♟️ ChessBase – Databáze šachových partií

ChessBase je webová aplikace vytvořená v Django frameworku, která slouží jako databáze šachových partií. 
Uživatelé budou moci ukládat, vyhledávat a filtrovat šachové partie podle hráčů, roku, turnaje, výsledku 
nebo otevření.

Cílem projektu je vytvořit přehledný systém pro správu šachových dat s využitím relační databáze. 
Aplikace bude obsahovat modely jako Hráč, Partie a Turnaj, mezi kterými budou definovány vztahy 
(ForeignKey a případně ManyToMany).

Součástí projektu bude:
- přehled seznamu partií
- detail partie s informacemi o hráčích a výsledku
- možnost přidávání a úprav záznamů
- filtrování a vyhledávání
- moderní responzivní design pomocí Bootstrapu

Projekt bude dále rozšířen o autentizaci uživatelů a administrátorské rozhraní.
