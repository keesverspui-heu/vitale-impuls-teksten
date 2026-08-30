# De teksten van vitale-impuls.nl

Deze map bevat alle zichtbare teksten van de website, los van de code.
Eén bestand per pagina, plus `paginas.md` voor titels, omschrijvingen en
menunamen.

## Vorm
Elk bestand bestaat uit blokken:

    ## sleutel
    de tekst

De sleutel komt terug in de HTML van de site als `{{sleutel}}`. Wie een
sleutel weghaalt of hernoemt, breekt de bouw: `build.py` stopt met een
foutmelding zodra er een `{{...}}` overblijft.

## Wat er in een tekst mag
Platte tekst, en verder alleen:

    **vet**   *schuin*   [woorden](/pad)

Meer niet. Geen HTML, geen scripts. De keuring in het beheerscherm weigert
de rest.

## Wie schrijft hier
- Rinda, via het beheerscherm (dat schrijft naar tak `test`).
- Claude, bij het bouwen aan de site (ook naar tak `test`).

## Takken
- `test` — wat er op de testsite staat.
- `main` — wat er op de echte site staat. Kees zet dat live, niemand anders.

De code van de site staat in de repository `vitale-impuls-site`. Bij het
bouwen wordt deze repository daar als map `teksten/` naast gezet.
