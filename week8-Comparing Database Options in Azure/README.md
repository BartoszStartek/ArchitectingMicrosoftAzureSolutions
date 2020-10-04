Opis sytuacji:
Cześć Drogi Architekcie! 
Pewnie doskonale pamiętasz o produkcie czyli Twoim e-commerce’owym rozwiązaniu.
Już miałeś okazję projektować architektury z nim związane, czas by pójść o krok dalej i rozważyć jak wykorzystać tą całą wiedzę o danych, by dobrze zaprojektować model ich składowania.

Przypomnę Ci o Twojej roli i firmie. 
Jesteś architektem w firmie, która tworzy systemy w branży e-commerce dla innych firm, które sprzedają w modelu business-to-consumer w całej Europie. Systemy budujesz w oparciu o Microsoft Azure i strategia budowania systemów Cloud Native została przyjęta i jest w pełni akceptowana przez Twoich klientów
Jako architekt możesz zdecydować zarówno o architekturze systemu jak i wzorcach, które wykorzystasz. Klienci oczekują dobrze zaprojektowanego systemu, nie wnikają w Twoje decyzje.  
System, który projektujesz, będzie odwiedzany przez klientów końcowych, a więc możesz się spodziewać, że:
1)	W wybranych godzinach będzie zarówno dużo odwiedzin strony jak i dużo zamówień
2)	System będzie miał bardzo nieprzewidywalną liczbę zamówień – zdarzą się okresy, że z systemu nikt nie będzie korzystał, ale też zdarzy się promocja typu „Black Friday”
3)	Do systemu importują swoje towary również partnerzy firmy, którzy w różnych okresach roku promują wybrane produkty
4)	System musi być jak najbardziej odporny na sytuacje awaryjne – jego podstawowa funkcjonalność, czyli sprzedaż i prezentacja ofert dla klientów powinna być dostępna „zawsze” 
A więc mam dla Ciebie wyzwanie! 

<b>Zadanie:</b>

 
<b>8.1 Przeanalizuj swoją architekturę aplikacji i zdecyduj, czy i w którym miejscu umieściłbyś wszystkie poznane typy składowania danych. </b>
 
Chciałbym być na poważnie przemyślał, jak i kiedy warto użyć Table Storage, dla jakich sytuacji dobry będzie Azure Search, gdzie przyda się Cosmos DB i jak zrobić analitykę dzięki wszystkim opcjom, które poznałeś. Rozważ DataWarehouse, HDInsights czy DataCatalog. Jeśli coś gdzieś nie pasuje, napisz o tym wprost. Decyzja musi być z głową i przemyślana. 
 
Zwróć uwagę na cenę, każdej z wybieranych usług. Może się okazać, że może zrobić coś lepiej, taniej, szybciej za pomocą innej usługi – czekam na takie propozycje. 

Dobór usług, z perspektywy kosztów to ważny element w pracy architekta dlatego musisz nabrać tutaj wprawy.
 
<b>8.2 Czas na praktykę!</b><br>
Powołaj najmniejszą z możliwych bazę Cosmos DB. Następnie spróbuj wykorzystać tzw. Change Feed a więc możliwość wyzwalania funkcji w reakcji na zmieniające się dane. 
 
