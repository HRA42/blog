+++
title = "Künstliche Intelligenz - Die Zukunft der Suchmaschinen?"
description = "Ist KI die Zukunft der Suchmaschinen? - Spoiler: Nein!"
date = "2023-05-23"
tags = [
        "Suchmaschinen",
        "Künstliche Intelligenz"
]
author = "Henry Rausch"
+++

## Was meine ich mit “Künstlicher Intelligenz”?

Es ist dir vermutlich nicht entgangen, in den vergangenen Wochen und Monaten war überall die Rede von „GPT“. 
Dabei handelt es sich um die „Generative Pre-trained Transformer“ Technik, eine Art künstlicher Intelligenz, die in der Lage ist, auf Basis von Texten, eigene Texte zu generieren. 
Die Technik hat den Vorteil, dass sie Texte erzeugt, die in vielen Fällen sehr menschenähnlich wirken. 
Das bedeutet, dass sie beispielsweise genutzt werden kann, um automatisch Texte zu generieren, die dann von Menschen überarbeitet werden können. 
Die automatische Generierung von Texten in Chatbots oder anderen Anwendungen kann von GPT profitieren.

{{< rawhtml >}}
<div style="display: flex; justify-content: center;">
    <div style="text-align: center;">
        <img src="/KI-SE/Meme1.jpg" height="400" />
    </div>
</div>
{{< /rawhtml >}}

Grade die von OpenAI erstellte Anwendung “ChatGPT” ist im Moment sehr beliebt. 
Sie bietet ein Eingabe Fenster und generiert daraufhin eine Ausgabe auf Grundlage der Datenquellen von OpenAI. 
OpenAI macht die Datensätze die für das Training von GPT verwendet wurden nicht öffentlich, sodass nicht klar ist welchen Quellen sich ChatGPT bedient. 
Am 12. Mai 2023 wurden sogenannte “Plugins” sowie ein Webbrowser für ChatGPT in einer Beta Phase vorgestellt. 
Damit ist ChatGPT in der Lage aktuelle Informationen aus dem Internet bzw. über die Plugins zu beziehen. 
Durch die Nutzung dieser beiden Techniken werden die Quellen und die Recherche Methoden transparenter, auch wenn mir noch nicht klar ist, wie ChatGPT entscheidet ob auf einen Datensatz des Tranings oder eines der verfügbaren Plugins zurück gegriffen wird. 
Ich werde in einem der nächsten Beiträge verstärkt auf das Thema Plugins eingehen.

<details>
<summary>Technik hinter den Generative Pre-trained Transformern ❗</summary>
Ohne jeden Zweifel ist die "Generative Pre-trained Transformer"-Technik die revolutionärste Anwendung von "Künstlicher Intelligenz", die wir bis heute gesehen haben und allgemein zugänglich ist. Allerdings stellt sich mir die Frage, was genau an einem GPT so intelligent sein soll, denn die Technik verwendet eben keine Intelligenz, um den Kontext zu verstehen. 
Im Grunde ist es ein sehr guter Algorithmus, der auf Basis von Wahrscheinlichkeit den nächsten besten Buchstaben, das nächste beste Wort und den nächsten besten Satz vorhersagt. 
Im Folgenden möchte ich kurz auf die Details dieses Sprachmodells eingehen.

GPT ist ein sogenanntes "Large Language Model", ein großes Sprachmodell, das mithilfe eines Datensatzes auf die korrekte Ausgabe von Sprache trainiert wurde. 
Dazu werden im Wesentlichen zwei Techniken eingesetzt:

