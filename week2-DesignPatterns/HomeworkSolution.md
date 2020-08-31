Pod lupę wziąłem trochę więcej wzorców niż w poleceniu, ale dużo jest według mnie godnych zastosowania.<br/>
<b>THROTTLING<b/><br/>
Ograniczenie ilości zapytań podczas krótkotrwałych okresów dużego popytu.<br/>
Dodatkowo dzięki throttlingowi jesteśmy w stanie zagwarantować dostęp do usługi zgodny z SLA bez konieczności auto skalowania.<br/>
Zaletą throttlingu jest informacja zwrotna którą otrzymuje aplikacja kliencka czy klient o przekroczeniu ilości zapytań.<br/>
Przykład usługi do zastosowania: API Management<br/>
<b>AUTOSCALLING<b/><br/>
Zdolność aplikacji do dynamicznej zmiany swoich rozmiarów, dzięki czemu uzyskujemy wysoką <br/>
wydajność i dostępność nawet w krytycznych momentach takich jak np. black Friday.
Jeżeli większość naszych klientów jest np. z Europy to możemy zmniejszyć liczbę instancji w godzinach <br/>
mniejszego zapotrzebowania np. w nocy (po wcześniejszej dokładnej analizie ruchu).
Przykład usługi do zastosowania: tutaj raczej opcje wbudowane w usługi wystarczą czy to VM, VM Scale Sety<br/>
czy skalowanie AppService. Należy tylko pamiętać o restarcie VM podczas resize (jeżeli byłaby potrzeba na skalowanie w górę a nie wszerz).<br/>
<b>Static Content Hosting<b/><br/>
Aplikacje e-commerce np. sklepy internetowe posiadają bardzo dużą ilość statycznej treści chociażby obrazy.<br/>
Zwiększenie wydajności aplikacji poprzez wzrost szybkości dostępu do danej treści oraz nie obciążanie aplikacji.<br/>
Zmniejszenie kosztów magazynowania.<br/>
Przykład usługi do zastosowania: Content Delivery Network<br/>
<b>Sharding<b/><br/>
Tutaj od razu nasuwa mi się jako pierwsze RODO i inne kwestie związane z bezpieczeństwem.<br/>
Niektóre regiony prawnie wymagają aby dane ich mieszkańców mogły być przechowywane tylko w danej lokalizacji.<br/>
Dodatkowo w przypadku pojedynczego miejsca składowania i dużej ilości zapytań / operacji wykonywanych na danych może spaść wydajność i czas odpowiedzi.<br/>
Ograniczenia i limity wynikające z przechowywania danych w jednym miejscu. Systemy e-commerce przechowują bardzo dużą ilość danych, aby nie doprowadzić<br/>
do sytuacji osiągnięcia limitu warto te dane dzielić.<br/>
Przykład usługi do zastosowania: Azure SQL Database, Azure CosmosDb<br/>
<b>Queue Based Load Leveling<b/><br/>
Dzięki użyciu kolejki usługa konsumuje w swoim tempie przychodzące wiadomości, nie wystąpi sytuacja zgubionej<br/>
wiadomości nawet w przypadku dużego obciążenia aplikacji.<br/>
Jeżeli aplikacja jest typu „loosely coupled” zastosowanie kolejek nie wpłynie na dostępność aplikacji gdy jeden z konsumentów <br/>
nie jest dostępny to i tak inna usługa może wrzucać swoje dane do kolejki nie powodując przestoju w pracy aplikacji.<br/>
Przykład usługi do zastosowania: Azure Service Bus<br/>
Zalety: możliwość tworzenia tematów, które w przeciwieństwie do zwykłej kolejki nie konkurują o dane.<br/>
<b>Load Balancing<b/><br/>
Nasza usługa musi być wysoce dostępna i wydajna. Zatem przychodzący ruch należy rozdzielać.<br/>
Usługa niezbędna do przeprowdzania konserwacji aplikacji bez przestojów w jej działaniu.<br/>
Przykład usługi do zastosowania: Load Balancer, Traffic Manager<br/>
Jeżeli np. nasi klienci są z całego świata warto zastosować Traffic Manager, który ma opcję przekierowywania klienta do najbliższego punktu końcowego<br/>
tak aby opóźnienie było jak najmniejsze. Zastosowanie w przypadku App Service'ów.<br/>
W przypadku aplikacji opartej na wirtualnych maszynach zastosowałbym Load Balancer.<br/>
Jeżeli potrzebne byłoby rozrzucanie ruchu na poziomie warstwy 7 to można zastosować jeszcze Application Gataway choć to dość kosztowne rozwiązanie.

