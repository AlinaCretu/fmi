# Criptografie și securitate - Ruxandra Olimid

## Examen

- via Hoinaru Mihai

> 1. Calcule la AES (parola, chei, caractere) 
> 2. Alg lui euclid. Cu p q e. 
> 3. Hash, coliziune. 
> 4. Modelul acela cu mi, ci, Enc (...), xor. Sa scoti m indice i de acolo.

- [modele de examen](https://www.dropbox.com/s/kmridta22rlz0j9/Modele%20examen%20Cripto.zip?dl=0) de pe vremea cand examenul era de doua ore

@AlexP: eu am găsit două dintre subiecte în curs, chiar dacă a trebuit să tai o pădure ca să le am pe toate printate.

## Materiale

- [seminarii](https://www.dropbox.com/s/42c8hg3aivjzbj3/Seminarii%20Cripto%20Daya.zip?dl=0) via Dayanna Amegica
- [enunturile seminariilor](https://www.dropbox.com/s/p4jmxcyhtrmy8rq/enuturi_seminarii.zip?dl=0)
- [cursurile descarcate](https://www.dropbox.com/s/x2p2zyitgc1zfjc/cursuri_crypto.zip?dl=0)
- [site-ul cursului](http://ruxandraolimid.weebly.com/cryptography.html)
- [AES Cheat Sheet](https://www.dropbox.com/s/u4zba6qztzmmhzb/aes.docx?dl=0) pentru examen via Ștefan Postăvaru

# Criptografie și securitate - Radu Boriga

## Model Examen (mai 2017)

(1p) 1. Cifrul Vigenere.
(1p) 2. Folosind cifrul Playfair, criptați-vă primul prenume ulizând numele ca parolă.
(1p) 3. Definiți noțiunile de confuzie și difuzie.
(1p) 4. Cifrul Vernam.
(1p) 5. Calculați o cheie pentru un sistem de criptare RSA cu n = 77.
6. Considerăm schema de criptare ElGamal pentru curbe eliptice, în care:
p - număr prim mare
E - curbă eliptică peste Zp
A - un punct de ordin mare al curbei eliptice E
n - un număr aleator din Zp*
B = nA
Kpriv = {n}
Kpub = {p,E,A,B}

(1p) a) Scrieți funcțiile de criptare și decriptare corespunzătoare.
(1p) b) Demonstrați corectitudinea funcției de criptare.
(2p) c) Fie curba eliptică E:y^2 = x^3 + x + 5(mod19) peste Z19, având 15 puncte:
O, A1(0,9), A2(0,10), A3(1,8), A4(1,11), A5(3,4), A6(3,15), A7(4,4), A8(4,15), A9(11,6), A10(11,13), A11(12,4), A12(12,15), A13(13,7), A14(13,12)

Punctul A1(0,9) este un generator al grupului asocial al curbei eliptice, deoarece:
O = 15A1, A2 = 14A1, A3 = 13A1, A4 = 2A1, A5 = 3A1, A6 = 12A1, A7 = 4A1, A8 = 11A1, A9 = 6A1, A10 = 9A1, A11 = 8A1, A12 = 7A1, A13 = 10A1, A14 = 5A1

Pentru A = A5 și n=7 criptați mesajul M = A13 și decriptați mesajul M' = (A10,A6).

Se acordă 1 punct din oficiu.
