Folgendes ist bloß eine (überprüfte) Übersetzung des original Herstellers dieses Decks.Dies steht auf der Original englischen Kaishi Seite,es sind jedoch immernoch nützliche Infos drinnen,auch für die deutsche Version,daher lohnt es sich es zu lesen.

**ALLE ANDEREN, AUF DIESER SEITE NICHT ERWÄHNTEN KARTENDECKS STEHEN IN KEINER VERBINDUNG ZU MIR, EINSCHLIESSLICH KI-GEMÄSSIGER ODER BEZAHLTER MODIFIKATIONEN.**

# Kaishi 1.5k

Willkommen im öffentlichen Repository für **Kaishi 1.5k**, einem modernen Anki-Kartenstapel, der Anfängern den japanischen Grundwortschatz näherbringt. Kaishi 1.5k ist hochgradig modular aufgebaut, und auf dieser Seite werden verschiedene Optionen erklärt, mit denen Sie den Stapel an Ihre Bedürfnisse anpassen können. So sieht die Vorderseite des Stapels aus:

<img src="https://github.com/donkuri/Kaishi/blob/main/pics/kaishi-front.png" alt="Front of a Card in Kaishi 1.5k" style="width: 100%; height: auto">

Wie Sie sehen, sind sowohl das Wort als auch die Sätze vorhanden, wobei das Wort im Satz hervorgehoben ist, sodass die wichtigen Informationen sofort erkennbar sind. Sobald man das Wort gut kennt, geht das Wiederholen schneller, da das Wort zuerst erscheint. Hier ist die Rückseite des Standardkartensatzes:

<img src="https://github.com/donkuri/Kaishi/blob/main/pics/kaishi-back.png" alt="Back of a Card in Kaishi 1.5k" style="width: 100%; height: auto">

Anders als bei den meisten anderen Core-Decks geben hier Furigana die Leseweise des Wortes an, die Bedeutung steht direkt darunter. Anschließend können Sie sich das Wort und den dazugehörigen Satz anhören. Optional können Sie auch den Tonhöhenakzent  hinzufügen (siehe unten). Falls es Anmerkungen/Notizen zu der jeweiligen Karte gibt, werden diese ebenfalls unten angezeigt.


