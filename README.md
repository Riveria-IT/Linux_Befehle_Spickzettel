# Linux Befehle – Spickzettel

Ein kompakter und schön strukturierter Überblick über die wichtigsten Linux-Befehle für den Alltag.  
Ideal für **Anfänger**, **Server-Verwaltung**, **Ubuntu/Debian** und allgemeine Terminal-Arbeit.

---

## Inhalt

- [Navigation](#navigation)
- [Dateien und Ordner](#dateien-und-ordner)
- [Dateien ansehen und bearbeiten](#dateien-ansehen-und-bearbeiten)
- [Suchen](#suchen)
- [Rechte und Besitzer](#rechte-und-besitzer)
- [Prozesse](#prozesse)
- [Systeminformationen](#systeminformationen)
- [Netzwerk](#netzwerk)
- [Pakete und Updates](#pakete-und-updates)
- [Dienste](#dienste)
- [Logs](#logs)
- [Archive](#archive)
- [Benutzer](#benutzer)
- [Die 10 wichtigsten Befehle](#die-10-wichtigsten-befehle)

---

## Navigation

### Aktuellen Ordner anzeigen
```bash
pwd
```

### Dateien und Ordner anzeigen
```bash
ls
```

### Detaillierte Ansicht inklusive versteckter Dateien
```bash
ls -la
```

### In einen Ordner wechseln
```bash
cd ordnername
```

### Einen Ordner zurück
```bash
cd ..
```

### Ins Home-Verzeichnis wechseln
```bash
cd ~
```

---

## Dateien und Ordner

### Ordner erstellen
```bash
mkdir test
```

### Leere Datei erstellen
```bash
touch datei.txt
```

### Datei kopieren
```bash
cp datei.txt kopie.txt
```

### Ordner mit Inhalt kopieren
```bash
cp -r ordner1 ordner2
```

### Datei verschieben oder umbenennen
```bash
mv alt.txt neu.txt
```

### Datei löschen
```bash
rm datei.txt
```

### Ordner löschen
```bash
rm -r ordner
```

### Ordner mit Inhalt zwangsweise löschen
```bash
rm -rf ordner
```

> Vorsicht: `rm -rf` löscht ohne Rückfrage.

---

## Dateien ansehen und bearbeiten

### Inhalt direkt anzeigen
```bash
cat datei.txt
```

### Datei seitenweise lesen
```bash
less datei.txt
```

### Datei mit Nano bearbeiten
```bash
nano datei.txt
```

### Datei mit Vim bearbeiten
```bash
vim datei.txt
```

---

## Suchen

### Datei nach Namen suchen
```bash
find /pfad -name datei.txt
```

### Wort in Datei suchen
```bash
grep "wort" datei.txt
```

### Rekursiv in Ordnern suchen
```bash
grep -r "wort" /pfad
```

---

## Rechte und Besitzer

### Datei ausführbar machen
```bash
chmod +x script.sh
```

### Rechte manuell setzen
```bash
chmod 755 datei
```

### Besitzer ändern
```bash
chown user:user datei
```

---

## Prozesse

### Laufende Prozesse anzeigen
```bash
ps aux
```

### Live-Prozessübersicht
```bash
top
```

### Komfortablere Prozessübersicht
```bash
htop
```

### Prozess beenden
```bash
kill PID
```

### Prozess hart beenden
```bash
kill -9 PID
```

---

## Systeminformationen

### Systemdetails anzeigen
```bash
uname -a
```

### Aktuellen Benutzer anzeigen
```bash
whoami
```

### Speicherplatz prüfen
```bash
df -h
```

### Ordnergröße anzeigen
```bash
du -sh ordner
```

### RAM-Auslastung anzeigen
```bash
free -h
```

### Laufzeit des Systems anzeigen
```bash
uptime
```

---

## Netzwerk

### IP-Adressen anzeigen
```bash
ip a
```

### Verbindung testen
```bash
ping google.com
```

### Webseite oder API abrufen
```bash
curl https://example.com
```

### Datei herunterladen
```bash
wget https://example.com/datei.zip
```

### Offene Ports und Dienste anzeigen
```bash
ss -tulpn
```

---

## Pakete und Updates

### Ubuntu / Debian
```bash
sudo apt update
sudo apt upgrade
```

```bash
sudo apt install paketname
```

```bash
sudo apt remove paketname
```

### Rocky Linux / AlmaLinux / CentOS
```bash
sudo dnf update
sudo dnf install paketname
```

---

## Dienste

### Status eines Dienstes prüfen
```bash
systemctl status nginx
```

### Dienst starten, stoppen oder neu starten
```bash
sudo systemctl start nginx
sudo systemctl stop nginx
sudo systemctl restart nginx
```

### Dienst beim Systemstart aktivieren
```bash
sudo systemctl enable nginx
```

---

## Logs

### Logs eines Dienstes anzeigen
```bash
journalctl -u nginx
```

### Wichtige Systemfehler anzeigen
```bash
journalctl -xe
```

### Logdatei live verfolgen
```bash
tail -f /var/log/syslog
```

---

## Archive

### Archiv erstellen
```bash
tar -czf backup.tar.gz ordner/
```

### Archiv entpacken
```bash
tar -xzf backup.tar.gz
```

### ZIP-Datei entpacken
```bash
unzip datei.zip
```

---

## Benutzer

### Benutzer erstellen
```bash
adduser neueruser
```

### Passwort setzen
```bash
passwd neueruser
```

### Zu anderem Benutzer wechseln
```bash
su - benutzername
```

### Befehl mit Adminrechten ausführen
```bash
sudo befehl
```

---

## Die 10 wichtigsten Befehle

```bash
ls
cd
pwd
cp
mv
rm
nano
sudo
systemctl
ip a
```

---

## Tipps für den Alltag

### Letzte Befehle anzeigen
```bash
history
```

### Terminal leeren
```bash
clear
```

### Hilfe zu einem Befehl anzeigen
```bash
man ls
```

### Letzten Befehl mit sudo wiederholen
```bash
sudo !!
```

---

## Hinweis

Diese Datei ist als schneller Spickzettel gedacht.  
Je nach Linux-Distribution können einzelne Befehle leicht abweichen.

---

## Lizenz

Frei nutzbar für private und berufliche Zwecke.
