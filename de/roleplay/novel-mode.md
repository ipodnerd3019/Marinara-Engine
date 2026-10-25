# Novel Mode: Gemeinsam eine Geschichte schreiben

In dieser Anleitung erfährst du, wie Novel Mode in Marinara Engine funktioniert. Novel Mode macht aus einem Roleplay-Chat eine einzige fortlaufende Seite, ähnlich einem Manuskript, auf der du und die KI gemeinsam eine Geschichte schreiben. Du erfährst, wie du einen Roman beginnst, Passagen schreibst und bearbeitest, die KI lenkst und dir die Geschichte vorlesen lässt.

## Was Novel Mode ist

Novel Mode ist ein Anzeigestil für Roleplay-Chats. Die Geschichte liest sich als eine Seite statt als Chat: Es gibt keine Avatare, Namen, Zeitstempel oder Sprechblasen. Jedes Mal, wenn die KI schreibt, fügt sie der Seite eine Passage hinzu. Absätze sind wie in einem gedruckten Buch eingerückt, und die Passagen gehen nahtlos ineinander über.

Anders als in einem normalen Rollenspiel schreibt die KI auch deinen Protagonisten. Sie schreibt seine Handlungen, Dialoge und Gedanken, sodass die Geschichte weiterläuft, ohne auf deinen Zug zu warten. Du lenkst sie stattdessen: Du schreibst eigene Passagen, bearbeitest, was schon auf der Seite steht, und gibst kurze Vorgaben für die nächste Passage.

Unter der Oberfläche ist ein Roman weiterhin ein Roleplay-Chat. Lorebooks, Zusammenfassungen, Erinnerungen, Verzweigungen und Agenten funktionieren genauso wie in jedem anderen Rollenspiel.

Mit mehreren Charakteren nutzt ein Roman immer den Gruppenmodus **Merged** (zusammengeführt): Die KI schreibt alle Charaktere mit einer Stimme, wie es ein Romanautor tut, und es gibt keine Züge, die man abwechselnd nehmen müsste. In Romanen blendet **Chat Settings** (Chat-Einstellungen) die Optionen für Gruppenmodus, Antwortreihenfolge und Dialogfarben aus. Der **Scenario Override** (Szenario überschreiben) der Gruppe gilt weiterhin.

## Einen Roman beginnen

1. Leg einen neuen Roleplay-Chat an.
2. Stell im ersten Schritt des Einrichtungsassistenten **Display style** (Anzeigestil) auf **Novel** (Roman).
3. Schließ den Assistenten ab. Charaktere und eine Persona sind optional. Füge Charaktere nur hinzu, wenn ihre Karten im Kontext der Geschichte stehen sollen.

Mit **Novel** behältst du deine Agenten wie in jedem Rollenspiel. Sprites, das HUD und Wettereffekte erscheinen, wenn die Agenten dahinter eingeschaltet sind (Expression Engine, World State und die Tracker-Agenten). Entferne diese Agenten im Assistenten oder unter **Chat Settings**, wenn du eine schlichte Seite willst. Romane tragen in der Chatliste ein Buchsymbol.

**Novel** wählt außerdem **Marinara's Novel Preset** aus, das die KI anweist, deinen Protagonisten zu schreiben (siehe unten). Ein anderes Preset kannst du im Schritt **Preset** des Assistenten oder später unter **Chat Settings** wählen. Wechselst du im selben Assistenten zu einem anderen Anzeigestil zurück, kehrt dein vorheriges Preset zurück, es sei denn, du hast inzwischen ein anderes gewählt.

## Schreiben und bearbeiten

