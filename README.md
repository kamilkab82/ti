#Notatki do technologii internetowych

Znaczniki:

* p
* ul,ol
  *li
* img
* h


```html
<!doctype html>
<html lang=pl>
<head>
  <meta charset=utf-8>
  <title>Szablon strony HTML5</title>
    body { background: #E2DF9A; }
  </style>
</head>
<body>
  <p>ąćęłńóśźż ĄĆĘŁŃÓŚŹŻ</p>
</body>
</html>
```
jajsj jo

<b>JEZYKI   PROGRAMOWANIA</b><br><br>
<b>ZAJECIA 1<br><br>
Zad 1<br>
Wyswietl sume, różnice, iloczyn i iloraz dwóch liczb calkowitych.<br></b>
<br>
<b>Wersja 1</b><br>
pokaże  błąd przy dzieleniu, bo zadeklarowano liczby calkowite int a,b
```c
#include <stdio.h>
int main(){
 int a,b;
 a=3;
 b=7;
 printf ("%d*%d=%d\n", a,b, a*b);
 printf ("%d/%d=%d\n", a,b, a/b);
 printf ("%d+%d=%d\n", a,b, a+b);
 printf ("%d-%d=%d\n", a,b, a-b);
 getchar();
 return 0;
}
```

<b>Wersja 2</b><br>
pokaże wszystkie odpwiedzi jako zmiennoprzecinkowe np. 21.000000, bo zadeklarowano zmiennoprzecinkowe double a,b
```c
#include <stdio.h>
int main(){
 double a,b;
 a=3;
 b=7;
 printf ("%lf*%lf=%lf\n", a,b, a*b);
 printf ("%lf/%lf=%lf\n", a,b, a/b);
 printf ("%lf+%lf=%lf\n", a,b, a+b);
 printf ("%lf-%lf=%lf\n", a,b, a-b);
 getchar();
 return 0;
}
```

<b>Wersja 3</b><br>
pokaże sumę, różnicę, iloczyn jako liczby całkowite /zmiennoprzecinkowe ale z zerem miejsc po przecinku, <br>a dzielenie z miejscami po przecinku.
```c
#include <stdio.h>
int main(){
 double a,b;
 a=3;
 b=7;
 printf ("%.0lf*%.0lf=%.0lf\n", a,b, a*b);
 printf ("%lf/%lf=%lf\n", a,b, a/b);
 printf ("%.0lf+%.0lf=%.0lf\n", a,b, a+b);
 printf ("%.0lf-%.0lf=%.0lf\n", a,b, a-b);
 getchar();
 return 0;
}
```
<b><br>Zad 2<br>
Oblicz obwód kola o promieniu r<br>
<br>
Wersja 1</b><br>
z dolaczona #include <math.h>, żeby liczylo pi /jako M_PI/, czyli podstawi samodzielnie wartosć pi<br>
Poda wartosc obwodu kola wraz z obliczeniami 
```c
#include <stdio.h>
#include <math.h>
int main(){
 double r;
 int a;
 a=2;
 printf ("podaj promień okręgu %lf\n", r);
 scanf ("%lf", &r);
 printf ("%d*%lf*%lf=%lf\n", a, M_PI, r, a*M_PI*r);
 getchar();
 getchar();
 return 0;
}
```

<b>Wersja 2</b><br>
z dolaczeniem #include <math.h><br>
Poda wartosci obwodu i pola kola wraz z obliczeniami
```c
#include <stdio.h>
#include <math.h>
int main(){
 double r;
 int a;
 a=2;
 printf ("podaj promień okręgu r %lf\n", r);
 scanf ("%lf", &r);
 printf ("%d*%lf*%lf=%lf\n", a, M_PI, r, a*M_PI*r);
 printf ("%lf*%lf=%lf\n", M_PI, r*r, M_PI*r*r);
 getchar();
 getchar();
 return 0;
}
```

