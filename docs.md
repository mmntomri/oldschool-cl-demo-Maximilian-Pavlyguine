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

Meine Pipeline läuft bei push und pull_request auf main.