- **Eigenen Text hinzufügen:** Schreib in die Zeile am Ende der Seite, in der **Keep writing, or press Send…** (weiterschreiben oder Senden drücken) steht. Sobald du die Zeile verlässt oder **Send** (Senden) drückst, wird dein Text zur nächsten Passage der Geschichte.
- **Alles auf der Seite bearbeiten:** Die ganze Seite ist ein einziger Editor. Klick irgendwo hinein und tipp los, wie in einer Textverarbeitung. Deine Änderungen speichern sich kurz nachdem du aufhörst zu tippen von selbst, und **Ctrl+Z** macht sie rückgängig.
- **Formatierung:** Text in einer Passage kann *kursiv* oder **fett** sein. Markier ihn und drück **Ctrl+I** oder **Ctrl+B** (**Cmd** auf dem Mac). Gespeichert wird er als Markdown, also als `*italic*` und `**bold**`, und `*text*`, `_text_`, `**text**` und `__text__`, die schon in einer Passage stehen, erscheinen kursiv und fett. Jedes andere Markup, etwa Überschriften, Listen, Links und HTML, erscheint als einfacher Text und wird nicht gesondert behandelt. Zeilenumbrüche bleiben erhalten: Eine Passage, deren Absätze auf einzelnen Zeilen stehen, behält das bei, wenn du sie bearbeitest.
- **Über mehrere Passagen markieren:** Du kannst Text markieren, kopieren und löschen, der sich über mehrere Passagen erstreckt. Jede Passage bleibt dabei ein eigener Teil der Geschichte: Löschst du über mehrere hinweg, wird Text aus jeder einzelnen entfernt, nie die Passagen selbst. Leerst du eine Passage vollständig und gehst weiter, fragt Marinara, ob sie gelöscht werden soll.
- **Aktionen einer Passage:** Zeig auf eine Passage oder setz den Cursor hinein, dann erscheinen ihre Aktionen am Rand: kopieren, übersetzen, neu generieren, Lesezeichen, anheften oder Notiz, **Mark as new start** (als neuen Anfang markieren), vor der KI verbergen, verzweigen und löschen, dazu **Speak** (Vorlesen), wenn Text to Speech an ist. Die letzte Passage hat außerdem **Peek prompt** (Prompt einsehen), und eine Passage, die mit einer Vorgabe entstanden ist, hat **Stored guidance** (gespeicherte Vorgabe), das die Richtung zeigt, die ihr mitgegeben wurde. Am Telefon tippst du auf die Passage oder setzt den Cursor hinein, um die Aktionen anzuzeigen.

## Die KI um mehr bitten

Die Nachrichtenleiste unter der Seite funktioniert wie in jedem Rollenspiel, mit einem Unterschied: Was du dort eintippst, wird nie zu einer Nachricht. Es lenkt nur die nächste Passage.

- **Send** mit leerer Leiste schreibt die nächsten paar Absätze der Geschichte.
- Tipp eine kurze Richtung ein, etwa `a storm arrives` („ein Sturm zieht auf“), und drück **Send**. Die KI lenkt die nächste Passage in diese Richtung, ohne die Vorgabe selbst in die Geschichte zu schreiben.
- Slash-Befehle, Diktat und die Umschalter für Verbindung und Persona funktionieren wie gewohnt. Anhänge und die Schnellantworten **Post only** (nur posten) und **Guide reply** (Antwort leiten) gibt es hier nicht: Nichts, was du postest, wird zu einer Nachricht, und **Send** schickt deinen Text ohnehin als Vorgabe.
- Impersonate gibt es in einem Roman nicht: Du hast keinen eigenen Zug zu schreiben, weil die KI deinen Protagonisten bereits schreibt. Der Befehl `/impersonate`, die Schnellantwort Impersonate und die Impersonate-Einstellungen des Chats sind ausgeblendet.
- Ist der Agent CYOA an, lenkt die Wahl einer seiner Optionen die nächste Passage dorthin, wie eine Vorgabe. Sie wird nie zu einer Nachricht von dir, deshalb ist der Impersonate-Schalter an den Auswahlmöglichkeiten ausgeblendet. Ist **Add CYOA choices to the message box instead of sending them** (CYOA-Auswahlmöglichkeiten ins Nachrichtenfeld einfügen, statt sie abzuschicken) an, landet die Wahl stattdessen in der Nachrichtenleiste, wo du sie mit deiner eigenen Vorgabe kombinieren kannst.
- Um eine Passage neu zu schreiben, nutze in ihren Aktionen das Neugenerieren (**Regenerate**, neu generieren). Deine Änderungen werden vorher gespeichert. Ist **Guide swipes/regens with chat input** (Swipes und Neugenerierungen mit der Chat-Eingabe lenken) unter **Settings** (Einstellungen) an und steht Text in der Nachrichtenleiste, heißt die Schaltfläche **Regenerate (guided)** und lenkt die neue Fassung zu diesem Text hin, wie **Send** es tut. Sobald eine Passage mehr als eine Fassung hat, wechselst du mit den Pfeilen darunter zwischen ihnen, und eine Änderung, die du gerade getippt hast, wird in der Fassung gespeichert, in der du sie getippt hast.
- Während die KI schreibt, wird **Send** zu **Stop** (stoppen).

## Wie die KI angewiesen wird, einen Roman zu schreiben

