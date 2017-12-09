# dreistesOpenSSH
## Beschreibung
Diese extrem dreiste Modifaktion des OpenSSH Servers soll dreisten Cybersecurity Analysts die Möglichkeit geben, die 
von fiesen Bösewichten probierten Passwörter zu loggen.
## Anleitung

1. Die `./configure` binary muss mit autoreconf aus dem Paket autoconf generiert werden. (einmalig pro System)
2. Mit `./configure --prefix=/DEIN/ZIEL/ --sysconfdir=/DEIN/ZIEL/` Projekt für das compilen "präperieren". (muss nur bei Änderungen der Pfade wiederholt werden)
3. Mit `make` compilen.
4. Mit `make install` nach /DEIN/ZIEL/ deployen.
5. Mit `mkdir /var/stolenPasswords` Pfad für geloggte Passworte bereitstellen.
6. In `/var/stolenPasswords/` werden die Passworte in der Datei `lowPw` gesammelt.

## Wichtig
Keine Gewährleistung für die Sicherheit. :(
