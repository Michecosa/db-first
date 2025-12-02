# DB SCHEMA

Struttura di una tabella per la gestione delle auto usate messe in vendita da un concessionario

## Nome tabella: AUTO USATE (nome entità: Auto_usate)

Colonne:

- id_auto INT
- marca VARCHAR(50)
- modello VARCHAR(50)
- anno_immatricolazione YEAR
- chilometraggio INT
- alimentazione VARCHAR(20)
- cambio VARCHAR(20)
- prezzo DECIMAL(10,2)
- colore VARCHAR(30)
- targa CHAR(7)
- note TEXT
