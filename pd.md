# Programare Declarativă - Traian Șerbănuță

* pregătire pentru examen 07.09.2015 via Mihai Anonim - https://www.dropbox.com/sh/o1f61y4pe773dx0/AADyhb5NHX_jZ1T2BiNzlt-qa?dl=0

Niste materiale pentru examen si pentru laborator se gasesc si [aici](https://github.com/Vlaaaaaaad/FMI-public-materials/tree/master/ProgramareDeclarativa).

### Model Test 2

(2p) 1. Se dau următoarele structuri de date:
data Stack a = NilStack                 data Queue a = NilQueue
             |Stiva a (Stack a)                      |Coada a (Queue a)
                deriving (Show)                         deriving (Show)

Să se implementeze următoarele funcții:
emptyStack :: Stack a                           emptyQueue :: Queue a
pushStack :: a -> Stack a -> Stack a            pushQueue :: a -> Queue a -> Queue a
popStack :: Stack a -> Maybe (a, Stack a)       popQueue :: Queue a -> Maybe (a, Queue a)

Unde:
empty* returnează structura de date goală
push* adaugă un element la structura de date respectivă
pop* returnează elementul din structura de date respectivă și noua structură, dacă se poate; în caz de eroare se returnează Nothing

(2p) 2. Să se scrie o funcție care primește ca argumente 3 cozi (dintre care 1 conține elemente, celelalte fiind vide), și returnează o coadă având elementele din prima coadă inversate ca poziții (practic se simulează o stivă folosind 2 cozi).
simulateStack :: Queue a -> Queue a -> Queue a -> Queue a
Ex: simulateStack(pushQueue 3 (pushQueue 2 (pushQueue 1 emptyQueue))) NilQueue
NilQueue == Coada 3 (Coada2 (Coada 1 NilQueue))

(1p) 3. a) Să se scrie o funcție care primește ca argumente 2 stive (prima conține elemente, a doua este vidă) și returnează prima stivă cu elementele inversate.
rev :: Stack a -> Stack a -> Stack a
Ex: rev (Stiva 3 (Striva 2 (Stiva 1 NilStack))) NilStack == Stiva 1 (Stiva 2 (Stiva 3 NilStack))

(1p) 3. b) Să se scrie o funcție care primește o pereche (Queue a, Stack a), și verifică dacă coada conține aceleași elemente ca stiva, dacă le scoatem 1 câte 1.
Ex: verifica (pushQueue 2 $ pushQueue 3 $ emptyQueue, pushStack 3 $ pushStack 2 $ emptyStack) == True

(2p) 4. Să se simuleze o coadă folosind 2 stive
spushQueue :: a -> (Stack a, Stack a) -> (Stack a, Stack a)
spopQueue :: (Stack a, Stack a) -> (a, (Stack a, Stack a))

(2p) 5. Să se citească de la tastatură un șir de caractere și să se inverseze folosind funcțiile de mai sus.
(Notare: 2p - folosind funcția simulateStack, 1p - folosind stiva, 0.5p - folosind alte funcții)
