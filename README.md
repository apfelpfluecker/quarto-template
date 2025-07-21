# Quarto Template für Hausarbeiten und Essays

Dieses Repository ist ein Template, um mithilfe von [Quarto](https://quarto.org) Hausarbeiten, Essays und ähnliche Abgaben zu erstellen. Es empfiehlt sich, direkt mit Git zu arbeiten, weil das viele Vorteile (vor allem eine akkurate Versionierung des Arbeitsfortschritts, wodurch kaum Daten verloren gehen können) mit sich bringt. Genauso gut kann das Repository aber auch einfach nur heruntergeladen und offline, ganz ohne Git genutzt werden.

Das, was hier zu finden ist, spiegelt meinen aktuellen Wissensstand wieder, wie ich mit möglichst einfachen und niedrigschwelligen Mitteln technisch sehr schöne Dokumente erstellen kann, vor allem um damit Universitäts-Abgaben zu schreiben und mich nicht mit MS Word oder LO Writer rumschlagen zu müssen. Vielleicht hat dieses Repo auch einen Mehrwert für andere – das würde mich sehr freuen. Um den Einstieg zu erleichtern, habe ich versucht, die wichtigen Sachen, die man bei Bedarf ggf. ändern will, mithilfe von Kommentierungen verständlich zu machen. Im Zweifel schreibt mich an oder lest in der sehr detailierten [Doku von Quarto](https://quarto.org/docs/guide/) nach, die ich an dieser Stelle ausdrücklich empfehle.

Die konzipierte Struktur des Repos ist wie folgt (es sind nicht alle Ordner online, weil sie leer sind):

- `/assets`: Der Ordner ist für Skripte und ähnliches gedacht, die zum Bauen des Templates erforderlich sind.
  - `before-body.tex`: Das ist ein LaTeX-Partial (siehe Quarto-Doku), das das Titelblatt baut. Gegebenenfalls müssen Layoutanpassungen vorgenommen werden, die entsprechenden Stellen habe ich per Kommentar markiert.
  - `custom.scss`: Das tut Dinge fürs HTML-Layout, ist aber eigentlich nicht so wichtig, da für mich der PDF-Output im Vordergrung steht.
  - `springervs.csl`: Das ist der Zitierstil, ich hab jetzt mal einen von Springer VS genommen, aber da kann natürlich jeder beliebige genutzt werden. Im [Zotero Style Repository](https://www.zotero.org/styles) für Zitierstile finden sich quasi alle.
- `/images`: Der Ordner ist vorgesehen für Grafiken. Da man die in der Regel vermutlich direkt im Quarto-Dokument erstellt, braucht man den Ordner vermutlich nicht so oft.
- `/outputs`: Der Outputs-Ordner wird automatisch beim Rendern erstellt. Darin findet man dann das gerenderte Dokument, den Output eben.
- `index.qmd`: Das ist das Quarto-Dokument, in dem die Hausarbeit, das Essay oder was auch immer geschrieben wird.
- `_quarto.yml`: Das ist die Projekt-YML-Datei, in der ganz viele Einstellungen stehen, darunter Schriftgröße, Zeilenabstand, aber auch, ob ein Inhalts-, Abbildungs-, und/oder Tabellenverzeichnis erstellt werden soll. Allerdings gibt es auch einen YML-Block in der `index.qmd`-Datei, da sind dann vor allem dokumentspezifische Einstellungen drin (Autor\*inneninfos etc., Titel, Untertitel, …). Diese YML-Doppelstruktur macht im konkreten Fall nicht so richtig viel Sinn, aber für größere Dokumente, die eher in Richtung Masterarbeit oder Buch gehen, macht das dann mehr Sinn. So ist es evtl. ein kleines bisschen unübersichtlich, aber ich hoffe, nicht *zu* unübersichtlich.
- `quarto-template.Rproj`: Das ist die Projektdatei. Das Projekt sollte immer mit dieser Datei geöffnet werden. Gerne einfach nach Bedarf umbenennen.
- `README.md`: Das ist diese Datei. ;)
- `references.bib`: Das ist die Bibtex-Datei, in der die Zitationen gespeichert werden. Ich empfehle dringend, für Zitationen [Zotero](https://www.zotero.org/) zu nutzen, das hat nicht nur hierfür enorm viele Vorteile. Leider hat die Zotero-Integration von RStudio relativ viele Bugs, deswegen empfehle ich, die Zitationen als BetterBibLaTeX oder BibLaTeX aus Zotero zu exportieren. Ich habe noch keine optimale Lösung gefunden, aber das scheint mir im Moment die beste. Beim (Better-)BibTex-Export gehen leider wichtige Daten verloren.
- `.gitignore`: Das ist die gitignore-Datei. Wenn ihr Git kennt, brauche ich sie nicht erklären, wenn nicht, dann ignoriert sie einfach.

Ansonsten habt Spaß beim Schreiben und modifiziert gerne alles, was euch nicht passt. :)
