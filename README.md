# Documentație Aplicație Python/Flask

**Autor:** Marin Valentin-Gabriel 432B

---

## Introducere

Aplicația prezentată este dezvoltată utilizând Python împreună cu framework-ul Flask pentru backend și tehnologii precum HTML, CSS și Bootstrap pentru frontend. Aceasta gestionează o relație de tip N:M între două entități: clienți și posturi TV.

---

## Tehnologii utilizate

### Python și Flask:
- Framework-ul Flask a fost utilizat pentru a dezvolta backend-ul aplicației. Flask oferă o arhitectură ușor de utilizat și scalabilă pentru aplicațiile web.

### HTML, CSS și Bootstrap:
- Frontend-ul aplicației utilizează HTML și CSS pentru structură și design, iar Bootstrap a fost folosit pentru a asigura responsivitatea și un stil modern al interfeței.

### MySQL:
- Baza de date utilizată este MySQL, iar conexiunea cu aplicația Flask a fost realizată folosind biblioteca `mysql-connector`.

---

## Descrierea aplicației

Aplicația este construită pentru a gestiona relația N:M dintre două entități principale:
- **Clienți** - reprezentați prin atributele: nume, prenume și email.
- **Posturi TV** - fiecare având un nume și o descriere.

Funcționalitățile aplicației includ:
- CRUD (Create, Read, Update, Delete) pentru tabelele `clienti` și `posturitv`.
- Asocierea și dezasocierea entităților `clienti` și `posturitv` printr-o tabelă intermediară (`clienti_posturi`).

---

## Diagrama bazei de date

Diagrama bazei de date reprezintă relația N:M dintre `clienti` și `posturitv` prin intermediul tabelei `clienti_posturi`. Aceasta a fost generată utilizând MySQL Workbench și este inclusă în secțiunea următoare (poate fi accesată și prin fișierul `MySQL_Diagram.html` din folderul resurse).

---

## Structura folderului aplicației

Structura completă a proiectului va putea fi găsită în folderul `resurse`, sub denumirea de `Structura_Proiect_Python.html`.

---

## Părți importante din cod

### Funcționalitățile CRUD:

#### Listare Client:
- Afișează lista clienților existenți în baza de date. Dacă utilizatorul introduce un parametru de căutare (email), funcția va filtra rezultatele după acel email.

#### Adăugare Client:
- Permite adăugarea unui client nou în baza de date printr-un formular.

#### Editare Client:
- Permite actualizarea informațiilor unui client existent.

#### Ștergere Client:
- Șterge un client specificat din baza de date.

---

## Manual de instalare și utilizare

### Instalare Python:
1. Descărcați și instalați Python 3.9.10 de pe site-ul oficial sau din folderul resurse.
2. Rulați instalatorul și, în timpul procesului, bifați opțiunea „Add Python to PATH” pentru a adăuga Python în variabilele de mediu.
3. Continuați instalarea urmând pașii din asistentul de instalare.

### Instalare MySQL:
1. Descărcați și instalați MySQL Server 8.0.40 de pe site-ul oficial MySQL sau din folderul resurse.
2. Urmați pașii din asistentul de instalare:
   - Selectați „Server only” dacă nu aveți nevoie de alte componente MySQL.
   - Configurați serverul:
     - **Username:** Alegeți un nume de utilizator (ex.: root).
     - **Password:** Alegeți o parolă sigură.
3. Finalizați instalarea.

### Configurare MySQL:
1. Deschideți MySQL Workbench sau orice alt client MySQL.
2. Conectați-vă la server utilizând credențialele configurate în timpul instalării.
3. Creați o nouă bază de date, și importați în aceasta fișierul `db.sql` din folderul `resurse`.
4. Navigați în folderul `src` al aplicației și localizați fișierul `config.py`.
5. Deschideți fișierul și înlocuiți valorile `*****` cu datele dumneavoastră:
   - Numele bazei de date
   - Numele utilizatorului MySQL
   - Parola utilizatorului MySQL

### Rulare aplicație:
1. După ce ați verificat toți pașii de mai sus, rulați aplicația utilizând executabilul furnizat.
2. Foarte important, aplicațiile rulează pe bază de executabil, iar antivirusul s-ar putea să detecteze aplicația ca fiind un virus. Este necesar să opriți antivirusul pentru a o rula corect.

---

## Bibliografie:
- **Python Software Foundation, "Python 3.9 Documentation,"** [Online]. Available: https://docs.python.org/3.9/.
- **Flask Project, "Flask Documentation,"** [Online]. Available: https://flask.palletsprojects.com/.
- **The Bootstrap Team, "Bootstrap Documentation,"** [Online]. Available: https://getbootstrap.com/.
- **Oracle Corporation, "MySQL 8.0 Reference Manual,"** [Online]. Available: https://dev.mysql.com/doc/.
- **Oracle Corporation, "MySQL Workbench User Guide,"** [Online]. Available: https://dev.mysql.com/doc/workbench/en/.
- **IEEE, "Conference Publishing Templates,"** [Online]. Available: https://www.ieee.org/conferences/publishing/templates.html.
