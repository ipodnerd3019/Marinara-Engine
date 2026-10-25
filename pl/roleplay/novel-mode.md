# Novel Mode: wspólne pisanie historii

Ten przewodnik wyjaśnia, jak działa Novel Mode w aplikacji Marinara Engine. Novel Mode zamienia czat w trybie Roleplay w jedną ciągłą stronę, przypominającą rękopis, na której ty i AI wspólnie piszecie historię. Dowiesz się z niego, jak zacząć powieść, pisać i edytować fragmenty, kierować AI i słuchać historii.

## Czym jest Novel Mode

Novel Mode to styl wyświetlania czatów w trybie Roleplay. Historia czyta się jak jedna strona, a nie czat: nie ma awatarów, imion, znaczników czasu ani dymków wiadomości. Za każdym razem, gdy AI pisze, dodaje do strony nowy fragment. Akapity mają wcięcia jak w drukowanej książce, a fragmenty płynnie przechodzą jeden w drugi.

Inaczej niż w zwykłym roleplayu AI pisze też twojego protagonistę. Opisuje jego działania, dialogi i myśli, więc historia toczy się dalej bez czekania na twoją turę. Ty kierujesz nią w inny sposób: piszesz własne fragmenty, edytujesz to, co już jest na stronie, i dajesz krótkie wskazówki do następnego fragmentu.

Pod spodem powieść nadal jest czatem w trybie Roleplay. Lorebooki, podsumowania, wspomnienia, gałęzie i agenci działają tak samo jak w każdym roleplayu.

Przy kilku postaciach powieść zawsze korzysta z trybu grupowego **Merged** (scalone): AI pisze wszystkie postacie jednym głosem, tak jak robi to powieściopisarz, więc nie ma tur do zajmowania. W powieściach **Chat Settings** (ustawienia czatu) ukrywa opcje trybu grupowego, kolejności odpowiedzi i koloru dialogów. **Scenario Override** (nadpisanie scenariusza) grupy nadal obowiązuje.

## Rozpoczynanie powieści

1. Utwórz nowy czat w trybie Roleplay.
2. W pierwszym kroku kreatora ustaw **Display style** (styl wyświetlania) na **Novel** (powieść).
3. Dokończ kreator. Postacie i persona są opcjonalne. Dodaj postacie tylko wtedy, gdy ich karty postaci mają trafić do kontekstu historii.

Wybór **Novel** zachowuje twoich agentów, jak w każdym roleplayu. Sprite'y, pasek HUD i efekty pogodowe pojawiają się, gdy włączeni są agenci, którzy za nie odpowiadają (Expression Engine, World State i agenci trackerów). Usuń tych agentów w kreatorze albo w **Chat Settings**, jeśli chcesz mieć czystą stronę. Powieści mają na liście czatów ikonę książki.

Wybór **Novel** ustawia też **Marinara's Novel Preset**, który każe AI pisać twojego protagonistę (zobacz niżej). Inny preset możesz wybrać w kroku **Preset** kreatora albo później w **Chat Settings**. Jeśli w tym samym kreatorze wrócisz do innego stylu wyświetlania, wraca poprzedni preset, chyba że w międzyczasie wybrano inny.

## Pisanie i edytowanie

