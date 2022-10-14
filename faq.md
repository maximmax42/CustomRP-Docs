---
description: Często zadawane pytania
---

# ❓ FAQ

## Pytania

### Da się dodać więcej niż dwa guziki?

Nie, Discord to ograniczył.

### Da się użyć innego typu aktywności (np. słucha, ogląda, streamuje)?

Nie, to też jest ograniczenie na Discordzie.

### Czemu gdy ustawię kilka dni w przyszłość Discord pokazuje ile godzin zostało?

Zgadłeś, to też ograniczenie wymyślone przez Discorda.

### Czy postanie wersja na Linux/Maca?

Aplikacja jest zbudowana na bibliotece pod Windowsa, dlatego wspieranie Linuxa i Maca oznaczałoby przepisanie całej aplikacji w innej bibliotece/innym języku programowania czego narazie nie planuję.

### Okno nazwane "Pipe" otworzyło się z jakiegoś powodu, co to jest?

Otworzyło się ponieważ przytrzymałeś Ctrl+Shift i kliknąłeś guzik Połącz (lub Ctrl i guzik Połącz lub guzik Połącz ponwnie w trayu na starszych wersjach). Zostaw jego wartość na -1 i zamknij je. Jest ono używane w przypadku gdy masz więcej niż jednego klienta Discord działającego w tym samym czasie. Zmienianie wartości wybiera którego klienta chcesz używać do pokazywania statusu.

## Rozwiązywanie problemów

Zanim spróbujesz czegokolwiek, upewnij się, że masz najnowszą wersję CustomRP!

### Kiedy klikam na przyciski obecności w moim profilu, nie działają.

Przyciski nie będą działać na kliencie stacjonarnym, z którym korzystasz z CustomRP, to problem Discorda. Możesz przetestować swoje przyciski z poziomu klienta mobilnego lub webowego, albo po prostu zapytaj kogoś innego.

### Zainstalowałem CustomRP, ale nie uruchamia się.

Jest to najprawdopodobniej wina twojego antywirusa uniemożliwiającego uruchomienie aplikacji. Dodaj folder `%appdata%CustomRP` do wyjątków.

### Zainstalowałem CustomRP, zezwoliłem na analitykę i aplikacja już nie działa.

Wymuś zamknięcie aplikacji w Menedżerze zadań, usuń folder `%localappdata%\maximmax42`, uruchom aplikację ponownie i nie zezwalaj na analitykę.

### Aplikacja się połaczyła, ale nie widzę statusu w moim profilu.

Upewnij się że masz włączony status aktywności w ustawieniach Discorda:

<figure><img src="https://user-images.githubusercontent.com/2225711/188219661-49713f90-fa76-4645-b04a-fc1bc0f029bd.png" alt=""><figcaption></figcaption></figure>

### Aplikacja działała, ale teraz łączy się w nieskończoność.

Być może dostałeś timeout od Discorda z powodu łączenia się/zmiany statusu za szybko i za dużo. Rozłącz się, poczekaj 5-10 minut, spróbuj połączyć się ponownie. Ponowne uruchomienie Discorda też może pomóc.

### Aplikacja mówi "Nieprawidłowe ID?"/"Czy Discord jest uruchomiony?" lub łączy się w nieskończoność, mimo że jestem pewien, że zrobiłem wszystko dobrze i Discord jest uruchomiony.

Czasami jest to spowodowane przez BetterDiscord. Jeśli masz go zainstalowanego, odinstaluj go, pozwól CustomRP połączyć się z Discordem przynajmniej raz, a następnie zainstaluj BD z powrotem. Jeśli nie, spróbuj uruchomić CustomRP jako administrator. Jeśli to nie pomoże, spróbuj dodać `%appdata%\CustomRP` lub w przypadku gdy używasz wersji portable, folder do którego wypakowałeś CustomRP (i może Discorda) do wyjątków zapory/antywirusa, a następnie zrestartuj komputer (możesz spróbować zrestartować tylko Discorda i CustomRP, ale w 95% przypadków to nie działa). Inną rzeczą, którą możesz spróbować, jest tymczasowe wyłączenie wszystkich klientów Discorda oprócz tego, którego używasz. Jeśli to nie pomoże, nie wiem co innego możesz zrobić, przepraszam.

### Aplikacja działała wcześniej, ale potem się zawiesiła, a teraz w ogóle się nie uruchamia.

Być może wstawiłeś długi ciąg losowego tekstu (lub tekst w języku który nie używa liter łacińskich) w jakimś polu i to spowodowało awarię aplikacji. Aby to naprawić, kliknij klawisz Win+R, wpisz `%localappdata%` i usuń lub zmień nazwę folderów z CustomRP w nazwie, a następnie uruchom aplikację. Pamiętaj że to resetuje aplikację całkowicie.

### Aplikacja ciągle się zawiesza podczas aktualizacji/próby połączenia/itp.

Jeśli jesteś w stanie uruchomić aplikację i uzyskać raport awarii który zawiera `System.IO.FileNotFoundException: Could not load file or assembly...`, zainstaluj aplikację ponownie.

Jeśli nie możesz znaleźć odpowiedzi na swoje pytanie/swój problem, wyślij wiadomość na kanał `#support` na [serwerze Discord CustomRP](https://www.customrp.xyz/discordserver), napisz do mnie na Discordzie (maximmax42#5572) lub [zgłoś błąd na Githubie](https://github.com/maximmax42/Discord-CustomRP/issues/new/choose)
