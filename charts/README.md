# Project Flight charts

Chart assets are grouped by airport ICAO code and are read-only in the app:

```text
charts/<ICAO>/<chart-name>.png
```

Examples:

- `charts/LCLK/Airport Diagram.png`
- `charts/LCLK/SID Runway 04.png`
- `charts/MDPC/STAR Runway 09 & 08.png`

The chart catalog in `index (6).html` supplies the display name for each file. Only repository maintainers should add or replace files in the matching ICAO folder and update `chartAssetCatalog`.
