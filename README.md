# PRIMO DB

Modellizzare la struttura di una tabella per memorizzare tutti i dati riguardanti delle auto usate messe in vendita da un concessionario

| FIELD           | TYPE        | ATTRIBUTES                                  | INDEXES     |
| --------------- | ----------- | ------------------------------------------- | ----------- |
| id              | INT         | AUTO_INCREMENT (NOT NULL, UNIQUE, UNSIGNED) | PRIMARY KEY |
| targa           | CHAR(7)     | UNIQUE, NOT_NULL                            |             |
| chilometraggio  | MEDIUMINT   | UNSIGNED, NULL                              |             |
| colore_primario | VARCHAR(20) | NULL, DEFAULT('colore base')                |             |
| venditore       | VARCHAR(80) | NULL, DEFAULT('private')                    |             |
| marca           | VARCHAR(50) | NOT_NULL                                    |             |
| modello         | VARCHAR(80) | NOT_NULL                                    |             |