<b>Wersja 3</b><br>
z dolaczeniem #include <math.h><br>
Poda wartosci obwodu i pola kola wraz z obliczeniami i tekstem
```c
#include <stdio.h>
#include <math.h>
int main(){
 double r;
 int a;
 a=2;
 printf ("podaj promień okręgu r %lf\n", r);
 scanf ("%lf", &r);
 printf ("%d*%lf*%lf=%lf Obwod kola\n", a, M_PI, r, a*M_PI*r);
 printf ("%lf*%lf=%lf Pole kola\n", M_PI, r*r, M_PI*r*r);
 getchar();
 getchar();
 
 return 0;
}
```

<b>Wersja 4</b><br>
z dolaczeniem #include <math.h><br>
Poda wartosci obwodu i pola kola wraz z obliczeniami i tekstem wyswietlonym przy zastosowaniu puts <br>i podwójnego getchar do przechodzenia dalej enterem
```c
#include <stdio.h>
#include <math.h>
int main(){
 double r;
 int a;
 a=2;
 printf ("podaj promień okręgu r %lf\n", r);
 scanf ("%lf", &r);
  puts("Obwod kola");
 printf ("%d*%lf*%lf=%lf\n", a, M_PI, r, a*M_PI*r);
 getchar();
 getchar();
 puts("Pole kola");
 printf ("%lf*%lf=%lf\n", M_PI, r*r, M_PI*r*r);
 getchar();

 return 0;
}
```

<b>Wersja 5</b><br> 
z dolaczeniem #include <math.h><br>
Poda wartosci obwodu i pola kola bez widocznych obliczen, tylko wynik i tekst
```c
#include <stdio.h>
#include <math.h>
int main(){
 double r;
 int a;
 a=2;
 printf ("podaj promień okręgu r %lf\n", r);
 scanf ("%lf", &r);
 printf ("Obwod kola %lf\n", a*M_PI*r);
 getchar();
 getchar();
 printf ("Pole kola %lf\n", M_PI*r*r);
 getchar();

 return 0;
}
```

<b>Wersja 6</b><br>
z dolaczeniem #include <math.h><br>
Poda wartosci obwodu i pola kola bez widocznych obliczen, <br>tylko wynik i opis wraz z podaniem dla jakiego promienia r
```c
#include <stdio.h>
#include <math.h>
int main(){
 double r;
 int a;
 a=2;
 printf ("podaj promień okręgu r %lf\n", r);
 scanf ("%lf", &r);
 printf ("Obwod kola o promieniu %lf wynosi %lf\n", r, a*M_PI*r);
 getchar();
 getchar();
 printf ("Pole kola o promieniu %lf wynosi %lf\n", r, M_PI*r*r);
 getchar();

 return 0;
}
```
<br>
<b>Zad 3<br>
Przelicz  F na C<br>
<br>
Wersja 1</b><br>
Zastosowanie while,<br> 
Zamieni F na C w zakresie od 0F do 300F z krokiem 20F int czyli tylko wartosci cakowite
```c
#include <stdio.h>
int main(){
int fahr, celsius;
int lower, upper, step;
lower=0;
upper=300;
step=20;
fahr=lower;
while (fahr<=upper){
      celsius=5*(fahr-32)/9;
      printf("%d\t %d\n", fahr, celsius);
      fahr=fahr+step;
                     }
 getchar();

 return 0;
}
```

<b>Wersja 2</b><br>
Zastosowanie while,<br> 
Zamieni stopnie F na C od 0F do 50F ale wynik z dokladnocia do jednego miejsca po przecinku, <br>czyli używamy zmiennoprzecinkowych - zamieniamy int na double i %d na %lf

```c
#include <stdio.h>
int main(){
double fahr, celsius;
int lower, upper, step;
lower=0;
upper=50;
step=1;
fahr=lower;
while (fahr<=upper){
      celsius=5*(fahr-32)/9;
      printf("%.1lf\t %.1lf\n", fahr, celsius);
      fahr=fahr+step;
                     }
 getchar();

 return 0;
}
```

