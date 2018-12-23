# OOP? A komu to potrzebne?
<p align="center">
  "<i>I'm not a great programmer; I'm just a good programmer with great habits.</i>" ~ K. Beck
</p>

<p align="center">
Inspiracją było repozytorium <a href="https://github.com/trimstray/test-your-sysadmin-skills">Test your admin skills</a>. Wersja dla developerów została utworzona przez: <a href="https://github.com/patrykwozinski">@patrykwozinski</a>.
</p>

<hr>

## O projekcie
Projekt został utworzony, aby wesprzeć programistów mających zamiar wybrać się w najbliższym czasie na rozmowy rekrutacyjne, a także osoby, które je przeprowadzają od strony technicznej.


## Pytania miękkie
...

## Wiedza ogólna

### 👨‍🚀 Junior Software Developer

<details>
<summary><b>Jakie znasz sposoby dziedziczenia w PHP?</b></summary><br>

W PHP istnieje możliwość dziedziczenia poprzez słowo kluczowe `extends` z jednej klasy, oraz dziedziczenia z wielu miejsc poprzez `Trait`.
  
</details>

### 👨‍🚀 Regular Software Developer

<details>
  <summary><b>Czy znasz jakieś przykłady Test Double?</b></summary><br>

  Dummy, Fake, Stub, Spy, Mock. Służą do zaślepiania implementacji.

</details>

<details>
  <summary><b>Korzystasz na swoim repozytorium użytkowników z metody oneByUsername(username), która ma za zadanie znaleźć użytkownika o podanym loginie. Co zrobisz w momencie, gdy nie zostaną zwrócone żadne rezultaty?</b></summary><br>
  
Najlepszą opcją jest rzucenie wyjątki, gdyż tak naprawdę nie spełniono założenia poszukiwania usera. W niższych klasach należy to odpowiednio obsłużyć. Inną opcją jest zwrócenie `null`. Odpowiedzi takie jak: pusta klasa user, pusta lista, pusty array, `false` - to błąd.
  
</details>

<details>
  <summary><b>Czy zasady związane z jakością oprogramowania dotyczą również testów?</b></summary><br>
  
  Tak, jakość testów jest równie ważna jak jakość aplikacji. Także warto włożyć wiele starań w ich odpowiednie przygotowanie, gdyż testy słabej jakości są drogie w utrzymaniu i powodują wiele problemów.
  
  </details>
  
 <details>
  <summary><b>Kiedy warto oznaczyć klasę jako finalną i w czym to pomaga?</b></summary><br>
  
  W momencie, gdy klasa jest już konkretną - dziedziczy po abstract lub implementuje interfejs. Blokuje to zbędne poziomy dziedziczenia i wymusza kompozycję.
  
</details> 

<details>
  <summary><b>Czym jest CQRS i jakie korzyści płyną z jego wykorzystania?</b></summary><br>
  
  **Command-Query Responsibility Segregation** to podział modelu na model odczytu oraz model zapisu. Wykorzystując CQRS tworzymy komendy (`Commands`) oraz zapytania (`Queries`). Komenda nigdy nie zwraca wartości, a zapytanie nigdy nie modyfikuje danych.
</details>

### 👨‍🚀 Senior Software Developer

<details>
  <summary><b>Czym jest zachowanie obiektu?</b></summary><br>
  
  Zachowaniem obiektu nie jest setowanie wartości, ale jest nim przykładowo `document->reassign(owner)` <- czyli coś, co mogłoby stać się z żywym obiektem.
  
</details>
