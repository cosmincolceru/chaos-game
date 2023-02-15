# Chaos Game

## Membrii echipei

-   Colceru Cosmin
-   Ungureanu Dan-Andrei
-   Nistor Gheorghe

## Descriere

Chaos game este o metodă de a genera fractali cu ajutorul poligoanelor. Regulile sunt simple și vor fi explicate folosind exemplul unui triunghi cu vârfurile A, B și C. Începem cu un punct aleator P1 în interiorul triunghiului. Pentru a calcula următoarul punct P2, alegem unul dintre cele trei vârfuri ale triunghiului la întâmplare și plasăm P2 în mijlocul traseului dintre punctul P1 și vârful selectat aleator. Repetăm acest proces de un număr mare de ori și vom obține fractalul numit triunghiul lui Sierpinski, o figură descrisă pentru prima dată de matematicianul polonez Wacław Sierpiński în 1915.

![](sierpinski-triangle.png)

### Generalizare

Acest mecanism de construcție pentru fractali poate fi aplicat oricărui poligon. Cu toate acestea, dacă creștem numărul de vârfuri, nu ar trebui să mai înjumătățim distanța, ci să ajustăm ușor factorul, altfel algoritmul nu va crea întotdeauna un fractal. De exemplu, dacă înjumătățim distanța dintre poziția curentă și vârful selectat aleator al unui pătrat, obținem o zonă umplută uniform cu puncte și nu un fractal.

Distanța care trebuie folosita pentru a obiține un fractal într-un poligon cu n vârfuri poate fi calculată după formula $r=\frac{n}{n + 3}$.

### Restricții la alegerea vârfurilor

Dacă adăugam restricții la alegerea vârfurilor putem obține alte tipuri de fractali. Astfel de restricții pot fi: - un vârf nu poate fi ales de doua ori la rând - dacă un vârf a fost ales, în următoarea iterație nu putem alege unul din vecinii acelui vârf - pe lângă vârfurile poligonului, acum putem alege și mijlocurile laturilor

Adăugând astfel de restricții și modificând valoarea `r`, putem obține astfel de fractali:

![](n4r1.png)

![](n4r2.png)

![](n5r5.png)

![](sierpinski-carpet.png)