<b>Wersja 3</b><br>
Zastosowanie while,<br> 
To samo co Wersja 2, ale ladnie wyswietli wyniki przecinkami jeden pod drugim
```c
#include <stdio.h>
int main(){
double fahr, celsius;
int lower, upper, step;
lower=0;
upper=50;
step=1;
fahr=lower;
while (fahr<=upper){
      celsius=5*(fahr-32)/9;
      printf("%5.1lf\t %7.1lf\n", fahr, celsius);
      fahr=fahr+step;
                     }
 getchar();
 return 0;
}
```

<b>Wersja 4</b><br>
Zastosowanie for , #define LOWER 0 itd<br> 
Jak w Wersji 1, ale przy #define STEP 0 daje niekonczaca sie petle <br>
wywietlac bedzie zera w nieskonczonosc i żeby wyjsc to wcisnac ctrl+c<br> 
Zmiana STEP na np. 20 da normalna petle<br> 
i zamieni F na C w zakresie od 0F do 300F z krokiem 20F 
```c
#include <stdio.h>
#define LOWER 0
#define UPPER 300
#define STEP 0
int main(){
int fahr, ;
for(fahr=LOWER; fahr<=UPPER; fahr=fahr+STEP)
printf("%3d %6.1lf\n", fahr,(5.0/9.0)*(fahr-32.0));
 getchar();
 return 0;
}
```
<br>
<b>Zad 4<br>
Oblicz n-ty wyraz (Un) ciagu Fibonacciego.</b><br>
<br>
Petla do-while <br>
```c
#include <stdio.h>
int main()
{
int u1, u2, u3;/*na kolejne wyrazy ciągu*/
int n;  /*nr wyrazu*/
int i; /*licznik*/
do
  { printf ("podaj numer wyrazu (co najmniej 3): ");
   scanf ("%d", &n);
  }
  while (n<3);
  u2=u1=1; /*dwa pierwsze wyrazy*/
  i=2;
  while (i++ < n) /*dziala tylko dla n>2 i++ najpierw sdprawdza i z n potem zwieksz o jeden*/
   {u3=u1+u2;
    u1=u2;
    u2=u3;
   }
   /*inna możliwość*/
   /*for (i=3; i<=2; i++, u1=u2, u2=u3) u3=u1+u2; */
   printf ("Wyraz o numerze %d ma wartość %d" , n, u3);
 getchar(); getchar();
 return 0;
}
```

<br>
<b>Zad 5<br>
Zbuduj trojkat  - choinke zudowana ze znakow * o zadeklarowanej liczbie wierszy.</b><br> 
Petla for. 
```c
#include <stdio.h>
#define znak '*' /*znak wypelnienia*/
int main()
{
int lbwier;/*calkowita liczba wierszy*/
int lw;  /*licznik wierszy*/
int lodst; /*liczba odstepow poprzedzajacych gwiazdke*/
int j;

  printf ("ile wierszy? ");
   scanf ("%d", &lbwier);
   
   for (lw=0 ; lw<lbwier ; lw++)
   { lodst = lbwier-lw-1;
     for (j=0 ; j<lodst ; j++) putchar (' '); /* putchar-wstaw (' ')-puste miejsce*/
     for (j=0 ; j<2*lw+1 ; j++) putchar (znak); /* (znak)-wstaw * */
     putchar('\n');
   }
 getchar(); getchar();
 return 0;
}
```

<br>
<b>Zad 6 </b><br>
<i>/jest to zadanie nr 1 z kartki nr 1/</i><br>
<b>Wyswietl liczby od 0 do 23</b><br>
<br>
Wersja z petla for.
```c
#include <stdio.h>
int main()
{
int i;
i=0;
 for( i=0; i<24; i++)
 {
    printf ("%d\n", i);
 }
 getchar(); getchar();
 return 0;
}  
```

Wersja z petla while.
```c
#include <stdio.h>
int main()
{
int i;
i=0;
 while( i<24)
 {
      printf ("%d\n", i);
      i++;
 }
 getchar(); getchar();
 return 0;
}
```

