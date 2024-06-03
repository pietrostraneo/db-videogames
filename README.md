# Archivio E-sports - README

## Descrizione
Questo progetto si propone di gestire un archivio di E-sports, includendo informazioni sui videogiochi, sulle software house produttrici, sui tornei e sui giocatori partecipanti. Il sistema permette anche di raccogliere recensioni dei giocatori e votazioni per i migliori videogiochi dell'anno.

## Schema E-R
Lo schema entità-relazione comprende le seguenti entità:

- **Videogioco**
  - Attributi:
    - Nome (stringa)
    - Trama (testo)
    - Data di rilascio (data)
  - Relazioni:
    - Produttore (Software House)
    - Piattaforme disponibili (Piattaforma)
    - Categorie (Categoria)
    - Classificazioni PEGI (Classificazione PEGI)
    - Recensioni (Recensione)

- **Software House**
  - Attributi:
    - Nome (stringa)
    - Partita IVA (stringa)
    - Città (stringa)
    - Nazione (stringa)
  - Relazioni:
    - Videogiochi prodotti

- **Piattaforma**
  - Attributi:
    - Nome (stringa)
  - Relazioni:
    - Videogiochi disponibili

- **Categoria**
  - Attributi:
    - Nome (stringa)
  - Relazioni:
    - Videogiochi appartenenti

- **Classificazione PEGI**
  - Attributi:
    - Nome (stringa)
  - Relazioni:
    - Videogiochi classificati

- **Torneo**
  - Attributi:
    - Nome (stringa)
    - Anno (data)
    - Città (stringa)
  - Relazioni:
    - Giocatori partecipanti

- **Giocatore**
  - Attributi:
    - Nome (stringa)
    - Cognome (stringa)
    - Nickname (stringa)
    - Città di provenienza (stringa)
  - Relazioni:
    - Tornei partecipati

- **Recensione**
  - Attributi:
    - Titolo (stringa)
    - Testo (testo)
    - Valutazione (da 1 a 5)
  - Relazioni:
    - Videogioco recensito

- **Premio**
  - Attributi:
    - Nome (stringa)
  - Relazioni:
    - Videogiochi premiati