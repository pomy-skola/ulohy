# Samostatná práce - RGB2

*odhadovaný čas: ~80 min. + přečtení zadání*

Vytvoříte aplikaci postavenou na frameworku [Flask](https://flask.palletsprojects.com/).

Aplikace umožní vytvářet barevný přechod mezi zvolenými barvami.

Demo aplikace najdete na [rgb.asgard.odbornaskola.cz](https://rgb.asgard.odbornaskola.cz).


## Zadání

- Vaše aplikace by se měla chovat a vypadat podobně jako v demo ukázce.
- Podívejte se, jaké vstupy jsou uživateli k dispozici a jak se vstupy validují (jaké přijímají hodnoty, jaké hodnoty odmítají).
- Zjistěte, jak funguje historie. Nápověda: používají se cookies (session).
- Seznam barev si nechte vygenerovat (~100 barev) a uložte je do samostatného souboru.


## Požadavky na implementaci

- Založte pro aplikaci repozitář na serveru Github, kam umístíte zdrojové kódy.
- Pro vytváření HTML stránek využijte koncept [dědičnosti šablon](https://jinja.palletsprojects.com/en/stable/templates/#template-inheritance). Tzn. založíte nějakou `base` šablonu a z ní se budou odvozovat šablony ostatní.
- Rozložení stránky (umístění: formuláře, barevného gradientu, historie)
- Formulář se odesílá metodou POST.
- Aplikace (frontend) nepoužívá javascript.
- Jména barev se validují.
- Formulář si pamatuje naposledy vyplněnou hodnotu.
- Historie je svazáná s relací prohlížeče, anonymní okno je tedy nová relace.
- Každá stránka bude validní HTML5 dokument.
