# Outdooractive

## Anbieter

**destination.one GmbH** – Hersteller von one.data. Diese Extension gehört zum offiziellen Katalog
[one-data-extensions](https://github.com/audioholic-78/one-data-extensions) und wird mit one.data gepflegt.

- Web: [www.destination.one](https://www.destination.one)
- Kontakt: [info@destination.one](mailto:info@destination.one)

## Kurzbeschreibung

Touren und Outdoor-Inhalte aus einem Outdooractive-Projekt übernehmen.

## Beschreibung

![Konnektor aus der Vorlage anlegen](screenshots/01-konnektor.png)

![Ablauf](screenshots/02-ablauf.png)

Beim Anlegen unter *Administration → Konnektoren* ist die Konfiguration vorbelegt. Platzhalter in Großbuchstaben (z. B. `PROJEKT`, `INSTANZ`) ersetzen und Zugangsdaten nur als **Name eines Secrets** (`credentials_ref`) hinterlegen.

**Hinweis:** Projekt-Kennung und API-Key.

### Konfiguration

```json
{
  "url": "https://www.outdooractive.com/api/project/PROJEKT/oois?display=verbose",
  "items_path": "tour",
  "id_path": "id",
  "auth": {
    "type": "query",
    "name": "key"
  }
}
```

Das Mapping auf den one.data-Datenstandard wird je Instanz unter *Konnektoren → Mapping* gepflegt.