**Marinara's Novel Preset** ist ein integriertes Preset, das für Romane geschrieben wurde. Es sagt der KI, dass sie mit dir an einem einzigen Manuskript schreibt, dass sie jeden Charakter schreibt, auch deinen Protagonisten, und dass sie Buchprosa schreibt: Absätze, Dialoge in Anführungszeichen, *Kursivschrift* nur für Gedanken und Betonung und sonst kein Markdown. Jede Passage setzt dort an, wo die Seite endet, und hört an einer natürlichen Pause auf, nie mit einer Frage an dich. Die KI folgt der Vorgabe, die du in die Nachrichtenleiste tippst, ohne sie zu zitieren oder Notizen darüber in die Passage zu schreiben.

Wer der Protagonist ist, hängt davon ab, wie du den Roman eingerichtet hast:

| Einrichtung | Protagonist | Besetzung |
| --- | --- | --- |
| Keine Persona und keine Charaktere | Der Protagonist, dem das Manuskript bereits folgt. Auf einer leeren Seite legt die KI einen fest, mit Namen, eigener Stimme und einem Ziel, und hält ihn stimmig. | Keine vorbereitete Besetzung. Die KI führt Charaktere ein, wie die Geschichte sie braucht. |
| Eine Persona und Charaktere | Deine Persona. Ihr Profil gehört zur Story-Bible, dem Nachschlagewerk der Geschichte. | Deine Charaktere, jeder seiner Karte treu. |
| Charaktere, aber keine Persona | Der Protagonist, dem das Manuskript bereits folgt. Sonst bei einem Charakter dieser Charakter, es sei denn, seine Karte beschreibt jemand anderen; dann erschafft die KI diese Person. Bei mehreren wählt die KI einen von ihnen oder einen neuen Charakter, wenn die Karten auf jemand anderen verweisen. | Deine Charaktere. |
| Eine Persona, aber keine Charaktere | Deine Persona. | Keine vorbereitete Besetzung. |

Eine Persona zählt, wenn sie eine Beschreibung oder anderen Text hat. Eine Persona mit nur einem Namen zählt als keine Persona, weil die KI ihren Namen nie sieht. Ohne Persona liest sich eine Karte, die `{{user}}` erwähnt, als „User“. Karten für einen Roman ohne Persona lesen sich deshalb am besten, wenn sie den Protagonisten beim Namen nennen oder `{{user}}` nicht erwähnen.

Das Preset stellt zu Beginn des Romans ein paar Fragen: die Altersfreigabe (**NSFW** oder **SFW**), die Erzählperspektive (dritte, erste oder zweite Person), den Erzählstil (nah am Protagonisten, an Szenenwechseln zwischen Perspektivfiguren wechselnd oder allwissend), die Zeitform, die Länge der Passagen (**Length**, Länge) und die Sprache. Die erste Option ist jeweils der Standard.

Wie Marinara's Universal Preset ist auch das Novel-Preset schreibgeschützt und lässt sich nicht löschen. Öffne es unter **Presets** und erstelle eine bearbeitbare Kopie, um seinen Wortlaut zu ändern. Es nutzt deine Verbindungs- und Chat-Generierungseinstellungen statt eigener. Siehe [Preset-Editor und Prompt-Manager](../prompts/presets.md).

Ein paar Dinge solltest du wissen:

- In Roleplay-Chats nutzt eine Verbindung mit eigenem Preset-Override stattdessen dieses Preset, auch in Romanen.
- Stellst du einen Roman später mit dem Schalter **Visual Novel display** (Visual-Novel-Anzeige) unter **Settings > Appearance** (Einstellungen > Darstellung) auf Visual Novel oder Classic um, bleibt das Novel-Preset erhalten. Wähl unter **Chat Settings** ein anderes Preset, wenn die KI deinen Protagonisten nicht mehr schreiben soll. Der Schalter ändert außerdem deinen Standard-Anzeigestil für Roleplay-Chats ohne gespeicherten Stil, nicht nur den geöffneten Roman.
- Ein anderes Preset funktioniert in einem Roman auch, aber die meisten Roleplay-Presets sagen der KI, dass sie nie deinen Charakter schreiben soll. Marinara's Universal Preset tut das, deshalb überlässt die KI deinen Protagonisten damit dir.

## Die Geschichte anhören

Ist Text to Speech an, gehört **Speak** zu den Aktionen jeder Passage. Ist **Only read dialogues** (nur Dialoge vorlesen) aus, wird auch die Erzählung vorgelesen, mit der Erzählerstimme, wenn **Use separate narrator voice** (eigene Erzählerstimme verwenden) an ist. Ist **Only read dialogues** an, wird nur der Dialog in Anführungszeichen vorgelesen.