Wersja z petla do-while.
```c
#include <stdio.h>
int main()
{
int i,;
i=0;
do
  { printf ("%d\n", i);
  i++;
  }
  while (i<24);
 getchar(); getchar();
 return 0;
} 
```

<br>
<b>Zad 7</b><br>
<i>/jest to zadanie nr 2 z kartki nr 1/</i><br>
<b>Wypisz liczby od - 3.5 do 7.5 z krokiem co 0.5 za pomoca petli do-while.</b><br>
Petla do-while. 
```c
#include <stdio.h>
int main()
{
double i,n;
i=-3.5;
n=7.5;
do
  { printf ("%.1lf\n", i);
  i=i+0.5;
  }
  while (i<=n);
 getchar(); getchar();
 return 0;
} 
```
bzzzzzzzzzzzz

```c

Zad . 1. Warunkowe, trójmian kwadratowy
#include <stdio.h>
#include <math.h>

int main(){
       double x1,x2,a,b,c,delta;
       printf("podaj wspolczynniki trojmianu kwadratowego\n");
       scanf("%lf %lf %lf", &a, &b, &c);  
       delta=b*b-(4*a*c);
                       if(delta<0) {
                       printf("To nie jest delta");
                                        }
                                        else {
                                         if (delta==0){
                                            x1=x2=-b/(2*a);
                                             }
                                                           else {
      
                                                           if(delta>0){
                                                           x1=(-b-sqrt(delta))/(2*a);
                                                            x2=(-b+sqrt(delta))/(2*a);
                                                            printf("miejsca zerowe to: x1=%lf, x2=%lf", x1, x2);
                                                             }
                                                               }
       }
getchar();
getchar();
return 0;
}

--------

#include <stdio.h>
#include <math.h>

int main(){
       int i , suma=0, j=0;
       for( i=1; i<=10000; i++){
            suma=0;
            for( j=1; j<i; j++)
            if (i%j==0)
            suma=suma+j;
            if(suma==i)
            printf("%d,", suma);
            
           }
getchar();
getchar();
return 0;
}
.......
#include <stdio.h>
int main(){
       int a, b,c,d=1;
       for(a=1; a<100; a++){
        for(b=a; b<100; b++){
       for(c=b; c<100; c++){
       if(a*a+b*b==c*c){
       printf("%d, %d, %d\n", a,b,c);
       d++;
       }
       if (d==20){
                 getchar();
          return 0;
       }
       }
       }
       }
       
getchar();
getchar();
return 0;
}

```html
Treść zadania 1

Napisz funkcję obliczającą pole kuli o podanym promieniu.

#include <stdio.h>
#include <math.h>

double pole(double r);

int main() {
    double r, p;
    printf("Podaj promien kuli: ");
    scanf("%lf",&r);
    p=pole(r);
    printf("\n\n Pole kola o promieniu %lf ma wartosc %lf", r, p);
    getchar();
    getchar();
    return 0;
        }   

double pole(double r) {
    double p;
    p=4*M_PI*r*r;                                                          
    return p;    
}

Treść zadania 2

Napisz funkcję warBezwzgledna zwracajaca wartość bezwzględną z liczby całkowitej.

#include <stdio.h>

int wartBezwzgledna(int x);

int main() {
    int x,y;
    puts("Podaj liczbe: ");
    scanf("%d",&x);
    y=wartBezwzgledna(x);
    printf("\n\n Wartosc bezwzgledna z %d wynosi %d", x, y);
    getchar();
    getchar();
    return 0;
        }   

int wartBezwzgledna(int x) {
    if(x<=0)
    x=-x;
    return x;    
}

Treść zadania 3

Napisz funkcję obliczającą a do potęgi n dla n należącego do N za pomocą pętli.

