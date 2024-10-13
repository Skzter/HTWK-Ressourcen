# WLAN und VPN Anleitungen

## Einrichtung Eduroam für Androidgeräte

Für die Einrichtung wird eine Internetverbindung vorausgesetzt, um das Zertifikat zu installieren.

### Zertifikat installieren

Zuerst laden Sie das [Zertifikat](T-TeleSec_GlobalRoot_Class_2.crt) runter und installieren es. 

**Android 14**:  
WLAN-Einstellungen -> Zertifikat installieren -> T-TeleSec... Zertifikat auswählen und Namen vergeben.

**Android 13**:  
WLAN-Einstellungen -> Drei Punkte oben rechts -> Erweiterte Einstellungen -> Zertifikat hinzufügen ->  T-TeleSec... Zertifikat auswählen und Namen vergeben.

### Mit Eduroam verbinden

   - Eduroam auswählen
   - EAP-Methode: PEAP
   - Phase-2-Authentifizierung: MS-CHAP v2
   - CA-Zertifikat: Zertifikat mit vorher festgelegtem Namen auswählen
   - TLS: TLS v1.0 / TLS-SSL
   - Online-Zertifikatstatus: Nicht prüfen
   - Domain: radius.rz.htwk-leipzig.de
   - Identität: **HTWK-Login**@htwk-leipzig.de
   - Anonyme Identität: eduroam@htwk-leipzig.de
   - Passwort: **HTWK-Passwort**
   - Verbinden drücken  

   - Es funktioniert (hoffentlich).