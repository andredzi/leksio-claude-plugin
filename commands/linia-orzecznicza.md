---
description: Linia orzecznicza w kwestii prawnej - stanowiska sądów, rozbieżności i chronologia
argument-hint: <kwestia prawna> [przepis, sądy, rok początkowy]
---

Opracuj linię orzeczniczą w kwestii wskazanej przez użytkownika:

$ARGUMENTS

Jeśli użytkownik podał przepis, użyj lookup_citation, potem get_provision_materials z category: "judgments". Sądy przekaż filtrem issuingBodyCodes albo courtIds w search_legal, rok początkowy filtrem issuedFrom.
Kroki: 1) search_legal z kinds: ["judgment"], sortowanie newest, kilka stron; 2) przeczytaj uzasadnienia kluczowych orzeczeń (read_document_text), zwłaszcza NSA i uchwał; 3) pogrupuj stanowiska, podaj chronologię, wskaż orzeczenia odmienne i to, czy linia jest ugruntowana; 4) zaznacz, które wyroki WSA mogą być nieprawomocne. Każde orzeczenie: sąd, data, sygnatura, adres SIP. Tezy AI oznaczaj jako opracowanie AI.

Zacznij od start_research z nowym requestKey i przekazuj research.id jako researchId do każdego narzędzia.
