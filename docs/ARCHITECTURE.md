# Zielarchitektur

```text
Anwendung / Nutzer / optionales Agentenwerkzeug
              |
        API-Vertrag + Policy
              |
   Gateway auf ausdrücklich gewähltem Host
              |
      geprüfter Backendadapter
              |
   ein konfigurierter Text-Inferenzworker
```

Ein Gerät darf mehrere Rollen tragen. Für einen Einzelhost ist kein Tunnel nötig.
Im Heimnetz können Rollen getrennt werden. Entfernte Gateways und private Tunnel sind optional.
Für PS5 beschreibt das experimentelle Referenzprofil den Weg über einen Heimnetzvermittler,
Reverse-SSH, VPS und optionalen HTTPS-Edge. Ein PC benötigt diesen Konsolen-Bootstrap nicht.

## Rollen

Client: stellt Anfragen und zeigt Ergebnisse. Gateway: Auth, validierte Felder, Grenzen und Abbruch.
Relay: Transport; kein automatischer Inferenzprozess. Worker: berechnet eine deklarierte Fähigkeit.
Koordinator: später optionales Modul für die Zuteilung ganzer unabhängiger Aufgaben.
Speicher-/Indexdienst: später gesonderte Fähigkeit, kein inhärenter Teil des Textworkers.

## Vertrag und Ausfälle

Erster Kandidat: GET /health, GET /v1/models, POST /v1/chat/completions für Text, optional SSE.
Modellaliase statt privater Dateipfade; keine frei wählbaren Request-Upstream-URLs.
Unsupported Features werden abgewiesen. Fehlende Usage bleibt unbekannt.
Headerzeit, erster sichtbarer Text und vollständige Antwortdauer sind getrennte Messpunkte.
Kein nachträglicher HTTP-504-Wechsel nach Beginn eines 200-Streams; Abbruch bleibt unvollständig.
Nach unbestätigtem Workerabbruch den einzigen Slot nicht voreilig erneut vergeben.

## Vertrauensgrenzen

Endpunktregistrierung ist eine Betreiberhandlung, kein Netzscan und keine Hardwareverifikation.
TLS/SSH nicht als Schutz eines unverschlüsselten letzten LAN-Hops ausgeben.
Authentifizierung am Gateway sichert keine direkt erreichbare Konsolenverwaltung.
Keine vertraulichen Prompts ungefragt in Cloud-/Fallbackpfade schicken. Keine globale
Speicheraggregation, kein Versprechen einer direkten Nutzung fremder GPUs durch einen Tunnel.
