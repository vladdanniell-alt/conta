# Contor Finanțe

Aplicație web dintr-un singur fișier pentru urmărirea banilor pe luni (RON, EUR, USD, GBP) și o listă de cumpărături pe zile. Nu are nevoie de server, bază de date sau instalare.

## Fișiere

| Fișier | Rol |
| --- | --- |
| `index.html` | Aplicația completă (pagina, stilurile și scriptul) |
| `vercel.json` | Setări pentru Vercel (adrese curate, antete de bază) |
| `favicon.svg` | Iconița din tab-ul browserului |
| `.gitignore` | Fișiere pe care Git le ignoră |
| `README.md` | Acest ghid |

## Publicare pe Vercel din GitHub

1. Creează un repository nou pe GitHub și urcă toate fișierele de mai sus în rădăcina lui (**Add file → Upload files**).
2. Pe Vercel apasă **Create New → Project**, alege **GitHub** și găsește repository-ul.
3. Apasă **Import**. La **Framework Preset** alege **Other**; restul rămâne la valorile implicite.
4. Apasă **Deploy**. Primești o adresă de forma `nume-proiect.vercel.app`.

După aceea, de fiecare dată când încarci o versiune nouă a lui `index.html` în repository, Vercel republică automat.

## Unde se salvează datele

Pe Vercel datele se salvează **în browserul** de pe dispozitivul folosit (localStorage). Asta înseamnă:

- pe telefon și pe calculator vei avea date separate;
- dacă ștergi datele site-ului din browser, se pierd;
- un browser în mod privat nu păstrează datele.

Nu există o copie în cloud. Dacă ai nevoie de date comune între dispozitive, aplicația trebuie conectată la o bază de date.

## Cursuri valutare

Cursurile BNR (EUR, USD, GBP) se introduc manual în panoul „Cursuri și profil”. Aplicația nu se conectează la BNR.
