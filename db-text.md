<!-- Istruzioni:
Create un file di testo per descrivere un database di un negozio di videogiochi.
Strutturate il file come fatto oggi in classe.  Specificate: il nome del database, la tabella e le potenziali colonne con i tipi di dato. -->

<!-- DATABASE -->
# database name: Videgames
# nome tabelle: videogame
- id  UNIQUE AUTO_INCREMENT
- codex_ean-8   SMALL NOTNULL
- Titolo stringa VARCHAR(50) NOTNULL
- descrizone stringa TEXT NOTNULL
- autore stringa VARCHAR(30) NOTNULL
- anno_di_pubblicazione date YEAR
- genere stringa VARCHAR(15) NOTNULL
- prezzo number FLOAT (4,2) NOTNULL
- casa_videoludica  stringa VARCHAR() NULL
- disponiblità  number  TINYINT NULL DEFAULT(0)
- quantità number SMALLINT
- immagine_copertina stringa VARCHAR()  NULL
- piattaforma stringa VARCHAR NOTNULL
- sistema_operativo  stringa VARCHAR NULL
- lingua stringa VARCHAR(20) NOTNULL
- preorder number TINYINT NOTNULL DEFAULT(0)
- edizione_delux stringa number TINYINT NULL DEFAULT(0)
- data_di_rialascio DATETIME NOTNULL
<!-- /DATABSE -->