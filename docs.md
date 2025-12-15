Was macht das Dockerfile? 
FROM alpine:latest	  Nimmt ein sehr kleines Linux-Betriebssystem als Basis
COPY app.sh /app.sh	  Kopiert app.sh in den Container
RUN chmod +x /app.sh	Macht das Container ausführen darf / kann
CMD ["/app.sh"]	      Startet den Container und führt das Skript aus

Was ist der Zweck der Pipeline? 
Er soll jedes mal automatisch nachdem man etwas pusht das Projekt ausführen und testen.

Was war für dich der schwierigste Teil dieser Aufgabe und warum?
An sich ist es nicht schwer, jedoch muss man die Befehle kennen und sehr genau arbeiten. 
Ich hatte zb in meinem Echo ein Leerzeichen zu viel, deswegen funktionierte es nicht.
Es ist sehr gut, dass man das so direkt praktisch mal macht, so hat man erste Erfolge und versteh besser wofür wir das machen und brauchen.

Bonus 1:
Meine Pipeline läuft bei push und pull_request auf main.

Bonus 2:

Bonus 3:
Warum sind automatische Pipelines sinnvoll?
-Änderungen automatisch getestet werden und aufgebaut.
-es einfacher und schneller geht als manuell zu testen.
-weniger menschliche Fehler passieren.
-stellt sicher, dass das Projekt funktionsfähig ist.

Wo siehst du CI/CD in echten Projekten?
Ich würde sagen überall wo an Projekten, egal ob WebApp, Spiele usw, da es Qualität, Kosten und Zeit positiv beeinflusst.
