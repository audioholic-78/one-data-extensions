# imx.Platform

## Anbieter

**destination.one GmbH** – Hersteller von one.data. Diese Extension gehört zum offiziellen Katalog
[one-data-extensions](https://github.com/audioholic-78/one-data-extensions) und wird mit one.data gepflegt.

- Web: [www.destination.one](https://www.destination.one)
- Kontakt: [info@destination.one](mailto:info@destination.one)

## Kurzbeschreibung

Objekte aus der imx.Platform (infomax) mit Paging übernehmen.

## Beschreibung

![Konnektor aus der Vorlage anlegen](screenshots/01-konnektor.png)

![Ablauf](screenshots/02-ablauf.png)

Beim Anlegen unter *Administration → Konnektoren* ist die Konfiguration vorbelegt. Platzhalter in Großbuchstaben (z. B. `PROJEKT`, `INSTANZ`) ersetzen und Zugangsdaten nur als **Name eines Secrets** (`credentials_ref`) hinterlegen.

**Hinweis:** Instanz-URL und Token je Mandant.

### Konfiguration

```json
{
  "url": "https://INSTANZ.imxplatform.de/api/objects?pageSize=500",
  "items_path": "items",
  "id_path": "id",
  "next_path": "links.next",
  "auth": {
    "type": "header",
    "name": "Authorization"
  }
}
```

Das Mapping auf den one.data-Datenstandard wird je Instanz unter *Konnektoren → Mapping* gepflegt.
