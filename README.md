# Database-Management-System


PROIECT  <br />
Cerințe obligatorii pentru a lua în considerare proiectul: <br />
1. Prezentați pe scurt baza de date (utilitatea ei). <br />
2. Realizați diagrama entitate-relație (ERD). <br />
3. Pornind de la diagrama entitate-relație realizați diagrama conceptuală a modelului propus, integrând toate atributele necesare. <br />
4. Implementați în Oracle diagrama conceptuală realizată: definiți toate tabelele, implementând toate constrângerile de integritate necesare <br />
5. Adăugați informații coerente în tabelele create (minim 5 înregistrări pentru fiecare entitate independentă; minim 10 înregistrări pentru tabela asociativă). <br />
6. Formulați în limbaj natural o problemă pe care să o rezolvați folosind un subprogram stocat independent care să utilizeze două tipuri diferite de colecții  <br />
studiate. Apelați subprogramul. <br />
7. Formulați în limbaj natural o problemă pe care să o rezolvați folosind un subprogram stocat independent care să utilizeze 2 tipuri diferite de cursoare <br />
studiate, unul dintre acestea fiind cursor parametrizat. Apelați subprogramul. <br />
8. Formulați în limbaj natural o problemă pe care să o rezolvați folosind un subprogram stocat independent de tip funcție care să utilizeze într-o singură <br />
comandă SQL 3 dintre tabelele definite. Definiți minim 2 excepții. Apelați subprogramul astfel încât să evidențiați toate cazurile tratate. <br />
9. Formulați în limbaj natural o problemă pe care să o rezolvați folosind un subprogram stocat independent de tip procedură care să utilizeze într-o <br />
singură comandă SQL 5 dintre tabelele definite. Tratați toate excepțiile care pot apărea, incluzând excepțiile NO_DATA_FOUND și TOO_MANY_ROWS. <br />
Apelați subprogramul astfel încât să evidențiați toate cazurile tratate. <br />
10. Definiți un trigger de tip LMD la nivel de comandă. Declanșați trigger-ul. <br />
11. Definiți un trigger de tip LMD la nivel de linie. Declanșați trigger-ul. <br />
12. Definiți un trigger de tip LDD. Declanșați trigger-ul. <br />
Cerințe opționale pentru nota finală N >= 6: <br />
13. Definiți un pachet care să conțină toate obiectele definite în cadrul proiectului. <br />
14. Definiți un pachet care să includă tipuri de date complexe și obiecte necesare unui flux de acțiuni integrate, specifice  <br />
bazei de date definite (minim 2 tipuri de date, minim 2 funcții, minim 2 proceduri) <br />
<br />
TEMA 4<br />
Mențineți într-o colecție codurile celor mai prost plătiți 5 angajați care nu câștigă comision. Folosind această colecție măriți cu 5% salariul <br />
acestor angajați. Afișați valoarea veche a salariului, respectiv valoarea nouă a salariului <br />
<br />
TEMA 5 <br />
2. Definiți un tip colecție denumit tip_orase_***. Creați tabelul excursie_*** cu următoarea structură: <br />
cod_excursie NUMBER(4), denumire VARCHAR2(20), orase tip_orase_*** (ce va conține lista orașelor care se vizitează într-o excursie, într-o ordine stabilită;<br />
de exemplu, primul oraș din listă va fi primul oraș vizitat), status (disponibilă sau anulată). <br />
a. Inserați 5 înregistrări în tabel. <br />
b. Actualizați coloana orase pentru o excursie specificată: <br />
- adăugați un oraș nou în listă, ce va fi ultimul vizitat în excursia respectivă; <br />
- adăugați un oraș nou în listă, ce va fi al doilea oraș vizitat în excursia respectivă; <br />
- inversați ordinea de vizitare a două dintre orașe al căror nume este specificat; <br />
- eliminați din listă un oraș al cărui nume este specificat. <br />
c. Pentru o excursie al cărui cod este dat, afișați numărul de orașe vizitate, respectiv numele orașelor. <br />
d. Pentru fiecare excursie afișați lista orașelor vizitate. <br />
e. Anulați excursiile cu cele mai puține orașe vizitate. <br />
3. Rezolvați problema anterioară folosind un alt tip de colecție studiat. <br />
<br />
TEMA 7 <br />
1. Pentru fiecare job (titlu – care va fi afișat o singură dată) obțineți lista angajaților (nume și salariu) care lucrează în prezent pe jobul respectiv.<br />
Tratați cazul în care nu există angajați care să lucreze în prezent pe un anumit job. Rezolvați problema folosind: <br /> 
2. Modificați exercițiul anterior astfel încât să obțineți și următoarele informații: <br />
- un număr de ordine pentru fiecare angajat care va fi resetat pentru fiecare job <br />
- pentru fiecare job <br />
o numărul de angajați <br />
o valoarea lunară a veniturilor angajaților <br />
o valoarea medie a veniturilor angajaților <br />
- indiferent job <br />
o numărul total de angajați <br />
o valoarea totală lunară a veniturilor angajaților <br />
o valoarea medie a veniturilor angajaților <br />
3. Modificați exercițiul anterior astfel încât să obțineți suma totală alocată lunar pentru plata salariilor și a comisioanelor tuturor angajaților,<br />
iar pentru fiecare angajat cât la sută din această sumă câștigă lunar. <br />
4. Modificați exercițiul anterior astfel încât să obțineți pentru fiecare job primii 5 angajați care câștigă cel mai mare salariu lunar. <br />
Specificați dacă pentru un job sunt mai puțin de 5 angajați. <br />
<br />
TEMA 8 <br />
1. Creați tabelul info_*** cu următoarele coloane: <br />
- utilizator (numele utilizatorului care a inițiat o comandă) <br />
- data (data și timpul la care utilizatorul a inițiat comanda) <br />
- comanda (comanda care a fost inițiată de utilizatorul respectiv) <br />
- nr_linii (numărul de linii selectate/modificate de comandă) <br />
- eroare (un mesaj pentru excepții). <br />
2. Modificați funcția definită la exercițiul 2, respectiv procedura definită la exercițiul 4 astfel încât <br />
să determine inserarea în tabelul info_*** a informațiile corespunzătoare fiecărui caz determinat de valoarea dată pentru parametru: <br />
- există un singur angajat cu numele specificat; <br />
- există mai mulți angajați cu numele specificat; <br />
- nu există angajați cu numele specificat. <br />
3. Definiți o funcție stocată care determină numărul de angajați care au avut cel puțin 2 joburi diferite și care în prezent lucrează într-un oraș dat <br />
ca parametru. Tratați cazul în care orașul dat ca parametru nu există, respectiv cazul în care în orașul dat nu lucrează niciun angajat. Inserați <br />
în tabelul info_*** informațiile corespunzătoare fiecărui caz determinat de valoarea dată pentru parametru. <br />
4. Definiți o procedură stocată care mărește cu 10% salariile tuturor angajaților conduși direct sau indirect de către un manager al cărui cod este dat <br />
ca parametru. Tratați cazul în care nu există niciun manager cu codul dat. Inserați în tabelul info_*** informațiile corespunzătoare fiecărui <br />
caz determinat de valoarea dată pentru parametru. <br />
5. Definiți un subprogram care obține pentru fiecare nume de departament ziua din săptămână în care au fost angajate cele mai multe persoane, <br />
lista cu numele acestora, vechimea și venitul lor lunar. Afișați mesaje corespunzătoare următoarelor cazuri: <br />
- într-un departament nu lucrează niciun angajat; <br />
- într-o zi din săptămână nu a fost nimeni angajat. <br />
Observații: <br />
a. Numele departamentului și ziua apar o singură dată în rezultat. <br />
b. Rezolvați problema în două variante, după cum se ține cont sau nu de istoricul joburilor angajaților. <br />
<br />
TEMA 9 <br /> 
1. Definiţi un pachet care să permită gestiunea angajaţilor companiei. Pachetul va conţine: <br /> 
a. o procedură care determină adăugarea unui angajat, dându-se informaţii complete despre acesta: <br /> 
- codul angajatului va fi generat automat utilizându-se o secvenţă; <br /> 
- informaţiile personale vor fi date ca parametrii (nume, prenume, telefon, email); <br /> 
- data angajării va fi data curentă; <br /> 
- salariul va fi cel mai mic salariu din departamentul respectiv, pentru jobul respectiv (se vor obţine cu ajutorul unei funcţii stocate în pachet); <br /> 
- nu va avea comision; <br /> 
- codul managerului se va obţine cu ajutorul unei funcţii stocate în pachet care va avea ca parametrii numele şi prenumele managerului); <br /> 
- codul departamentului va fi obţinut cu ajutorul unei funcţii stocate în pachet, dându-se ca parametru numele acestuia; <br /> 
- codul jobului va fi obţinut cu ajutorul unei funcţii stocate în pachet, dându-se ca parametru numele acesteia. <br /> 
Observaţie: Trataţi toate excepţiile. <br /> 
b. o procedură care determină mutarea în alt departament a unui angajat (se dau ca parametrii numele şi prenumele angajatului, respectiv numele <br /> 
departamentului, numele jobului şi numele şi prenumele managerului acestuia): <br /> 
- se vor actualiza informaţiile angajatului: <br /> 
- codul de departament (se va obţine cu ajutorul funcţiei corespunzătoare definită la punctul a); <br /> 
- codul jobului (se va obţine cu ajutorul funcţiei corespunzătoare definită la punctul a); <br /> 
- codul managerului (se va obţine cu ajutorul funcţiei corespunzătoare definită la punctul a); <br /> 
- salariul va fi cel mai mic salariu din noul departament, pentru noul job dacă acesta este mai mare decât salariul curent; altfel se va păstra salariul curent;<br /> 
- comisionul va fi cel mai mic comision din acel departament, pentru acel job; <br /> 
- data angajării va fi data curentă; <br /> 
- se vor înregistra informaţii corespunzătoare în istoricul joburilor. <br /> 
Observaţie: Trataţi toate excepţiile. <br /> 
c. o funcţie care întoarce numărul de subalterni direcţi sau indirecţi ai unui angajat al cărui nume şi prenume sunt date ca parametrii; <br /> 
Observaţie: Trataţi toate excepţiile. <br /> 
d. o procedură care determină promovarea unui angajat pe o treaptă imediat superioară în departamentul său; propuneţi o variantă de restructurare a <br /> 
arborelui care implementează ierarhia subaltern – şef din companie; Observaţie: Trataţi toate excepţiile. <br /> 
e. o procedură prin care se actualizează cu o valoare dată ca parametru salariul unui angajat al cărui nume este dat ca parametru: <br /> 
- se va verifica dacă valoarea dată pentru salariu respectă limitele impuse pentru acel job; <br /> 
- dacă sunt mai mulţi angajaţi care au acelaşi nume, atunci se va afişa un mesaj corespunzător şi de asemenea se va afişa lista acestora; <br /> 
- dacă nu există angajaţi cu numele dat, atunci se va afişa un mesaj corespunzător; <br /> 
f. un cursor care obţine lista angajaţilor care lucrează pe un job al cărui cod este dat ca parametru; <br /> 
g. un cursor care obţine lista tuturor joburilor din companie; <br /> 
h. o procedură care utilizează cele două cursoare definite anterior şi obţine pentru fiecare job numele acestuia şi lista angajaţilor care lucrează<br /> 
în prezent pe acel job; în plus, pentru fiecare angajat să se specifice dacă în trecut a mai avut sau nu jobul respectiv.<br /> 
