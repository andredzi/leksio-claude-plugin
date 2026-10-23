---
description: Research podatkowy w SIP Leksio - przepisy, interpretacje i orzeczenia ze źródłami
argument-hint: <pytanie podatkowe> [stan faktyczny, podatki, dzień stanu prawnego]
---

Przeprowadź research podatkowy w SIP Leksio i odpowiedz na pytanie użytkownika:

$ARGUMENTS

Jeśli użytkownik podał stan faktyczny, podatki (np. CIT, VAT) albo dzień stanu prawnego, uwzględnij je. Brzmienie przepisów na podany dzień sprawdź przez get_act_wording z tą datą. Bez daty:
Stan prawny: bieżący (zaznacz, jeśli przepis zmienił się w ostatnich latach).
Kroki: 1) ustal przepisy (lookup_citation albo search_legal z kinds: ["act"]); 2) sprawdź brzmienie na dzień (get_act_wording); 3) zbierz interpretacje KIS i orzeczenia sądów administracyjnych, zaczynając od 5-8 wyników CBOSA/EUREKA i sprawdzając też stanowiska przeciwne; 4) przeczytaj read_document_text z section: disposition, potem authority_reasoning lub court_reasoning i potrzebne facts. Gdy podział jest niepewny albo niepełny, czytaj all. Nie utożsamiaj stanowiska wnioskodawcy z oceną organu. Jeśli organ je zaakceptował i odstąpił od uzasadnienia, przeczytaj również applicant_position i wskaż oba fragmenty; 5) odpowiedz: wniosek, podstawa prawna, linia interpretacyjna i orzecznicza z datami, rozbieżności, ryzyka. Każdy cytat podaj z sygnaturą, datą, organem i linkiem url/sipUrl na sip.leksio.pl. Nie wymyślaj sygnatur.

Zacznij od start_research z nowym requestKey i przekazuj research.id jako researchId do każdego narzędzia.
