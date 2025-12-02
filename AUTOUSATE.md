# DB SCHEMA

Struttura di una tabella per la gestione delle auto usate messe in vendita da un concessionario

## Nome tabella: AUTO USATE (nome entità: auto_usate)

Colonne:

- id_auto INT **PRIMARY KEY**, NOT NULL
- marca VARCHAR(50) NOT NULL
- modello VARCHAR(50) NOT NULL
- anno_immatricolazione YEAR NOT NULL
- chilometraggio INT NOT NULL
- alimentazione VARCHAR(20) NOT NULL
- cambio VARCHAR(20) NOT NULL
- prezzo DECIMAL(10,2) NOT NULL
- colore VARCHAR(30) NULL
- targa CHAR(7) NOT NULL UNIQUE
- note TEXT NULL

## Tabella: AUTO USATE

| Colonna               | Tipo          | Vincoli               |
| --------------------- | ------------- | --------------------- |
| id_auto               | INT           | PRIMARY KEY, NOT NULL |
| marca                 | VARCHAR(50)   | NOT NULL              |
| modello               | VARCHAR(50)   | NOT NULL              |
| anno_immatricolazione | YEAR          | NOT NULL              |
| chilometraggio        | INT           | NOT NULL              |
| alimentazione         | VARCHAR(20)   | NOT NULL              |
| cambio                | VARCHAR(20)   | NOT NULL              |
| prezzo                | DECIMAL(10,2) | NOT NULL              |
| colore                | VARCHAR(30)   | NULL                  |
| targa                 | CHAR(7)       | NOT NULL, UNIQUE      |
| note                  | TEXT          | NULL                  |
