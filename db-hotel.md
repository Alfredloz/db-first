<!-- Istruzioni:
Provare a strutturare il seguente database che modellizza un hotel: Ci sono varie stanze, ognuna con le proprie caratteristiche. Le diverse stanze vengono prenotate per periodi di tempo, da ospiti. Ad ogni prenotazione devono essere associati tutti gli ospiti della stanza.
Nella repo mettete sia il file del diagramma che il file esportato come immagine. -->

<!-- database -->
# database name: Nova_Hotel_database
- Nome_albergo: id Unique
- Indirizzo_albergo: VARCHAR NOTNULL
- ORARI: TINYINT NOTNULL
- numero_di_telefono :TINYINY NOTNULL
- orario_check-in: TINYINT NOTNULL
- orario_check-out: TINYINT NOTNULL
- lingue_per_il_client: VARCHAR(50) NOTNULL
- ristorante_albergo: VARCHAR NULL default (1)
- bar_albergo: VARCHAR NULL default (1)
- parcheggio: TINYINT NOTNULL deafault (0)

# Tipi di stanze (a, b, c, d)
- ID UNIQUE AUTO_INCREMENT
- tipo_di_stanze: TINYINT NOTNULL

# Stanze A-B-C-D
- (FK from tipi_di_stanze)
- id UNIQUE AUTO_INCREMENT
- descrizione: TEXT NOTNULL
- Quantità: TINYINT NOTNULL
- fumatori: TINYINT NULL default(0)
- animali_domestici: NOTNULL 
- numeromax_ospiti: NOTNULL
- costo_per_giorno: FLOAT(6,2) NOTNULL
- disponibilità: TINYINT NOTNULL default(1)
- servizio_in_camera: VARCHAR default (1)

# Customer
- ID UNIQUE AUTON_INCREMENT
- nome_e_cognome: VARCHAR NOTNULL
- data_di_nascita: DATE NOTNULL
- e-mail: VARCHAR(20) NOTNULL
- cittadinanza: VARCHAR NOTNULL
- tipo_di_documento: VARCHAR NOTNULL
- contatto_telefonico: TINYINT NOTNULL
- indirizzo_domicilio/fatturazione: VARCHAR NOTNULL
- check-in: DATETIME NOTNULL
- check-out: DATETIME NOTNULL
- possesso_animali_domestici: TINYINT NOTNULL

<!-- /database -->

