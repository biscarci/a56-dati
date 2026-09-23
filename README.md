# Dati A56 — Tangenziale di Napoli

`status.json` con le chiusure programmate della Tangenziale di Napoli (A56),
aggiornato automaticamente ogni 6 ore.

**Fonte dei dati:** [tangenzialedinapoli.it](https://www.tangenzialedinapoli.it) —
avvisi ufficiali, interpretati da un parser automatico.

⚠️ **I dati possono contenere errori.** Verifica sempre sul sito ufficiale prima
di metterti in viaggio.

## Formato

```json
{
  "generatedAt": "2026-09-22T23:17:46+02:00",
  "sourceRange": "21.09 al 27.09.2026",
  "items": [
    {
      "id": "camaldoli",
      "direzione": "capodichino",
      "status": "giallo",
      "label": "Camaldoli — svincolo d'ingresso chiuso",
      "source": "rules",
      "windows": [{"from": "...", "to": "..."}]
    }
  ],
  "unparsed": [],
  "urgentNotice": null
}
```

- `direzione`: `capodichino` (verso le autostrade) o `pozzuoli`
- `status`: `verde` aperta · `giallo` svincolo/ingresso chiuso · `rosso` tratto chiuso con uscita obbligatoria
- `unparsed`: avvisi che il parser non ha saputo interpretare, in testo grezzo

Questo repository contiene solo i dati. Il codice che li genera è privato.
