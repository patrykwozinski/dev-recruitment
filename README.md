<p align="center">
  <img src="https://kinsta.com/wp-content/uploads/2017/03/wordpress-developer.png" alt="Logo"/>
</p>

<p align="center">
  "<i>I'm not a great programmer; I'm just a good programmer with great habits.</i>" ~ K. Beck
</p>

<p align="center">
Inspiracją było repozytorium <a href="https://github.com/trimstray/test-your-sysadmin-skills">Test your admin skills</a>. Wersja dla developerów została utworzona przez: <a href="https://github.com/patrykwozinski">@patrykwozinski</a>. Wszelkie wspieranie projektu i dodawanie sugestii bardzo miło widziane.
</p>

<br>

***

<br>

## O projekcie
Projekt został utworzony, aby wesprzeć programistów mających zamiar wybrać się w najbliższym czasie na rozmowy rekrutacyjne, a także osoby, które je przeprowadzają od strony technicznej.


## Pytania rekrutacyjne


### 👨‍🎓 Junior Software Developer

###### PHP (1)
<details>
<summary><b>Jakie znasz sposoby dziedziczenia w PHP?</b></summary><br>

W PHP istnieje możliwość dziedziczenia poprzez słowo kluczowe `extends` z jednej klasy, oraz dziedziczenia z wielu miejsc poprzez `Trait`.
  
</details>

###### Testowanie aplikacji (1)
<details>
  <summary><b>Jaka jest różnica pomiędzy <code>setUp()</code> i <code>setUpBeforeClass()</code> w testach?</b></summary><br>
  
  - `setUp()` jest to metoda odpalana przed każdym kolejnym testem, po nim zaś wywoływane jest `tearDown()`
  - `setUpBeforeClass()` to metoda, która wywoływana jest przed wszystkimi testami z danej klasy testowej i po przejściu wszystkich testów uruchamiane jest `tearDownAfterClass()`
</details>


### 👨‍💻 Regular Software Developer

###### PHP (1)

<details>
  <summary><b>Czy znasz jakiś przykład, gdzie można zastosować klasy anonimowe w PHP?</b></summary><br>
  
  Świetnym miejscem do klas anonimowych są Stuby i inne test double gdzie nie interesuje nas to, jaki obiekt jest zwracany, a potrzebujemy bardzo łatwą jego implementację. Przykładowo `StubRepository` implementujący interfejs konkretnego repozytorium zależnie od tego, co przesyła nam w argumencie test, może budować odpowiednią klasę anonimową i ją zwracać.
</details>

###### Testowanie aplikacji (2)

<details>
  <summary><b>Czy znasz jakieś przykłady Test Double?</b></summary><br>

  Dummy, Fake, Stub, Spy, Mock. Służą do zaślepiania implementacji.
</details>

<details>
  <summary><b>Czy zasady związane z jakością oprogramowania dotyczą również testów?</b></summary><br>
  
  Tak, jakość testów jest równie ważna jak jakość aplikacji. Także warto włożyć wiele starań w ich odpowiednie przygotowanie, gdyż testy słabej jakości są drogie w utrzymaniu i powodują wiele problemów.
  </details>

###### Object Oriented Programming (5)

<details>
  <summary><b>Korzystasz na swoim repozytorium użytkowników z metody oneByUsername(username), która ma za zadanie znaleźć użytkownika o podanym loginie. Co zrobisz w momencie, gdy nie zostaną zwrócone żadne rezultaty?</b></summary><br>
  
Najlepszą opcją jest rzucenie wyjątki, gdyż tak naprawdę nie spełniono założenia poszukiwania usera. W niższych klasach należy to odpowiednio obsłużyć. Inną opcją jest zwrócenie `null`. Odpowiedzi takie jak: pusta klasa user, pusta lista, pusty array, `false` - to błąd.
</details>
  
 <details>
  <summary><b>Kiedy warto oznaczyć klasę jako finalną i w czym to pomaga?</b></summary><br>
  
  W momencie, gdy klasa jest już konkretną - dziedziczy po abstract lub implementuje interfejs. Blokuje to zbędne poziomy dziedziczenia i wymusza kompozycję.
</details> 

<details>
  <summary><b>Jakie są zalety korzystania z NullObject pattern?</b></summary><br>
  
  Jest to świetne rozwiązanie problemu walki z wszędobylskimi nullami, odpalania metod na nullach i budowy wielu zbędnych ifów.
</details>

<details>
  <summary><b>Czym jest enkapsulacja i w jaki sposób pomagają w jej utrzymaniu Value Objecty zastępujące typy proste?</b></summary><br>
  
  Ukrywają one implementacje konkretnych zachowań używających natywnych funkcji języka, nadają wyższy poziom abstrakcji.
</details>  

<details>
  <summary><b>Czy istnieje zestaw zasad, które pomagają w pisaniu poprawnego z punktu widzenia obiektowości kodu?</b></summary><br>
  
 Jednym z zestawów zasad związanych z obiektowością jest **GRASP** - General Responsibility Assignment Software Principles, który składa się z dziewięciu reguł traktujących o tym w jaki sposób projektować kod i odpowiedzieć sobie na pytania: gdzie umieścić jakąś odpowiedzialność, do kogo przypisać odpowiedzialność, jak kierować zależności i wiele innych.
</details>

###### Architektura aplikacji (1)

<details>
  <summary><b>Czym jest CQRS i jakie korzyści płyną z jego wykorzystania?</b></summary><br>
  
  **Command-Query Responsibility Segregation** to podział modelu na model odczytu oraz model zapisu. Wykorzystując CQRS tworzymy komendy (`Commands`) oraz zapytania (`Queries`). Komenda nigdy nie zwraca wartości, a zapytanie nigdy nie modyfikuje danych.
</details>


### 👨‍🏫 Senior Software Developer

###### Object Oriented Programming (1)

<details>
  <summary><b>Czym jest zachowanie obiektu?</b></summary><br>
  
  Zachowaniem obiektu nie jest setowanie wartości, ale jest nim przykładowo `document->reassign(owner)` <- czyli coś, co mogłoby stać się z żywym obiektem.
</details>
