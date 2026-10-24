# Leksio dla Claude

Wtyczka łączy Claude z bazą prawną SIP Leksio: aktami prawnymi, orzeczeniami sądów i interpretacjami
podatkowymi z oficjalnych źródeł (Dziennik Ustaw, CBOSA, SAOS, EUREKA). Claude wyszukuje dokumenty po
problemie, sygnaturze albo oznaczeniu przepisu, czyta sentencję i uzasadnienie, sprawdza brzmienie
przepisu na wskazany dzień i podaje każde źródło z linkiem do sip.leksio.pl.

## Co zawiera

- **Konektor Leksio** (`https://mcp.leksio.pl/sip`): 11 narzędzi tylko do odczytu, logowanie kontem Leksio
  przez OAuth.
- **Umiejętność `research-prawny`**: metoda pracy ze źródłami, zasady cytowania i obsługa limitów.
- **Komendy** (umiejętności uruchamiane przez Ciebie): `/research-podatkowy`, `/przepis-na-dzien`,
  `/linia-orzecznicza`, `/sprawdz-cytaty`. Claude nie uruchamia ich sam, bo każda zużywa research.

## Wymagania

- Konto Leksio z potwierdzonym adresem e-mail i akceptacja
  [Zasad Leksio MCP](https://leksio.pl/zasady/leksio-mcp) przy pierwszym połączeniu.
- Pula researchy wynika z planu konta: darmowe 5 w miesiącu, SIP Pro 50, SIP Pro+ 150. Jeden research
  obejmuje do 50 wywołań narzędzi.
- Umiejętności działają, gdy w Claude włączone jest wykonywanie kodu (Ustawienia, Możliwości).

## Gdzie działa

Claude na stronie claude.ai, w aplikacji na komputer i telefon, w Cowork oraz w Claude Code.
W Claude Code zainstaluj wtyczkę poleceniem:

```
/plugin install leksio --marketplace andredzi/leksio-claude-plugin
```

Przy pierwszym użyciu Claude Code otworzy logowanie Leksio w przeglądarce. Ekran zgody pokaże
„Leksio MCP dla Claude Code”.

## Prywatność i zakres

Leksio nie zapisuje treści pytań. Przechowuje dostawcę, znaczniki czasu, liczniki operacji
i identyfikatory pobranych dokumentów. Umiejętność prowadzi Claude tak, by do narzędzi trafiało samo
zagadnienie prawne, bez danych osób i kontrahentów. Wyniki to materiał do analizy, nie porada prawna.
Szczegóły: [pomoc](https://leksio.pl/pomoc?temat=leksio-mcp),
[polityka prywatności](https://leksio.pl/zasady/prywatnosc).

## Licencja

Pliki wtyczki udostępniamy na licencji Apache 2.0 (`LICENSE`). Licencja nie obejmuje usługi Leksio,
bazy SIP Leksio, serwera MCP ani nazwy i logo Leksio (`NOTICE`).

---

# Leksio for Claude (English)

This plugin connects Claude to the Leksio SIP database of Polish legal acts, court judgments and tax
rulings from official sources. Claude searches by topic, case number or statutory citation, reads the
disposition and reasoning, checks the wording of a provision as at a given date and cites every source
with a link to sip.leksio.pl.

It bundles the Leksio connector (11 read-only tools, OAuth sign-in with a Leksio account), the
`research-prawny` skill with the research and citation method, and four user-invoked skills for tax research,
provision-on-date checks, case-law lines and citation verification. A verified Leksio account and
acceptance of the Leksio MCP Rules are required. Monthly research allowance: free 5, SIP Pro 50,
SIP Pro+ 150; each research includes up to 50 tool calls. Works in Claude on the web, desktop, mobile,
Cowork and Claude Code (`/plugin install leksio --marketplace andredzi/leksio-claude-plugin`). Skills require code execution to be enabled.
Leksio does not store the content of your questions; the skill keeps personal and counterparty data out of
tool calls. Results are not legal advice.

The plugin files are licensed under Apache 2.0 (`LICENSE`); the Leksio service, database, MCP
server, name and logo are not (`NOTICE`).

Operated by Leksio sp. z o.o. Support: https://leksio.pl/pomoc?temat=leksio-mcp
