# Samostatná práce - Whish list (GET, POST)

*odhadovaný čas: ~180 min.*

Vytvoříte aplikaci postavenou na frameworku [Flask](https://flask.palletsprojects.com/).

Aplikace formou webové stránky umožní uživateli si spravovat svůj "wish list".

## Požadavky na implementaci

Struktura položky jednoho přání

```plain
Wish
├── title
├── description
├── category          (material / experience / travel / other)
├── status            (open / partially funded / fulfilled)
├── priority          (1–5)
├── image_url
├── link_url
├── timeframe         (optional)
├── date_added
```

- Nebudeme používat žádný databázový backend.
- Data se budou ukládat do JSON souboru. Pro název použijte login uživatele - omezte znaky, které může login (a tedy i název souboru) obsahovat - jaké to budou znaky?
- Výpis seznamu bude v HTML tabulce. Tabulka bude obsahovat všechna pole přání, a navíc i odkaz na detail.
- Detail přání bude na samostatné stránce (s vlastní URL).
- Editace a mazání přání budou mít rovněž svou stránku (URL).
- Nebudeme nyní řešit více uživatelů. Tzn. login a password pro daného uživatele bude formou hashe buď někde v souboru, a nebo zadrátované přímo v kódu, a nebo součástí ENV.

## Workflow

- Aby bylo možné spravovat svá přání, je nezbytné se přihlásit.
- Uživatel si může po přihlášení přidávat nebo odebírat položky ze svého seznamu přání.
- Aplikace nabídne procházení seznamu přání, zobrazovat detaily, vyhledávat (v polích `title` a `description`), filtrovat a řadit podle `category`, `status` a `priority`.
