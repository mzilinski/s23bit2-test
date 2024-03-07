# Linux Administrative Guide
## Linux-Dateirechte

In Linux hat jede Datei und jedes Verzeichnis eine Reihe von Berechtigungen, die bestimmen, wer die Datei oder das Verzeichnis lesen, schreiben oder ausführen kann. Diese Berechtigungen sind in drei Gruppen unterteilt:

- Benutzer: Der Eigentümer der Datei.
- Gruppe: Andere Benutzer, die zur gleichen Gruppe gehören wie die Datei.
- Andere: Alle anderen Benutzer auf dem System.

Jede dieser Gruppen hat drei Berechtigungen:

- Lesen (r)
- Schreiben (w)
- Ausführen (x)

Die Berechtigungen einer Datei können mit dem Befehl `ls -l` angezeigt werden. Sie erscheinen in der Ausgabe als eine Reihe von zehn Zeichen, z. B. `-rw-r--r--`. Das erste Zeichen gibt den Dateityp an (z. B. `-` für eine normale Datei, `d` für ein Verzeichnis). Die nächsten neun Zeichen repräsentieren die Berechtigungen für Benutzer, Gruppe und andere (jeweils drei Zeichen).

Die Berechtigungen können mit dem Befehl `chmod` geändert werden. Zum Beispiel ändert `chmod u+x dateiname` die Berechtigungen der Datei `dateiname`, so dass der Benutzer sie ausführen kann.