[Wenn Sie neu anfangen Japanisch zu lernen,lesen sie bitte folgende Guide.](https://donkuri.github.io/learn-japanese/guide/)

### Inhaltsverzeichnis

- [Wo kriege ich das Deck?](#where-do-i-get-the-deck)
- [Wie benutz ich das Deck?](#how-do-i-use-this-deck)
- [Andere verwandte Decks](#other-related-decks)
- [Welche Optionen stehen für das Deck zur Verfügung?](#what-options-are-available-for-the-deck)
- [Mir gefallen die Bilder nicht!](#i-dont-like-the-images)
- [Mir gefällt es nicht, dass die Sätze immer angezeigt werden!](#i-dont-like-having-sentences-always-on)
- [Die Audioausgabe für dieses Wort ist falsch!](#the-audio-for-this-word-is-wrong)
- [Wie importiere ich Kaishi auf ein anderes Deck?](#how-to-import-kaishi-on-top-of-another-deck)
- [Die Entstehungsgeschichte des Decks](#the-genesis-of-the-deck)
- [Übersetzung des Decks](#translation-of-the-deck)
- [Was mach ich nach diesem Deck?](#what-do-i-do-after-this-deck)
- [Credits](#credits)

## Wo finde ich das Deck?

Du findest das Deck entweder auf der [Releases](https://github.com/donkuri/Kaishi/releases/) Seite dieses GitHub-Repositorys oder auf [AnkiWeb](https://ankiweb.net/shared/info/1196762551), sofern es sich nicht in der Überarbeitung befindet. **Das Deck wird von Anki 2.1.50 und höher unterstützt.**

## Wie verwende ich dieses Deck?

Eine Erklärung, wie Kaishi in das Japanischlernen allgemein integriert ist, findest du im [Leitfaden](https://donkuri.github.io/learn-japanese/guide/).

## Weitere verwandte Decks

ねむい hat ein Radikal-Deck basierend auf Kaishi 1.5k erstellt. Jedes darin enthaltene Kanji-Radikal ist mit dem ersten Wort in Kaishi verknüpft, das dieses Radikal enthält. Es umfasst außerdem einige weitere Radikale, die nicht direkt in Kaishi vorkommen. Du kannst dieses Deck **parallel zu Kaishi verwenden, wenn du Schwierigkeiten mit Kanji hast**, da es die Kanji-Radikale nach und nach einführt und dir so hilft, sie effizienter zu verstehen. Du findest das Deck [hier auf AnkiWeb](https://ankiweb.net/shared/info/1722008986). Vielen Dank!

## Welche Optionen bietet das Deck?

Es gibt verschiedene Möglichkeiten, deine Karten anzupassen. Wähle dazu das Kaishi-Deck aus, klicke auf „Kartenverwaltung“, wähle eine beliebige Karte aus dem Deck und klicke oben rechts auf „Karten…“.

### Tonhöhenakzent

Die wichtigste Option ist, ob du Tonhöhenakzente auf deinen Karten verwenden möchtest. Aktuell wird in der Community oft darüber diskutiert, ob man Tonhöhenakzente lernen sollte oder nicht. Wir haben uns für einen Mittelweg entschieden: Die Daten zum Tonhöhenakzent sind vorhanden, du entscheidest, ob du sie verwenden möchtest. Wenn Sie die Tonhöhenakzente nicht verwenden möchten, können Sie sie jederzeit später aktivieren. Die Aktivierung ist ganz einfach. Hier finden Sie die Kartenoptionen unter „Vorlage für Rückseite“ für das Kartenset (klicken Sie auf den kleinen Punkt über der Suchleiste).


```CSS
<div lang="ja">
{{furigana:Word Furigana}}

<!-- This part enables pitch accent.

{{#Pitch Accent}}
	<br><div style='font-size: 24px'>{{Pitch Accent}}</div>
{{/Pitch Accent}} 

-->

<div style='font-size: 25px; padding-bottom:20px'>{{Word Meaning}}</div>
<div style='font-size: 25px;'>{{furigana:Sentence Furigana}}</div>
<div style='font-size: 25px; padding-bottom:10px'>{{Sentence Meaning}}</div>

{{Word Audio}}
{{Sentence Audio}}
<br>
{{Picture}}

{{#Notes}}
	<br>
	<div style="font-size: 20px; padding-top:12px">Note: {{Notes}}</div>
{{/Notes}}

<!-- This part enables pitch accent notes.

{{#Pitch Accent Notes}}
<div style="font-size: 20px; width: fit-content; max-width:40vw; margin: auto">
	<details><summary>Pitch Accent Notes</summary>
		<br>{{Pitch Accent Notes}}
	</details>
</div>
{{/Pitch Accent Notes}}

-->

</div>
```

Um die Tonhöhenakzente zu aktivieren, müssen Sie lediglich alle `<!--` und `-->` Teile entfernen, die Kommentare darstellen, wie folgt:


```CSS
<div lang="ja">
{{furigana:Word Furigana}}

{{#Pitch Accent}}
	<br><div style='font-size: 24px'>{{Pitch Accent}}</div>
{{/Pitch Accent}} 

<div style='font-size: 25px; padding-bottom:20px'>{{Word Meaning}}</div>
<div style='font-size: 25px;'>{{furigana:Sentence Furigana}}</div>
<div style='font-size: 25px; padding-bottom:10px'>{{Sentence Meaning}}</div>

{{Word Audio}}
{{Sentence Audio}}
<br>
{{Picture}}

{{#Notes}}
	<br>
	<div style="font-size: 20px; padding-top:12px">Note: {{Notes}}</div>
{{/Notes}}

{{#Pitch Accent Notes}}
<div style="font-size: 20px; width: fit-content; max-width:40vw; margin: auto">
	<details><summary>Pitch Accent Notes</summary>
		<br>{{Pitch Accent Notes}}
	</details>
</div>
{{/Pitch Accent Notes}}

</div>
```

**Um zu sehen, wie die Notation von Tonhöhenakzenten funktioniert, schauen Sie sich bitte [dieses Problem](https://github.com/donkuri/Kaishi/issues/104#issuecomment-3171889366) an.**

### Kleinere Optionen

Es gibt einige kleinere Optionen, die Sie anpassen können.

#### Furigana
Wenn Sie die Furigana entfernen möchten, löschen Sie einfach die Abschnitte „furigana:“ aus der Rückseitenvorlage.

#### Weitere Kartenoptionen

Sie können die Art der Karten, die Sie sehen möchten, komplett ändern. Hier ist die Vorderseitenvorlage von Kaishi 1.5k:


```CSS
<div lang="ja">
{{Word}}
<div style='font-size: 20px;'>{{Sentence}}</div>
</div>
```

Wie Sie sehen, haben wir nur das Wort und den Satz. Wenn Sie *Satz*-Karten wünschen, entfernen Sie einfach den Teil `{{Word}}` oder fügen Sie stattdessen `{{Sentence}}` ein und entfernen Sie den Rest. Wenn Sie *Wort*-Karten wünschen, entfernen Sie einfach den Teil `<div style='font-size: 20px;'>{{Sentence}}</div>`. Wenn Sie stattdessen *Audio*-Karten wünschen, entfernen Sie alles und fügen Sie `{{Word Audio}}`, `{{Sentence Audio}}` oder beides hinzu, falls Sie beides möchten.

#### Schriftarten, Schriftgröße oder andere Formatierungsoptionen ändern

Hier ist die „Stil“  Vorlage von Kaishi 1.5k:

```CSS
.card {
 font-family: "ヒラギノ角ゴ Pro W3", "Hiragino Kaku Gothic Pro", "Noto Sans JP", Osaka, "メイリオ", Meiryo, "ＭＳ Ｐゴシック", "MS PGothic", "MS UI Gothic", sans-serif;
 font-size: 44px;
 text-align: center;
}

img {
max-width: 300px;
max-height: 250px;
}

.mobile img {
max-width: 50vw;
}

/* This part defines the bold color. */
b{color: #5586cd}
```
Die verschiedenen Stylingoptionen finden Sie [hier](https://docs.ankiweb.net/templates/styling.html). Wie Sie sehen, bietet Kaishi 1.5k im Stil-Tab nur wenige Optionen. Mit `font-family` können Sie verschiedene Schriftarten auswählen, mit `font-size` die Schriftgröße ändern und mit `text-align` die Textausrichtung anpassen, beispielsweise linksbündig. Standardmäßig werden **fette** Wörter in Kaishi 1.5k farbig dargestellt. Die Option zum Ändern dieser Darstellung ist `b{color: }`, wie oben gezeigt. Geben Sie einfach einen Hexadezimalcode oder einen Farbnamen wie `red` ein, um die gewünschte Farbe zu erhalten. Wenn Sie keine Farbe wünschen, entfernen Sie einfach den gesamten Teil `b{color: }`.

## Ich mag es nicht, wenn Sätze immer angezeigt werden!

Manche Nutzer möchten den Satz nicht immer im Vordergrund sehen. Das ist völlig verständlich, da manche Nutzer sich dann  nur die Sätze merken. Der Grund das es diese Sätze gibt,ist um den Lernern Kontext zu geben, da Bedeutung immer vom Kontext abhängt. Falls gewünscht, können Sie Ihre Vorlage für die Vorderseite der Karte und die Stil-Vorlage gemäß [dem Kommentar zu diesem Problem](https://github.com/donkuri/kaishi/issues/131#issuecomment-3968847411) anpassen, um die Wörter zu verwischen. Vielen Dank an [Hit2Skill](https://github.com/Hit2Skill) für den Tipp!

## Die Audio für dieses Wortes ist falsch!

Bestimmte Wörter wie 次 (つぎ) und あげる wurden als falsch ausgesprochen gemeldet. Dies liegt daran, dass Anfänger die japanische Nasalierung oft nicht wahrnehmen (und sich ihrer nicht bewusst sind), bei der /g/-Laute ähnlich wie /n/ klingen können. Eine Erklärung dazu finden Sie in [diesem Video](https://www.youtube.com/watch?v=xpzpbuFHVVU). **Leider ist eine bessere Audioqualität in Form von nicht-nasalierten Versionen dieser Wörter oft nicht direkt verfügbar.**

## So importieren Sie Kaishi in ein anderes Deck

Wenn Sie bereits mit Core2k oder Tango N4-N5 (oder einem ähnlichen Deck) arbeiten und zu Kaishi 1.5k wechseln möchten, folgen Sie diesen Schritten von [Kuuube](https://github.com/Kuuuube).

1. Importieren Sie Kaishi wie gewohnt mit der .apkg-Datei.

2. Gehen Sie zu „Datei > Exportieren“ und exportieren Sie das Kaishi-Deck als „Notizen als einfache Textdatei (.txt)“. Belassen Sie alle anderen Einstellungen auf den Standardwerten.

3. Löschen Sie das Kaishi-Deck.

4. Wählen Sie das Deck aus, in das Sie Kaishi importieren möchten, klicken Sie auf „Kartenverwaltung“, dann auf eine beliebige Karte, drücken Sie „Strg + A“ und wählen Sie im Menü oben links „Notozen > Notiztyp ändern…“. Stellen Sie sicher, dass alle ausgewählten Notizen vom gleichen Notizentyp sind, da „Notizen > Notizntyp ändern…“ sonst möglicherweise nicht angezeigt wird.

5. Wechseln Sie zum Notiztyp „Kaishi 1.5k“. Stellen Sie sicher, dass im Feld „Word“ in der Spalte „New“ das Feld angezeigt wird, das Ihr Kartenstapel für das danebenstehende Wort verwendet.

Wenn Sie keine Karten aus Ihrem aktuellen Kartenstapel löschen möchten, die nicht in Kaishi enthalten sind, überprüfen Sie, ob auch die anderen Felder korrekt ausgerichtet sind. Andernfalls können Sie die Standardeinstellungen verwenden und auf „Speichern“ klicken.

6. Importieren Sie die in Schritt 2 exportierte Kaishi-Textdatei.

7. Stellen Sie beim Importieren sicher, dass der Notiztyp auf „Kaishi 1.5k“ und der Kartenstapel auf den gewünschten Zielstapel eingestellt ist.

Wenn Sie Karten löschen möchten, die nicht in Kaishi enthalten sind, fügen Sie das Schlagwort „Kaishi“ unter „Schlagwörter hinzufügen“ hinzu.

8. Klicken Sie auf „Importieren“.

9. Um Karten zu löschen, die nicht in Kaishi enthalten sind, wählen Sie Ihr Deck aus, klicken Sie auf „Kartenverwaltung“, wählen Sie Ihr Deck im linken Menü aus, fügen Sie `-tag:Kaishi` in die Suchleiste ein, wählen Sie eine beliebige Karte aus, drücken Sie `Strg + A` und gehen Sie im Menü oben links zu „Notizen > Löschen“.

**Wenn Sie Daten auf Basis von Core 2.3k importieren, lesen Sie bitte [diesen Link](https://github.com/Manhhao/anki.transfer-review-history).**

## Mir gefallen die Bilder nicht!

Das ist verständlich. 1500 einheitliche und kostenlose Bilder für das Deck zu finden, war eine enorme Herausforderung (vielen Dank dafür, [liarbeast](https://github.com/liarbeast)!). Daher passen einige Bilder nicht perfekt zum Satz oder Wort. Das ist berechtigte Kritik. Wenn Sie das Bild entfernen möchten, gehen Sie wie folgt vor. Klicken Sie in der Kartenverwaltung  auf eine Kaishi-Karte und drücken sie auf "Karten...". Suchen Sie nach der Vorlage der Rückseite . Darin finden Sie „{{Picture}}“. Entfernen Sie einfach diesen Text. Alternativ können Sie den gesamten Inhalt durch Folgendes ersetzen:


```html
<div lang="ja">
{{furigana:Word Furigana}}

<!-- This part enables pitch accent.

{{#Pitch Accent}}
	<br><div style='font-size: 24px'>{{Pitch Accent}}</div>
{{/Pitch Accent}} 

-->

<div style='font-size: 25px; padding-bottom:20px'>{{Word Meaning}}</div>
<div style='font-size: 25px;'>{{furigana:Sentence Furigana}}</div>
<div style='font-size: 25px; padding-bottom:10px'>{{Sentence Meaning}}</div>

{{Word Audio}}
{{Sentence Audio}}
<br>

{{#Notes}}
	<br>
	<div style="font-size: 20px; padding-top:12px">Note: {{Notes}}</div>
{{/Notes}}

<!-- This part enables pitch accent notes.

{{#Pitch Accent Notes}}
<div style="font-size: 20px; width: fit-content; max-width:40vw; margin: auto">
	<details><summary>Pitch Accent Notes</summary>
		<br>{{Pitch Accent Notes}}
	</details>
</div>
{{/Pitch Accent Notes}}

-->

</div>
```

## Die Entstehung des Decks

Dieses Deck entstand aus einer Diskussion zwischen Tyogin und mir auf dem [TMW-Discord-Server](https://learnjapanese.moe/join/). Wir beklagten uns beide darüber, dass die damals beliebten Anfängerdecks viele ärgerliche Mängel aufwiesen. Anfänger waren bei der Verwendung von Core 2k und Tango aufgrund verschiedener Probleme immer wieder verwirrt. Tango enthielt einige obskure Wörter wie ナンプラー (eine thailändische Fischsauce), und viele waren nicht wirklich daran interessiert, dass die vielen Grundphrasen und Ländernamen einen so großen Teil des Decks einnahmen. Die Felder des Decks waren schlecht formatiert, was es unmöglich machte, das Deck anders als ursprünglich vorgesehen – nämlich als Satzkarten – zu verwenden. Core 2k hingegen war modular aufgebaut, wies aber zahlreiche Übersetzungsfehler, fehlende oder unpassende Bilder auf, und einige der Sätze waren wenig hilfreich und spiegelten teilweise nicht einmal die Bedeutung des verwendeten Wortes wider.


Beide Probleme waren so ärgerlich, dass uns alle zwei Wochen Anfänger danach fragten. Tyogin schlug vor, das Problem selbst zu beheben, und ein kleines Team wurde zusammengestellt. Wir verwendeten hauptsächlich Daten aus Core2k, Core10k, Tango N4 und Tango N5. Anschließend kombinierten wir die Daten, sortierten die Wörter mithilfe verschiedener Yomichan/Yomitan-Frequenzwörterbücher nach Häufigkeit und wählten etwa 1500 Wörter aus. Wir korrigierten dann die Übersetzungen jedes Wortes, wählten den besten Satz für jedes Wort aus und korrigierten diesen gegebenenfalls. Von den 1500 ausgewählten Sätzen mussten wir etwa 120 korrigieren. Danach bezogen wir die Tonhöhenakzentdaten und die Audioaufnahmen für Wörter, denen die korrekte Audioaufnahme fehlte, von [AJT Japanese](https://ankiweb.net/shared/info/1344485230). Ein zweiköpfiges Team (Karifurai und cindsa) überprüfte die Tonhöhenakzentdaten und fügte bei Bedarf Tonhöhenanmerkungen hinzu. Wir haben anschließend die Stille in den Audiodateien entfernt und den Audiopegel zwischen den verschiedenen Dateien angeglichen. Zusätzlich haben wir Furigana aus AJT Japanese für die Wörter und Sätze erstellt. Danach haben wir ein einfaches CSS für Hinweiskarten mit gezielten Sätzen entworfen, das in der Standardversion des Decks verwendet wird. Abschließend haben mehrere Personen das Deck Korrektur gelesen, um möglichst wenige Fehler zu vermeiden.

Kaishi (開始) bedeutet „Anfang“. Wir fanden diesen Namen passend und haben uns deshalb dafür entschieden. Wir hoffen, dass dieses Deck Ihnen einen wunderbaren Einstieg ins Japanischlernen ermöglicht.


## What do I do after this deck?

[Mit "mining" anfangen ](https://donkuri.github.io/learn-japanese/guide/#consuming-native-content) . Siehe  [hier](https://github.com/donkuri/japanese-resources/?tab=readme-ov-file#mining) für eine Liste von Mining Notiztypen.



## Übersetzung des Kartensets

Wenn Sie daran interessiert sind, das Kartenset in Ihre Muttersprache zu übersetzen, erstellen Sie bitte ein Issue im [GitHub-Tracker](https://github.com/donkuri/Kaishi/issues). Das Deck wurde bereits in folgende Sprachen übersetzt: **[Russisch](https://github.com/NeonGooRoo/KaishiRu)**, **[Indonesisch](https://ankiweb.net/shared/info/1512066033)**, **[Vietnamesisch](https://github.com/duy103zxc/kaishi-vi/releases)**, **[Ukrainisch](https://github.com/maksiksq/KaishiUa)**, **[Brasilianisches Portugiesisch](https://github.com/nonsolvent/Kaishi-pt-BR)**, **[Spanisch](https://github.com/Dogi5/Kaishi-ESP)**, **[Mandarin](https://github.com/maimemo/kaishi-zh-cn/)** und **[Französisch](https://github.com/khmskhmskhms/kaishi-FR)**. und **[Arabisch](https://github.com/kaihouguide/kaishi-arabic)**.


## Danksagung

Dieses Kartenset wurde mit der Hilfe folgender Personen erstellt:

[栗](https://github.com/donkuri/) – Hauptarchitektur, alle technischen Aspekte, Übersetzungen, Korrekturlesen

Tyogin – Hauptarchitektur, die ersten 200 Karten neu angeordnet, Sätze geändert, Korrekturlesen

shoui – Korrekturlesen des gesamten Kartensets, Übersetzungen korrigiert

Julian – Hilfe beim Hinzufügen von Anmerkungen und Überprüfung einiger Satzübersetzungen

karifurai – Überprüfung der Tonhöhenakzente für die ersten 750 Karten und Hinzufügen von Tonhöhenhinweisen

cindsa – Überprüfung der Tonhöhenakzente für die letzten 750 Karten und Hinzufügen von Tonhöhenhinweisen

[Kuuube](https://github.com/Kuuuube) – Vorschlag zur Verwendung von FFmpeg, verfasste den Abschnitt zum Übertragen der Karten nach Kaishi 1.5k (siehe oben)

[stephenmk](https://github.com/stephenmk) – Anwendung des Jmdict-Furigana-Tools auf Kaishi 1.5k zur Korrektur der Furigana (siehe oben) Version 1.3.0

[Kaanium](https://github.com/kaanium) – Mitarbeit an einem Skript zur Umwandlung des Decks in die Schreibversion

[Lars](https://github.com/liarbeast) – Hinzufügung von Bildern von [irasutoya](https://www.irasutoya.com/)

Folgende Tools wurden bei der Erstellung des Decks verwendet:

[AJT Japanese](https://github.com/Ajatt-Tools/Japanese) – Tonhöhenakzent, Furigana und Teile des Audiomaterials wurden mit diesem Add-on generiert

[FFmpeg](https://ffmpeg.org/) – Entfernung von Stillepassagen in verschiedenen Audiodateien

[Tenacity](https://tenacityaudio.org/) – Bearbeitung von Störgeräuschen in verschiedenen Audiodateien

Wir haben außerdem verschiedene Ideen von Mitgliedern des TMW-Discord-Servers erhalten, darunter auch den Namen des Decks. Die Sätze selbst stammen aus verschiedenen Core-Decks von Anki.


