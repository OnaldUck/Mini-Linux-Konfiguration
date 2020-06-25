# Mini-Linux-Konfiguration
Eine kleine Sammlung der wichtigsten Befehle für die sporadische Linux Nutzung.
Es ist als eine erinnerungsstütze gedacht. Wenn man 1x pro Jahr damit zu tun hat muss Mann wieder die Suchmaschine bemühen

Ich verzichte überall `sudo` einzuschieben. Wenn es benötigt wird, wird man dazu ehe aufgefordert. 

## Betriebssystem aktualisieren 

Befehl | Funktion
-- | --
`apt update` | Aktualisierungen suchen
`apt upgrade` | alle Aktualisierungen installieren
`apt sysupgrade` | Systemupgrade, z.B. vom Ubuntu 19.x auf 20.x
`apt autoremove` | Bereinigung nach update oder Upgrade
`apt autoremove --purge` | erzwungenes Bereinigen

## OpenSSH Server installieren bzw. SSH (Putty) Zugriff erstellen

Befehl | Funktion
-- | --
`apt install openssh-server` | OpenSSH Server installieren
`ufw allow ssh` | Firewall für port 23 öffnen

Gegabenfalls folgende die Config editieren `nano /etc/ssh/sshd_config` und folgende Zeilen ampassen `PasswordAuthentication yes` und z.B. `AllowUsers andreas@192.168.*.*`

## Dateien / Ordner
Befehl | Funktion
-- | --
`rm -r -f [Ordner]` | Ordner inc. Unterorder löschen

