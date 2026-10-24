# onedata-ext – offizieller Katalog des one.data marketplace

Dieses Repo enthält die Extensions von destination.one für den **one.data marketplace** in one.data. Jede Extension liegt in
einem eigenen Ordner und wird einzeln installiert – über den Link auf den Unterordner:

```
https://github.com/audioholic-78/onedata-ext/tree/main/connectors/outdooractive
```

| Ordner | Art | Inhalt |
|---|---|---|
| `connectors/` | Konnektor | destination.one, mein.toubiz, imx.Platform, DataCycle, JOIN, Outdooractive, Maptoolkit, Regiondo, OpenStreetMap, VBB, Wikidata, Digitalize the Planet, OpenWeather, SkiData, TYPO3, OGC API – Features, n8n |
| `import/` | Datenmigration | DAMAS (XML), TDH (XML), generisches XML, generisches JSON |
| `export/` | Export | DAMAS-XML, TDH-XML (eingebaute Formate, `runtime: builtin`) |
| `schema/` | – | JSON-Schema für `extension.json` (Editor-Unterstützung) |

## Versionen

Jede Extension trägt ihre Version in `extension.json`. Updates prüft one.data am neuesten Tag des Repos
(`vX.Y.Z`, sonst `main`): Ist dort die Version im Unterordner höher als die installierte, zeigt der Marketplace
„Update verfügbar“.

## Eigene Extensions

Vorlagen für Partner: `onedata-ext-demo-import`, `onedata-ext-demo-connector`, `onedata-ext-demo-export`.
Leitfaden: `docs/EXTENSIONS.md` im one.data-Repo.
