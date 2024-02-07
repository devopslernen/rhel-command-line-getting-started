# Softwareverwaltung mittels DNF- und Yum- Paketmanager 

Auf Red Hat Enterprise Linux (RHEL) steht der Paketmanager "**"DNF (Dandified Yum)"** zur Softwareverwaltung zur Verfügung, der aus dem Paketmanager **"Yum"** hervorgegangen ist. DNF ermöglicht dabei u.a. die Installation, Deinstallation und Aktualisierung von Softwarepaketen. Der Nachfolger DNF ist hierbei kompatibel zu Yum, beispielsweise kann analog zu `dnf install` auch `yum install` verwendet werden.

- **Verfügbare Updates auflisten:**
  
  ```bash
  sudo dnf check-update
  ```
  
- **Softwarepakete installieren:**
  ```bash
  sudo dnf install paketname
  ```

- **Installation einer lokalen Paket-Datei (.rpm-Datei):**
  
  ```bash
  sudo dnf localinstall ./paketdatei.rpm
  ```
  
- **Softwarepaket deinstallieren:**
  ```bash
  sudo dnf remove paketname
  ```

- **Paket in Paketdatenbank suchen:**
  ```bash
  dnf search suchbegriff
  ```

- **Verfügbare Pakete auflisten:**
  
  ```bash
  dnf list
  ```
  
- **Installierte Pakete auflisten:**
  ```bash
  dnf list installed
  ```

- **Alle installierten Pakete aktualisieren:**
  ```bash
  sudo dnf upgrade
  ```

- **Automatische Deinstallation nicht mehr benötigter Pakete und Abhängigkeiten:**
  
  ```bash
  sudo dnf autoremove
  ```
  
- **Temporäre Dateien löschen - Cache bereinigen:**
  
  ```bash
  sudo dnf clean all
  ```
  
- **Infos zu Paket anzeigen:**
  ```bash
  dnf info paketname
  ```