1. Unbeaufsichtigtes Lernen bedeutet, dass das Programm Daten aus dem Trainingssatz verarbeitet, um zu "lernen". Es bestimmt also die einzelnen Parameter natürlicher Sprache und versteht den Aufbau von Sätzen. 
Im Grunde funktioniert es dabei ein bisschen wie beim Erlernen einer Sprache: Zuerst musst du die Vokabeln lernen, um zu verstehen, wie du bestimmte Worte korrekt benutzt.
2. Beaufsichtigtes Lernen kann man sich wie eine Sprachreise in ein anderes Land vorstellen. 
Dabei lernt man den Kontext, in dem die Sprache verwendet wird, kennen. 
Man kann sich das sehr gut an dem englischen Wort "funny" verdeutlichen. Die Vokabel sagt korrekt übersetzt "lustig". Wenn man jedoch in England ist, wird "funny" häufiger in der Bedeutung "komisch" verwendet. Mit Chat GPT wird ein Text vorgelegt und dazu die Bedeutung des Texts erklärt, sodass die einzelnen Wörter einen Kontext bekommen und dem Programm klar wird, wie es welche Worte verwenden muss.
Das wichtigste Merkmal des Sprachmodells ist die Ausgabe von Wahrscheinlichkeiten. Das Programm sagt nur den nächsten Buchstaben, das nächste Wort und den nächsten Satz voraus. 
Es ist häufig möglich, eine andere Antwort zu generieren, indem man einfach die Frage wiederholt. Daher sind die Informationen eines Sprachmodells nicht immer korrekt.

{{< rawhtml >}}
<div style="display: flex; justify-content: center;">
    <div style="text-align: center;">
        <img src="/KI-SE/SchemaKI.png" height="400" />
    </div>
</div>
{{< /rawhtml >}}

Für diesen Beitrag reicht eine oberflächliche Betrachtung aus. Wenn du weitere Informationen benötigst, empfehle ich dir folgende Quellen:

