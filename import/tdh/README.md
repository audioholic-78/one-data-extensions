# Tourismus-Datenhub TDH (XML)

## Anbieter

**destination.one GmbH** – Hersteller von one.data. Diese Extension gehört zum offiziellen Katalog
[one-data-extensions](https://github.com/audioholic-78/one-data-extensions) und wird mit one.data gepflegt.

- Web: [www.destination.one](https://www.destination.one)
- Kontakt: [info@destination.one](mailto:info@destination.one)

## Kurzbeschreibung

Migration aus dem Tourismus-Datenhub: XML-Exportdateien (Element item) übernehmen.

## Beschreibung

![Format in der Datenmigration auswählen](screenshots/01-datenmigration.png)

![Ablauf](screenshots/02-ablauf.png)

Unter *Administration → Datenmigration* das Format wählen und die Datei hochladen. Die Datensätze landen quellgetreu im Staging; danach eine Mapping-Version wählen und importieren.

**Hinweis:** Exportdatei aus dem TDH hochladen.

### Optionen

```json
{
  "record_element": "item",
  "id_path": "@id",
  "type_path": "@type"
}
```