#include <stdio.h>
int main() {
    double a,x=1;
    int n, i;
    puts("Podaj liczbe: ");
    scanf("%lf",&a);
    puts("Podaj wykladnik (liczba naturalna): ");
    scanf("%d",&n);
    for(i=1;i<=n;i++){
    x=x*a;
}
    printf("\n\n Wartosc %lf do potegi %d wynosi %lf ", a, n, x);
    getchar();
    getchar();
    return 0;
        }

lub jako funkcja

#include <stdio.h>
double potegaAn(double a, int n);

int main() {
    double a, x;
    int n;
    puts("Podaj liczbe: ");
    scanf("%lf",&a);
    puts("Podaj wykladnik (liczba naturalna): ");
    scanf("%d",&n);
    x=potegaAn(a,n);
    printf("\n\n Wartosc %lf do potegi %d wynosi %lf ", a, n, x);
    getchar();
    getchar();
    return 0;
        }   
double potegaAn(double a, int n) {
    int i;
    double x=1.0;
    for(i=1;i<=n;i++){
    x=x*a;
}
    return x;
}

Treść zadania 4 jest zbyt skomplikowana

w skrócie - napisać funkcję, która liczy pierwiastek z liczby oraz porównuje go z pierwiastkiem z tej liczby z funkcji wbudowanej

#include <stdio.h>
#include <math.h>

double pierwA(double a);

int main() {
    double a,x,y, blad;
    puts("Podaj liczbe: ");
    scanf("%lf",&a);//Będzie liczony pierwiastek z tej liczby "a"
    x=pierwA(a);    //Pierwiastek policzony moją funkcją
    y=sqrt(a);      //Pierwiastek policzony funkcją wbudowaną sqrt
    blad=(x-y)/y;   //Błąd względny
    printf("\n\n Pierwiastek z liczby %lf wynosi %lf, \n\n a z funkcji sqrt() wynosi\
 %lf, \n\n zatem blad wzgledny wynosi %.16le", a, x, y, blad>=0 ? blad : -blad);
    getchar();
    getchar();
    return 0;
        }

double pierwA(double a) {
    double x, epsilon=1e-15;
    x=(a/2.0)+1.0;
    while((x-(a/x))>epsilon*x || (x-(a/x))<-epsilon*x) // lub fabs(x-a/x)>epsilon*x
    x=(x+(a/x))/2.0;
    return x;
    }

Treść zadania 5 (jest w formie algorytmu)

Szybkie boliczanie potęgi n-tej liczby a

#include <stdio.h>
int potegaAn(int a, int n);

int main() {
    int a, p, n;
    puts("Podaj liczbe naturalna: ");
    scanf("%d",&a);
    puts("Podaj wykladnik (liczba naturalna): ");
    scanf("%d",&n);
    p=potegaAn(a,n);
    printf("\n\n Wartosc %d do potegi %d wynosi %d ", a, n, p);
    getchar();
    getchar();
    return 0;
        }   

int potegaAn(int a, int n) {
    int i=n, p=1, q=a;
    while(i>0){
    if(i%2!=0)
    p=p*q;
    q=q*q;
    i=i/2;
}

    return p;
}

Treść zadania 6

Rozbuduj funkcję z poprzedniego zadania tak, aby funkcja działała także dla ujemnych potęg (n całkowite) i dla a będących typu double.

#include <stdio.h>
double potegaAn(double a, int n);

int main() {
    int n;
    double a, p;
    puts("Podaj liczbe: ");
    scanf("%lf",&a);
    puts("Podaj wykladnik (liczba naturalna): ");
    scanf("%d",&n);
    p=potegaAn(a,n);
    printf("\n\n Wartosc %lf do potegi %d wynosi %lf ", a, n, p);
    getchar();
    getchar();
    return 0;
        }   

double potegaAn(double a, int n) {
    int i=n, minus=0;
    double p=1.0, q=a;
           if(i<0){
           minus=1;
            i=-i;
                 }
                 while(i>0){
                      if(i%2!=0)
                      p=p*q;
                      q=q*q;
                      i=i/2;
                            }
                     if(minus==0)             
                     return p;
                     else
                     return (1.0/p);
}