- **Dodawanie własnego tekstu:** pisz w wierszu na końcu strony, w którym widać **Keep writing, or press Send…** (pisz dalej albo naciśnij Send). Gdy opuścisz wiersz albo naciśniesz **Send** (wyślij), twój tekst staje się następnym fragmentem historii.
- **Edytowanie wszystkiego na stronie:** cała strona to jeden edytor. Kliknij w dowolnym miejscu i pisz, jak w edytorze tekstu. Zmiany zapisują się same chwilę po tym, jak przestaniesz pisać, a **Ctrl+Z** je cofa.
- **Formatowanie:** tekst we fragmencie może być *kursywą* albo **pogrubiony**. Zaznacz go i naciśnij **Ctrl+I** lub **Ctrl+B** (**Cmd** na Macu). Zapisuje się jako markdown, czyli `*italic*` i `**bold**`, a `*text*`, `_text_`, `**text**` i `__text__`, które już są we fragmencie, wyświetlają się kursywą i pogrubieniem. Każdy inny znacznik, na przykład nagłówki, listy, linki i HTML, wyświetla się jako zwykły tekst i nie jest specjalnie obsługiwany. Podziały wierszy są zachowywane: fragment, którego akapity stoją w pojedynczych wierszach, zostaje taki po edycji.
- **Zaznaczanie w wielu fragmentach:** możesz zaznaczać, kopiować i usuwać tekst obejmujący kilka fragmentów. Każdy fragment pozostaje osobną częścią historii: usuwanie przez kilka fragmentów zabiera tekst z każdego z nich, ale nigdy samych fragmentów. Jeśli całkowicie opróżnisz fragment i przejdziesz dalej, Marinara zapyta, czy go usunąć.
- **Akcje fragmentu:** wskaż fragment albo ustaw w nim kursor, a na marginesie pojawią się jego akcje: kopiowanie, tłumaczenie, ponowne generowanie, zakładka, przypięcie lub notatka, **Mark as new start** (oznacz jako nowy początek), ukrycie przed AI, gałąź i usunięcie, a przy włączonej funkcji tekstu na mowę także **Speak** (czytaj na głos). Ostatni fragment ma też **Peek prompt** (podejrzenie promptu), a fragment napisany ze wskazówką ma **Stored guidance** (zapisana wskazówka), które pokazuje kierunek, jaki mu nadano. Na telefonie dotknij fragmentu albo przenieś do niego kursor, żeby je pokazać.

## Proszenie AI o więcej

Pasek wiadomości pod stroną działa jak w każdym roleplayu, z jedną różnicą: to, co tam wpiszesz, nigdy nie staje się wiadomością. Kieruje tylko następnym fragmentem.

- **Send** przy pustym pasku dopisuje kilka kolejnych akapitów historii.
- Wpisz krótki kierunek, na przykład `a storm arrives` ("nadciąga burza"), i naciśnij **Send**. AI poprowadzi następny fragment w tę stronę, nie wpisując samej wskazówki do historii.
- Komendy slash, dyktowanie oraz przełączniki połączenia i persony działają jak zwykle. Załączniki oraz szybkie odpowiedzi **Post only** (tylko opublikuj) i **Guide reply** (pokieruj odpowiedzią) nie są dostępne: nic, co publikujesz, nie staje się wiadomością, a **Send** i tak wysyła twój tekst jako wskazówkę.
- Funkcja Impersonate nie jest dostępna w powieści: nie masz własnej tury do napisania, bo AI już pisze twojego protagonistę. Komenda `/impersonate`, szybka odpowiedź Impersonate i ustawienia Impersonate czatu są ukryte.
- Gdy agent CYOA jest włączony, wybór jednej z jego opcji kieruje następnym fragmentem w tę stronę, tak jak wskazówka. Nigdy nie staje się twoją wiadomością, dlatego przełącznik Impersonate przy wyborach jest ukryty. Gdy włączone jest **Add CYOA choices to the message box instead of sending them** (dodawanie wyborów CYOA do pola wiadomości zamiast ich wysyłania), wybór trafia do paska wiadomości, gdzie możesz połączyć go z własną wskazówką.
- Żeby napisać fragment od nowa, użyj w jego akcjach ponownego generowania (**Regenerate**). Twoje edycje zapisują się najpierw. Gdy w **Settings** (Ustawienia) włączone jest **Guide swipes/regens with chat input** (kierowanie wariantami i regeneracją tekstem z pola czatu), a w pasku wiadomości jest tekst, przycisk nazywa się **Regenerate (guided)** i kieruje nową wersję w stronę tego tekstu, tak jak **Send**. Gdy fragment ma więcej niż jedną wersję, strzałki pod nim przełączają między wersjami, a edycja, którą właśnie wpisujesz, zapisuje się w wersji, w której ją wpisano.
- Gdy AI pisze, **Send** zmienia się w **Stop** (zatrzymaj).

## Jak AI dostaje instrukcje pisania powieści

