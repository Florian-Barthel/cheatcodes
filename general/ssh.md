# [Home](../README.md)

### rsync

Install `sudo apt-get install rsync `
```sh
# Befehl
 rsync [OPTIONEN] QUELLE(N) ZIEL 

# Lokal -> Remote
rsync -a -e -P "ssh -p 3322" /home/linuxize/images/ user@12.12.12.12:/var/www/images/

# Remote -> Lokal
rsync -a -e -P "ssh -p 3322" user@12.12.12.12:/var/www/images/ /home/linuxize/images/

# optionen
-a # kopiert alle Eigenschaften 
--ignore-existing # schreibt nur neue Dateien
--delete # löscht Dateien die im Zielverzeichniss sodass die Ordner danach exakt gleich sind
-z # komprimiert Dateien vorher
-P # zeigt einen Progress Bar an
-e # wählt Remote Shell aus (für ssh)
```