- [Übersicht von OpenAI](https://openai.com/product/gpt-4)
- [Funktionsweise von Sprachmodellen von Spektrum der Wissenschaft](https://www.spektrum.de/news/wie-funktionieren-sprachmodelle-wie-chatgpt/2115924)
- [Einführung in das GPT Modell von Rahul Prsad M.](https://medium.com/@rahulmallah785671/a-brief-about-gpt-model-1cde6409763d)
- [Übersicht über die Probleme von Generativer AI von Freedom Preetham](https://medium.com/autonomous-agents/mathematically-evaluating-hallucinations-in-llms-like-chatgpt-e9db339b39c2)
- [Die Natur von GPT von John Nosta](https://johnnosta.medium.com/the-nature-of-gpt-hallucinations-and-the-human-mind-c1e6fd63643d)
</details>

## Implementierung in Suchmaschinen

Neeva AI, Google Bard, Microsoft Bing Chat und dutzende andere Unternehmen integrieren künstliche Intelligenz in ihre Suchmaschinen.
Microsoft entwickelt auch Github Copilot, eine Programmierassistenz, die bei der Entwicklung von Github hilft. 
Ähnliche Funktionen für Microsoft Office-Programme sind in Arbeit. 
Ich habe viele dieser Dienste in den letzten Wochen und Monaten ausprobiert und möchte im Folgenden einige Produkte vorstellen:

### Neeva AI

{{< notice warning >}}
❗ Am 20. Mai 2023 gab Neeva die Einstellung ihrer Suchmaschine bekannt. 
Ich habe Neeva seit dem Erscheinen in Deutschland aktiv genutzt und war in einer internen Gruppe mit den Entwicklern verbunden. 
Die Einstellung war einer der ausschlaggebenden Punkte für diesen Beitrag.

[Weitere Informationen zur Einstellung von Neeva Search](https://neeva.com/blog/may-announcement)
{{< /notice >}}

Neeva AI war eine werbefreie und datenschutzfreundliche Suchmaschine auf Basis künstlicher Intelligenz, die personalisierte Ergebnisse lieferte und Abonnements für bestimmte Themen anbot. 
Das Unternehmen wurde von ehemaligen Google-Mitarbeitern gegründet, um eine bessere Suche anzubieten, die sich auf die Bedürfnisse der Nutzer konzentriert. 
Sie entwickelten ihren eigenen Suchindex und ein eigenes Sprachmodell.

Ich habe vor Neeva, SearchXNG auf meinen Servern zu hosten und aktiv genutzt. 
SearchXNG ist eine Metasuchmaschine, die sehr flexibel konfigurierbar ist und verschiedene Suchmaschinen für jede Suche nach den Ergebnissen befragt und diese nach persönlicher Präferenz sortiert ausgibt.

Im Oktober 2022 wurde ich von meinem Kontakt bei Neeva gefragt, ob ich Interesse hätte, einen frühen Zugang zur deutschen Version zu nutzen.
Im Dezember wurde Neeva dann offiziell in Deutschland eingeführt. 
Ich habe sofort alle Webbrowser auf die neue Suchmaschine umgestellt und sie bis zur Ankündigung der Abschaltung aktiv genutzt.

Neeva war mit weitem Abstand die beste Suchmaschine, die ich bis dahin verwendet hatte.
Sie lieferte mir die besten Suchergebnisse für meine tägliche Arbeit und zeigte dabei keinerlei Werbung.
Zusätzlich konnte ich meinen Google-, Microsoft- und Github-Account verknüpfen und somit aus der Suche heraus auf alle meine Dateien und E-Mails zugreifen.
Wie du merkst, war ich sehr begeistert von diesem Paket.

Im Februar wurde Neeva AI angekündigt, ein in die Suche integrierter AI-Assistent, der eine Zusammenfassung der Suchergebnisse automatisch generierte und als erstes Suchergebnis anbot. 

{{< rawhtml >}}
<div style="display: flex; justify-content: center;">
    <div style="text-align: center;">
        <img src="/KI-SE/SchemaNeevaAI.jpg" height="400" />
    </div>
</div>
{{< /rawhtml >}}

Für mehr Informationen über die Funktionsweise kannst du den Beitrag von Neeva auf Twitter dazu lesen:
[Wie funktioniert Neeva AI?](https://twitter.com/neeva/status/1643659558160683011?s=46&t=xebfLU7XJLaZSBio9PNplg)

Ich fragte mich damals schon, ob ich dieses Feature in meinen Alltag integrieren könnte. 
Drei Monate später stellte ich fest, dass ich die Zusammenfassungen meistens ignorierte und fast immer lieber auf ChatGPT zurückgriff, wenn ich eine spezifische Frage hatte. 
Ende April wurde bekannt gegeben, dass Neeva die Integration von Apps sowie die Linksammlung “Spaces” ab Mitte Mai einstellt.
Aus heutiger Sicht ist dies verständlich, da die Finanzierung des Dienstes scheinbar nicht mehr gewährleistet werden konnte, was bei 2 Millionen aktiven Nutzern ziemlich merkwürdig ist.

Die mediale Berichterstattung über das Ende von Neeva zeigt mir wieder einmal sehr deutlich, wie manches Medium gerne einmal die Worte im Mund herumdreht.
Ob dies nun der Tatsache geschuldet ist, dass man das Original nicht versteht oder nicht verstehen will, vermag ich nicht zu beurteilen.

Es ist schade um Neeva, die entwickelte Technologie sowie die 2 Petabyte an Webseiten, die seit 2019 gesammelt wurden.

### Google Bard

Google Bard ist ein Chatprogramm, das von Google entwickelt wurde, um mit Microsofts Bing Chat zu konkurrieren.
Die Anwendung basiert auf dem Pathways Language Model 2, kurz: PaLM2, das von Google entwickelt wurde und in etwa halb so Leistungsfähig wie GPT4 ist.
Jan-Keno Janssen vom c’t Magazin hat Google Bard ausführlich getestet und festgestellt das Bard sehr gut darin ist Zusammenfassungen von Texten zu erstellen. 
Es sei außerdem viel schneller als ChatGPT und Bing Chat. 
Die Ergebnisse von Bard sind allerdings nicht so gut wie die von ChatGPT. 

{{< rawhtml >}}
<div style="display: flex; justify-content: center;">
    <div style="text-align: center;">
        <img src="/KI-SE/Meme2.jpg" height="400" />
    </div>
</div>
{{< /rawhtml >}}

Ich konnte Google Bard auch bereits ausprobieren und war enttäuscht weil es mir auf viele technische Fragen einfach keine Antworten geben konnte oder wollte.
Das ist erwartbar da sich Google bereits bei der Vorstellung blamierte als Bard falsche Informationen heraus gab. 
Auf die Vorstellung entbrannte eine Debatte über Regulierung von diesen Chat Programmen. 

Wenn du mehr über Google Bard erfahren möchtest findest du das Video von c’t 3003 zu Google Bard hier:

{{< youtube 1TOFiUyZu8I >}}

## Generative Künstliche Intelligenz als Zukunft der Suchmaschine?

Jedes Unternehmen das mit Suchmaschinen Geld verdient ist im Moment dabei die eine oder andere Form von Generativer Künstlicher Intelligenz in das jeweilige Produkt zu integrieren.
Die Entwicklungen des letzten halben Jahres zeigt das es noch kein klares Modell gibt wie man die klassische Suchmaschine am besten mit Künstlicher Intelligenz verbindet.
Microsoft und Google bieten ihre KI als zusätzliche Option der Suche an, viele kleinere Unternehmen nutzen die Technik für Zusammenfassungen von Webdokumenten.

Mein Arbeitsprozess hat sich durch künstliche Intelligenz in den jeweiligen Produkten nicht nachhaltig verändert.
Ich nutze Suchmaschinen häufig wenn noch keine genaue Vorstellung habe was ich suche. 
Beispielsweise suche ich oft nach Dokumentationen eines bestimmten Produkt um mir einen Eindruck davon zu machen ob ich es testen möchte und um zu Erfahren wie ich es effektiv einsetze.
Dabei ist Künstliche Intelligenz zumindest im Moment häufig noch nicht hilfreich, da die Informationen entweder veraltet oder nicht vorhanden sind.
Ich habe selten einen echten Mehrwert aus Zusammenfassungen von Webdokumenten ziehen können, da häufig zwar das große ganze korrekt erfasst und zusammengefasst wird, aber die Details Informationen nicht vorhanden sind.
Speziell wenn man nach bestimmten Fehlermeldungen oder Programmlösungen sucht sind normale Suchmaschinen deutlich effektivier wenn der Fehler sehr spezifisch ist.
Ich habe jeden Tag mit Fehlermeldungen in Datev zutun die häufig kryptisch sind, da die meisten Fehler nur eine Nummer tragen, zum Beispiel: 

> #SC00006F - Es ist der Fehler (6) beim Aufruf einer Komponente des Sicherheitspakets aufgetreten.
> 

Fragt man nun ChatGPT was das bedeuten könnte, gibt selbst die aktuelle Version mit Zugang zum Internet keine Information aus. 
Man solle die Datev Dokumentation aufsuchen und dort den Fehler ausfindig machen. 
So schnell ist man wieder zurück in der Welt der Suchmaschinen. 
Da die Software Landschaften immer komplexer und umfangreicher wird sind die häufig sehr generellen Lösungen generativer KI nicht ausreichend um ein komplexes Fehlerbild zu Analysieren und zu beheben.

{{< rawhtml >}}
<div style="display: flex; justify-content: center;">
    <div style="text-align: center;">
        <img src="/KI-SE/Meme3.png" height="400" />
    </div>
</div>
{{< /rawhtml >}}

Ich glaube das die Zukunft von Suchmaschinen grade im Bereich der Vernetzung die Nutzererfahrung deutlich verbessern kann. 
Eine Suche die durch alle deine Anwendungen Informationen finden kann. 
Das wäre ein echter Meilenstein und würde das Finden von Informationen deutlich vereinfachen. 
Viele Unternehmen haben sehr gute, umfangreiche Dokumentationen. 
Allerdings ist es schwer genau diese Informationen zu finden, wenn man nicht genau weiß was man sucht. 
Hier könnte eine Suchmaschine der Zukunft definitiv einen Durchbruch erzielen.

Wie ist deine Meinung zu Künstlicher Intelligenz in Suchmaschinen? Was glaubst du wie die Zukunft die Suche nach Informationen verändern wird?