**Marinara's Novel Preset** to wbudowany preset napisany dla powieści. Mówi AI, że współtworzy z tobą jeden rękopis, że pisze każdą postać, łącznie z twoim protagonistą, i że pisze prozą książkową: akapity, dialogi w cudzysłowie, *kursywa* tylko dla myśli i podkreśleń, bez innego markdownu. Każdy fragment zaczyna się tam, gdzie kończy się strona, i zatrzymuje się w naturalnym miejscu, nigdy na pytaniu do ciebie. AI stosuje się do wskazówki wpisanej w pasku wiadomości, nie cytując jej i nie dopisując o niej uwag do fragmentu.

To, kto jest protagonistą, zależy od tego, jak skonfigurowano powieść:

| Konfiguracja | Protagonista | Obsada |
| --- | --- | --- |
| Bez persony i bez postaci | Protagonista, za którym rękopis już podąża. Na pustej stronie AI ustala go, nadając mu imię, głos i jakiś cel, i dba o jego spójność. | Brak przygotowanej obsady. AI wprowadza postacie, gdy historia ich potrzebuje. |
| Persona i postacie | Twoja persona. Jej profil należy do biblii historii. | Twoje postacie, każda wierna swojej karcie. |
| Postacie bez persony | Protagonista, za którym rękopis już podąża. W przeciwnym razie przy jednej postaci jest nią ta postać, chyba że jej karta opisuje kogoś innego – wtedy AI tworzy tę osobę. Przy kilku AI wybiera jedną z nich albo nową postać, jeśli karty wskazują na kogoś innego. | Twoje postacie. |
| Persona bez postaci | Twoja persona. | Brak przygotowanej obsady. |

Persona się liczy, gdy ma opis lub inny tekst. Persona z samym imieniem liczy się jak brak persony, bo AI nigdy nie widzi jej imienia. Bez persony karta, która wspomina `{{user}}`, czyta się jako "User", więc karty pisane do powieści bez persony działają najlepiej, gdy nazywają protagonistę po imieniu albo nie wspominają `{{user}}`.

Na początku powieści preset zadaje kilka pytań: o kategorię treści (**NSFW** lub **SFW**), punkt widzenia (trzecia, pierwsza lub druga osoba), styl narracji (blisko protagonisty, ze zmianą postaci prowadzącej przy zmianie sceny albo wszechwiedzący), czas narracji, długość fragmentu (**Length**, długość) i język. Pierwsza opcja każdego pytania jest domyślna.

Tak jak Marinara's Universal Preset, preset Novel jest tylko do odczytu i nie da się go usunąć. Otwórz go w **Presets** (presety) i utwórz edytowalną kopię, żeby zmienić jego treść. Korzysta z twoich ustawień generowania z połączenia i czatu, a nie z własnych. Zobacz [Edytor presetów i menedżer promptów](../prompts/presets.md).

Kilka rzeczy warto wiedzieć:

- W czatach w trybie Roleplay połączenie z własnym nadpisaniem presetu używa zamiast tego tamtego presetu, również w powieściach.
- Późniejsza zmiana powieści na Visual Novel lub Classic przełącznikiem **Visual Novel display** (widok Visual Novel) w **Settings > Appearance** (Ustawienia > wygląd) zachowuje preset Novel. Wybierz inny preset w **Chat Settings**, jeśli AI ma już nie pisać twojego protagonisty. Przełącznik zmienia też domyślny styl wyświetlania czatów w trybie Roleplay bez zapisanego stylu, a nie tylko otwartą powieść.
- Inny preset też działa w powieści, ale większość presetów do roleplayu każe AI nigdy nie pisać twojej postaci. Marinara's Universal Preset tak robi, więc z nim AI zostawia protagonistę tobie.

## Słuchanie historii

Gdy funkcja tekstu na mowę jest włączona, akcje każdego fragmentu obejmują **Speak**. Gdy **Only read dialogues** (czytanie tylko dialogów) jest wyłączone, czytana jest też narracja, głosem narratora, jeśli włączone jest **Use separate narrator voice** (używanie osobnego głosu narratora). Gdy **Only read dialogues** jest włączone, czytany jest tylko dialog w cudzysłowie.
