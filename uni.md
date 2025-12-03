## UNI-DB

## TABLE

- dipartimenti
- cosrsi_laurea
- corsi
- insegnanti
- corsi_insegnanti
- appelli_esami
- studenti
- appeli_studenti

## DIPARTIMENTI

- id INT PK AI
- name VARCHAR(100)

## CORSI_LAUREA

- id INT PK AI
- name VARCHAR(100)
- dipartimeno_id INT FK

## CORSI

- id INT PK AI
- name VARCHAR(100)
- corso_laurea_id INT FK

## INSEGNANTI

- id INT PK AI
- name VARCHAR(100)
- surname VARCHAR(100)

## CORSI_INSEGNANTI

- id INT PK AI
- corso_id INT FK
- insegnante INT FK

## APPELLI_ESAMI

- id INT PK AI
- corso_id INT FK
- data DATE

## STUDENTI

- id INT PK AI
- name VARCAHR(100)
- surname VARCHAR (100)
- corso_laurea_id INT FK

## APPELLI_STUDENTI

- id INT PK AI
- appello_id INT FK
- studente_id INT FK
- voto TINYINT
