# Parola segreta

Gioco in rete: il server sceglie una parola di cinque lettere, i giocatori provano
a indovinarla.

Federico Di Marzio


## API

- POST /partite : comincia una partita. Risposta 201.
- GET /partite/N : stato della partita N. Risposta 200, oppure 404.
- POST /partite/N/tentativi : propone una parola, nel corpo in JSON.
Risposta 201, oppure 400 o 404.
