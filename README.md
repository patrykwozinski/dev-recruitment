<p align="center">
  <img src="https://kinsta.com/wp-content/uploads/2017/03/wordpress-developer.png" alt="Logo"/>
</p>

<p align="center">
  "<i>I'm not a great programmer; I'm just a good programmer with great habits.</i>" ~ K. Beck
</p>

<p align="center">
<sub>
  The inspiration to create the following set of questions and answers was <a href="https://github.com/trimstray/test-your-sysadmin-skills">Test your admin skills</a> repository. The developer version has been prepared by <a href="https://github.com/patrykwozinski">@patrykwozinski</a>. Any suggestions for changes, new questions or additions of answers are very welcome.
</sub>
</p>

<br>

***

<br>

<b>Available language versions:</b>
<p>
  &nbsp;&nbsp;🇬🇧 <a href="https://github.com/patrykwozinski/dev-recruitment/blob/master/README.md">English version</a>
  <br>
  &nbsp;&nbsp;🇵🇱 <a href="https://github.com/patrykwozinski/dev-recruitment/blob/master/translations/PL.md">Polish version</a>
</p>

<br>

***

<br>

:bulb: &nbsp;Questions are only examples and initial implementation to the topic. Completely exhausting the topic is possible after searching for materials on your own.

:warning: &nbsp;Questions marked **`***`** do not have answers or they are incomplete. It is nice to see in such cases **pull requests** with the suggested problem solution.

:vertical_traffic_light: &nbsp;In a situation where you find a question that does not make much sense or contains incorrect answers - please do a pull request with suggested changes and become a project contributor.

<br>

## About the project
The project was created to support programmers who intend to go on recruitment interviews in the near future, as well as people who carry them out from the technical side.

## Recruitment questions


### 👨‍🎓 Junior Software Developer

###### PHP (1)
<details>
<summary><b>What ways of inheriting in PHP do you know?</b></summary><br>

In a PHP exists inheriting by `extends` keyword from one class. We can also inherit from many places by `Trait`.  
</details>

###### Application testing (1)
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

###### Application testing (2)

<details>
  <summary><b>What types of Test Doubles do you know?</b></summary><br>

  Dummy, Fake, Stub, Spy, Mock. They are used to plug the implementation.
</details>

<details>
  <summary><b>Do the rules related to the quality of the software also apply to tests?</b></summary><br>
  
  Yes, the quality of the tests is as important as the quality of the application. It is also worth putting a lot of effort into their proper preparation, because poor quality tests are expensive to maintain and cause many problems.
  </details>

###### Object Oriented Programming (6)

<details>
  <summary><b>Korzystasz na swoim repozytorium użytkowników z metody <code>oneByUsername(username)</code>, która ma za zadanie znaleźć użytkownika o podanym loginie. Co zrobisz w momencie, gdy nie zostaną zwrócone żadne rezultaty?</b></summary><br>
  
Najlepszą opcją jest rzucenie wyjątki, gdyż tak naprawdę nie spełniono założenia poszukiwania usera. W niższych klasach należy to odpowiednio obsłużyć. Inną opcją jest zwrócenie `null`. Odpowiedzi takie jak: pusta klasa user, pusta lista, pusty array, `false` - to błąd.
</details>
  
 <details>
  <summary><b>When is it worth to mark the class as final and how does it help?</b></summary><br>
  
 At the moment when the class is already concrete - it inherits from the abstract or implements the interface. This blocks unnecessary levels of inheritance and forces the composition.
</details> 

<details>
  <summary><b>Jakie są zalety korzystania z NullObject pattern?</b></summary><br>
  
  Jest to świetne rozwiązanie problemu walki z wszędobylskimi nullami, odpalania metod na nullach i budowy wielu zbędnych ifów.
</details>

<details>
  <summary><b>Czym jest enkapsulacja i w jaki sposób pomagają w jej utrzymaniu Value Objecty zastępujące typy proste?</b></summary><br>
  
  Ukrywają one implementacje konkretnych zachowań używających natywnych funkcji języka, nadają wyższy poziom abstrakcji. Dzięki Value Objectom jesteśmy w stanie określić konkretny stopień języka naturalnego, którym będziemy posługiwać się podczas rozwoju aplikacji.
</details>  

<details>
  <summary><b>Czy istnieje zestaw zasad, które pomagają w pisaniu poprawnego z punktu widzenia obiektowości kodu?</b></summary><br>
  
 Jednym z zestawów zasad związanych z obiektowością jest **GRASP** - General Responsibility Assignment Software Principles, który składa się z dziewięciu reguł traktujących o tym w jaki sposób projektować kod i odpowiedzieć sobie na pytania: gdzie umieścić jakąś odpowiedzialność, do kogo przypisać odpowiedzialność, jak kierować zależności i wiele innych.
</details>

<details>
  <summary><b>What types of design patterns do you know?</b></summary><br>
  
  Design patterns are divided into three types:
  - **creational patterns**
  - **structural patterns**
  - **behavioral patterns**
</details>

###### Application architecture (1)

<details>
  <summary><b>Czym jest CQRS i jakie korzyści płyną z jego wykorzystania?</b></summary><br>
  
  **Command-Query Responsibility Segregation** to podział modelu na model odczytu oraz model zapisu. Wykorzystując CQRS tworzymy komendy (`Commands`) oraz zapytania (`Queries`). Komenda nigdy nie zwraca wartości, a zapytanie nigdy nie modyfikuje danych.
</details>

<details>
  <summary><b>What is the difference between Active Records and ORM? What are the pros and cons of using these approaches? ***</b></summary><br>
  
  :warning: Missing answer. Create a pull request and become a contributor!
</details>


### 👨‍🏫 Senior Software Developer

###### Object Oriented Programming (2)

<details>
  <summary><b>What is behavior of an object?</b></summary><br>  

  Behavior of an object is a thing possible to the living creature. For example `document->reassign(owner)` - we can reassign new owner of a document. Getting and setting this information is not a behavior.
</details>

<details>
  <summary><b>Jakie są minusy dodawania prefixów metod <code>get</code> / <code>set</code> w publicznych metodach obiektów?</b></summary><br>
  
  Dodawanie prefixów takich jak `get` czy `set` blokuje nam możliwość czytania odpowiedzialności klas oraz ich cech. Gettery i settery to naleciałość, która pozostała po proceduralnym podejściu i jest nieprawidłowym nawykiem, który skutkuje wynoszeniem zbyt dużych ilości informacji na zewnątrz klasy. Publiczne metody powinny określać możliwe interakcje z obiektem oraz prezentujące jego cechy.
</details>
