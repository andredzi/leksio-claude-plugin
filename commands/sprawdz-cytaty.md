---
description: Sprawdza sygnatury, publikatory i przepisy z tekstu w bazie SIP Leksio
argument-hint: <tekst z cytowaniami do sprawdzenia>
---

Sprawdź każde cytowanie w poniższym tekście w SIP Leksio. Wyciągnij sygnatury orzeczeń, numery interpretacji, publikatory (Dz.U., M.P.) i przepisy (art., §, ust., pkt z nazwą aktu). Dla każdego wywołaj lookup_citation. Gdy dokument istnieje, porównaj datę, sąd albo organ i treść tezy z tym, co twierdzi tekst (w razie wątpliwości przeczytaj fragment przez read_document_text).
Zwróć tabelę: cytowanie | wynik (potwierdzone / brak w SIP / rozbieżne) | co się zgadza albo nie zgadza | adres SIP. Brak w SIP nie dowodzi, że dokument nie istnieje; zaznacz to. Nie poprawiaj cytowań zgadywaniem.

Zacznij od start_research z nowym requestKey i przekazuj research.id jako researchId do każdego narzędzia.

Tekst do sprawdzenia:
$ARGUMENTS
