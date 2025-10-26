#  Eksploracyjna analiza zaangażowania użytkowników w mediach społecznościowych: 

# Twitter, Instagram, Tiktok, Youtube 
## 1) Wstęp 
Wzrost znaczenia mediów społecznościowych zrewolucjonizował sposób komunikacji. W niniejszej analizie badamy zbiór danych, który wyjaśnia zaangażowanie na kluczowych platformach. Analiza została przeprowadzona w programie SPSS.  
 
## 2) Cel badania 
Celem analizy jest zbadanie, które cechy postów w mediach społecznościowych wpływają na poziom zaangażowania użytkowników (mierzonego przez liczby: polubień, udostępnień i komentarzy). Analiza ma charakter eksploracyjny, czyli rozpoznanie wzorców i zależności w danych. 
 
## 3) Baza danych  
Zmienne nominalne: 
•	Platform (np. TikTok, Instagram) 

•	Hashtag (np. #Challenge, #Education)

•	Content_type (np. Video, Shorts, Post) 
 
Zmienne ciągłe: 
•	Views (liczba wyświetleń) 

•	Likes (liczba polubień) 

•	Shares (liczba udostępnień) 

•	Comments (liczba komentarzy) 
  
## 4) Analiza braków danych i wybór metody imputacji 
<img width="588" height="300" alt="wykresd1" src="https://github.com/user-attachments/assets/ce13f265-3412-4238-9b8e-5b3dbbba3636" />

W pierwszym etapie przeprowadzono diagnozę braków danych. Zidentyfikowano braki jedynie w zmiennych ilościowych.  
 
Na nich będziemy przeprowadzać analizę braków danych. Na początku sprawdzając czy braki danych w zbiorze są typy MCAR.  
MCAR test: Chi-kwadrat = 37.792, DF = 24, Istotnosc = 0.036

Na podstawie testu Little’a służący do weryfikacji hipotezy o braku MCAR. Odrzucamy hipotezę zerowa o losowości braków. Zatem braki danych nie są całkowicie losowe (MCAR). 
 
Nie możemy zastąpić brakującej wartości średnia, ponieważ mamy dane które nie są typu MCAR. W związku z tym zastosowano imputację średnią z grup.  
 

## 5. Wykorzystanie metody k-średnich  
X1 – Views;
X2 – Likes;
X3 – Shares;
X4 - Comments 

Wartości współczynnika zmienności (CV) dla analizowanych zmiennych (Views, Likes, Shares, Comments) przekraczają 90%, co świadczy o bardzo dużym zróżnicowaniu danych. Taka wysoka zmienność oznacza, że poszczególne obserwacje (posty) różnią się istotnie pod względem zasięgu oraz zaangażowania użytkowników. 
 
Wysoki poziom współczynnika zmienności stanowi uzasadnienie dla zastosowania analizy skupień, ponieważ wskazuje na możliwość wyodrębnienia jednorodnych wewnętrznie i zróżnicowanych między sobą grup. Wyraźna różnorodność sugeruje istnienie odmiennych typów postów, co umożliwia sensowne grupowanie przy użyciu metody k-średnich. 
 
Analizując korelacje pomiędzy czterema zmiennymi, możemy zastosować je do analizy skupień, ponieważ nie ma współliniowości. 
 
Wartości przekątnej macierzy odwrotnej nie przekraczają 10, oscylują około wartości 1.
![image](https://github.com/user-attachments/assets/d7be26a4-60e6-4d52-bc6b-499244f9765f)

![image](https://github.com/user-attachments/assets/1752ca15-6b3c-46f8-a25a-94b3cf0e16b0)

## 7. Analiza odpowiedniej liczby skupień
![image](https://github.com/user-attachments/assets/a282eabe-5ae0-4d31-af44-9121dd0a7086)

Na podstawie wykresu łokcia optymalna liczba skupień to 3, ponieważ właśnie przy tej liczbie następuje wyraźne załamanie krzywe dalsze zwiększanie liczby klastrów powoduje już tylko niewielki spadek błędu, co oznacza malejące korzyści z dodawania kolejnych skupień. 
Obiekty (posty) zostały podzielone na 3 skupienia na podstawie zmiennych: Views, Likes, Shares, Comments. 


![image](https://github.com/user-attachments/assets/1bff4447-f31a-4ad7-96b6-0d78850a3750)

Skupienie 1: Posty popularne – mają bardzo wysokie wyświetlenia i polubienia, ale przeciętne udostępnienia i komentarze.

Skupienie 2: Posty viralowe/kontrowersyjne – mają bardzo wysokie udostępnienia i komentarze przy niskich polubieniach; silnie angażują odbiorców.

Skupienie 3: Posty mało popularne – mają niskie wyniki we wszystkich wskaźnikach (wyświetlenia, polubienia, udostępnienia, komentarze).

## 8. Profilowanie uzyskanych skupień 

ZX1: Views (Wyświetlenia)
ZX2: Likes (Polubienia)
ZX3: Shares (Udostępnienia)
ZX4: Comments (Komentarze)

![image](https://github.com/user-attachments/assets/51832a5d-5e11-4f84-9ec2-edbea0f5f6da)
![image](https://github.com/user-attachments/assets/66e378fb-e7c4-40f9-b52a-2d0eadd48c55)
![image](https://github.com/user-attachments/assets/89e9ee0a-eba1-4241-82df-b023ca0b6e93)




1. Skupienie 1 (26 postów) - "Gwiazdy"

Platforma: Głównie Twitter i YouTube

Tematyka: Różnorodna (#Challenge, #Comedy, #Fitness, #Gaming)

Formaty: Mieszanka - live, posty, tweety, shortsy

Charakter: Posty o wysokim zasięgu i polubieniach, ale umiarkowanym zaangażowaniu

2. Skupienie 2 (14 postów) - "Prowokatorzy"

Platforma: Równomierny rozkład (głównie YouTube, TikTok)

Tematyka: Głównie komedia i edukacja

Formaty: Dominują krótkie filmy (Shorts, Reel)

Charakter: Mało polubień, ale dużo udostępnień i komentarzy - wywołują dyskusje

3. Skupienie 3 (57 postów) - "Cichy Tłum"

Platforma: Wszystkie platformy (najwięcej YouTube, Twitter)

Tematyka: Różnorodna bez wyraźnego skupienia

Formaty: Wszystkie typy treści

Charakter: Niskie wyniki we wszystkich wskaźnikach - typowe posty bez dużego odzewu

## Wnioski:

Analiza pokazuje, że skuteczność postów zależy od połączenia platformy, formatu i tematyki. "Gwiazdy" działają na Twitterze/YouTube, "Prowokatorzy" wykorzystują krótkie filmy o kontrowersyjnych tematach, a większość treści po prostu nie zdobywa znaczącej popularności.


