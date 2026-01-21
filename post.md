# Samostatná práce - Poštovní zásilka (POST)

*odhadovaný čas: ~60 min. + přečtení zadání*

Vytvoříte aplikaci postavenou na frameworku [Flask](https://flask.palletsprojects.com/).

Aplikace formou webové stránky umožní uživateli vyplnit formulář pro odeslání poštovní zásilky. Data z formuláře budou validována a uložena do JSON souboru.

## Požadavky na implementaci

- Založte pro aplikaci repozitář na serveru Github, kam umístíte zdrojové kódy.
- Výchozí stránka (`/`) bude obsahovat formulář pro zadání údajů o zásilce.
- Formulář bude odesílán metodou **POST**.
- Pro vytváření HTML stránek využijte **Jinja šablony**.
- Data z formuláře budou **validována** na straně serveru.
- Validní data budou **uložena do JSON souboru** `zasilky.json`.
- Po úspěšném odeslání se uživateli zobrazí potvrzení.
- Při chybě validace se zobrazí formulář znovu s chybovými hláškami.
- Každá stránka bude validní HTML5 dokument.

## Formulářová pole

Formulář bude obsahovat následující pole:

| Pole | Typ | Povinné | Validace |
|------|-----|---------|----------|
| Jméno odesílatele | text | ano | min. 2 znaky |
| Adresa odesílatele | text | ano | min. 5 znaků |
| PSČ odesílatele | text | ano | přesně 5 číslic |
| Jméno příjemce | text | ano | min. 2 znaky |
| Adresa příjemce | text | ano | min. 5 znaků |
| PSČ příjemce | text | ano | přesně 5 číslic |
| Hmotnost zásilky (kg) | number | ano | kladné číslo |
| Typ zásilky | select | ano | balík / dopis / cenný balík |
| Pojištění | checkbox | ne | - |
| Poznámka | textarea | ne | max. 200 znaků |

