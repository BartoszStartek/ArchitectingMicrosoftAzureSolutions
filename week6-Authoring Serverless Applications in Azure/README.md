<b>Opis sytuacji:</b><br/>
Pamiętasz zadanie z początku kursu? Wracamy do naszego systemu e-commerce i projektowania aplikacji Cloud Native.<br/>
Przypomnę Ci o Twojej roli i firmie.<br/>
Jesteś architektem w firmie, która tworzy systemy w branży e-commerce dla innych firm, które sprzedają w modelu business-to-consumer w całej Europie. Systemy budujesz w oparciu o Microsoft Azure i strategia budowania systemów Cloud Native została przyjęta i jest w pełni akceptowana przez Twoich klientów
Jako architekt możesz zdecydować zarówno o architekturze systemu jak i wzorcach, które wykorzystasz. Klienci oczekują dobrze zaprojektowanego systemu, nie wnikają w Twoje decyzje.  
System, który projektujesz, będzie odwiedzany przez klientów końcowych, a więc możesz się spodziewać, że:<br/>
1)	W wybranych godzinach będzie zarówno dużo odwiedzin strony jak i dużo zamówień<br/>
2)	System będzie miał bardzo nieprzewidywalną liczbę zamówień – zdarzą się okresy, że z systemu nikt nie będzie korzystał, ale też zdarzy się promocja typu „Black Friday”<br/>
3)	Do systemu importują swoje towary również partnerzy firmy, którzy w różnych okresach roku promują wybrane produkty<br/>
4)	System musi być jak najbardziej odporny na sytuacje awaryjne – jego podstawowa funkcjonalność, czyli sprzedaż i prezentacja ofert dla klientów powinna być dostępna „zawsze”<br/>
Tym razem chcemy faktycznie zbudować aplikację Cloud Native i najchętniej tak zbudować system by jak najmniej zarządzać serwerami. (pamiętasz? Serverless – Manage Your Servers Less 🙂)
<br/><b>Zadanie:</b><br/>
#6.1<br/>	Wybierz 3 moduły / kawałki systemu (dowolne) może być np. System rezerwacji produktów u poddostawców, system płatności, system rezerwacji produktów w magazynie, system przetwarzania zdjęć produktów, w których wykorzystałbyś rozwiązania typu Azure Web App, Azure API Management oraz Azure Functions. Opisz ten kawałek rozwiązania (rysunki mile widziane) i min 3 punkty przy każdym wybranym module / kawałku systemu, dlaczego to jest dobry wybór.<br/>
#6.2<br/>	Wybierz min. 2 przykłady, w których użycie tych rozwiązań nie jest możliwe i wolisz / musisz zostać przy klasycznej maszynie wirtualnej. Napisz mi 2-3 powody, dlaczego na pewno nie da się tego zrobić.<br/>
#6.3<br/>	Jeśli masz już dość myślenia i planowania i nie możesz doczekać się by coś zrobić praktycznie to zadanie nr 3 jest dla Ciebie  Chciałbym byś połączył kilka komponentów za sobą a przy tym nie wydał strasznej ilość budżetu. Język pisania dowolny<br/>
<b>Opis zadania:</b><br/> 
-Stwórz prostą funkcję, opartą o timer, która dodaje wiadomości do kolejki typu Storage Queue. <br/>
-Stwórz drugą funkcję, która czeka na wiadomości w Storage Queue i zapisuje jej do bazy. <br/>
-Stwórz trzecią funkcję, która reaguje na request http i dla podanej w parametrze daty zwraca pewną wartość.<br/>
-Stwórz Azure API Management (kiedy będziesz miał już wszystkie inne elementy gotowe) i wystaw na Azure API Management funkcję z zadania nr 3. Dodatkowo, dodaj do wywołania tej funkcji politykę, która nie pozwala jej wywołać częściej w minucie niż trzy razy <br/>
Have fun! To zadanie pokaże Ci (mam nadzieję w prosty sposób, czym są i jak działają funkcje)
