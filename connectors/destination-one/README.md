# destination.one

## Anbieter

**destination.one GmbH** – Hersteller von one.data. Diese Extension gehört zum offiziellen Katalog
[one-data-extensions](https://github.com/audioholic-78/one-data-extensions) und wird mit one.data gepflegt.

- Web: [www.destination.one](https://www.destination.one)
- Kontakt: [info@destination.one](mailto:info@destination.one)

## Kurzbeschreibung

Datensätze aus destination.one (one.meta) über die REST-Suche übernehmen.

## Beschreibung

![Konnektor aus der Vorlage anlegen](screenshots/01-konnektor.png)

![Ablauf](screenshots/02-ablauf.png)

Beim Anlegen unter *Administration → Konnektoren* ist die Konfiguration vorbelegt. Platzhalter in Großbuchstaben (z. B. `PROJEKT`, `INSTANZ`) ersetzen und Zugangsdaten nur als **Name eines Secrets** (`credentials_ref`) hinterlegen.

**Hinweis:** Lizenzschlüssel als Secret hinterlegen, EXPERIENCE ersetzen.

### Konfiguration

```json
{
  "url": "https://meta.et4.de/rest.ashx/search/?experience=EXPERIENCE&type=POI&template=ET2014A.json&limit=500",
  "items_path": "items",
  "id_path": "global_id",
  "type_path": "type",
  "auth": {
    "type": "query",
    "name": "licensekey"
  }
}
```

Das Mapping auf den one.data-Datenstandard wird je Instanz unter *Konnektoren → Mapping* gepflegt.
