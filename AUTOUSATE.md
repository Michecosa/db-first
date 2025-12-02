# DB SCHEMA

Struttura di una tabella per la gestione delle auto usate messe in vendita da un concessionario

## Nome tabella: AUTO USATE (nome entità: auto_usate)

Colonne:

- id_auto INT **PRIMARY KEY**, AUTO_INCREMENT, NOT NULL
- marca VARCHAR(50) NOT NULL
- modello VARCHAR(50) NOT NULL
- anno_immatricolazione YEAR NOT NULL
- chilometraggio INT NOT NULL
- alimentazione VARCHAR(20) NOT NULL
- cambio VARCHAR(20) NOT NULL
- prezzo DECIMAL(10,2) NOT NULL
- colore VARCHAR(30) NULL
- targa CHAR(7) NOT NULL UNIQUE
- stato_auto VARCHAR(20) NOT NULL DEFAULT('Disponibile')
- data_arrivo DATE NOT NULL DEFAULT(now())
- cilindrata SMALLINT NOT NULL
- potenza SMALLINT NOT NULL
- note TEXT NULL

## Tabella: AUTO USATE

| Colonna                     | Tipo          | Vincoli                               |
| --------------------------- | ------------- | ------------------------------------- |
| **_id_auto_**               | INT           | PRIMARY KEY, NOT NULL, AUTO_INCREMENT |
| **_marca_**                 | VARCHAR(50)   | NOT NULL                              |
| **_modello_**               | VARCHAR(50)   | NOT NULL                              |
| **_anno_immatricolazione_** | YEAR          | NOT NULL                              |
| **_chilometraggio_**        | INT           | NOT NULL                              |
| **_alimentazione_**         | VARCHAR(20)   | NOT NULL                              |
| **_cambio_**                | VARCHAR(20)   | NOT NULL                              |
| **_prezzo_**                | DECIMAL(10,2) | NOT NULL                              |
| **_colore_**                | VARCHAR(30)   | NULL                                  |
| **_targa_**                 | CHAR(7)       | NOT NULL, UNIQUE                      |
| **_note_**                  | TEXT          | NULL                                  |
