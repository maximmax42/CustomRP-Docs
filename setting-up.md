---
description: RTFM
---

# 🛠 Ustawienie

Jeśli masz jakieś problemy sprawdź [FAQ](faq.md).

Zanim zaczniesz upewnij się że masz włączony status aktywności w ustawieniach Discorda:

<figure><img src="https://user-images.githubusercontent.com/79161805/195936167-0f5cb6b3-8cb6-4474-97d7-a18c301b9e7e.png" alt=""><figcaption></figcaption></figure>

## Proces ustawiania

(nie ma tłumaczenia dla portalu deweloperskiego Discord)

* Przejdź do https://discord.com/developers/applications/.
* Kliknij **New Application** (nowa aplikacja) w prawym górnym rogu.

![image](https://user-images.githubusercontent.com/2225711/161050202-c796103d-6712-401e-be96-3f3712512375.png)

* Wybierz nazwę dla aplikacji, będzie się wyświetlała po napisie "W grze" w statusie; kliknij **Create** (stwórz).
* Skopiuj **Application ID** (ID aplikacji) i wklej je do Custom RP w polu **ID**, wtedy kliknij **Połącz**. Jeśli wszystko poszło dobrze, twój status na Discordzie powinien pokzywać "W grze **\[nazwa aplikacji]**".
  * Pamiętaj: Jeśli masz ustawiony status własny (ten z emotką), będzie wyświetlał się nad tym z CustomRP, który mimo to będzie pokazany na profilu.

![image](https://user-images.githubusercontent.com/2225711/161050341-8169af53-5d3f-44d6-b745-cc711e8d1476.png)

* Na stronie swojej aplikacji przejdź do Rich Presence -> Art Assets i prześlij co najmniej jeden obraz w Rich Presence Assets, jeśli chcesz ich użyć. W CustomRP istnieje poręczny przycisk **Upload Assets** w menu Plik (możesz również kliknąć Ctrl+U), który przeniesie cię tam, jeśli pole ID jest skonfigurowane poprawnie.
  * Inaczej, możesz po prostu wstawić adres URL do obrazu w polu **Key**.
  * Uwaga: Mimo że możesz nazwać swój zasób dowolną nazwą do 999 symboli, API zaakceptuje tylko nazwy z maksymalnie 256 symbolami.
* Przejdź do strony wizualizatora, aby skonfigurować pola **Stan, Szczegóły, Key dużego obrazu, Tekst dużego obrazu, Key małego obrazu, Tekst małego obrazu, Rozmiar drużyny, Max drużyny**. Wszystkie z nich są opcjonalne.
* Po znalezieniu konfiguracji, która cię zadowala, skopiuj wartości do odpowiednich pól w CustomRP.
  * Wskazówka: Możesz najechać na prawie każdy element sterujący w aplikacji (w tym linię etykiet **Details**) aby otrzymać podpowiedź!
* Jeśli chcesz ustawić również przyciski, wypełnij oba pola Text i URL.
  * Uwaga: Kiedy będziesz klikał na przyciski w swoim własnym statusie, nie będą one działać, ale nie martw się, będą działać dla wszystkich innych. To problem po stronie Discorda.
* Kliknij **Zaktualizuj status** (lub **Połacz**, jeśli nie jesteś jeszcze połączony).
* Gratulacje, jest super!


### Używam więcej niż jednego klienta Discord, co mam zrobić?

Jeśli masz więcej niż jednego klienta Discord i chcesz, aby Twój status pojawiał się na innym koncie niż to, które aplikacja wybrała automatycznie, kliknij **Rozłącz**, następnie przytrzymaj klawisze Ctrl+Shift na klawiaturze i kliknij **Połącz**. Pojawi się okienko z wpisywaną liczbą, należy wpisać cyfrę 1, zamknąć okienko i ponownie kliknąć **Połącz**, już bez Ctrl+Shift. W przypadku, gdy to znowu złe konto, spróbuj numeru 0, potem 2 i tak dalej aż do 9.

Zwróć uwagę, że jeśli masz kilka klientów Discorda uruchomionych podczas startu, numer w okienku przypisany do każdego klienta może nie być stały od startu do startu i może się zmienić w zależności od tego, który klient uruchomił się jako pierwszy. Aby temu zapobiec, możesz ręcznie uruchomić dodatkowe klienty lub użyć Harmonogramu zadań systemu Windows, aby opóźnić ich uruchomienie.

Jeśli masz 2 konta, których używasz w tym samym czasie i chcesz, aby każde z nich miało inny status, to wykonaj następujące kroki:

* Skonfiguruj najpierw swoje główne konto za pomocą powyższych instrukcji.
* Pobierz najnowszą **przenośną (.zip)** wersję CustomRP (z [strony internetowej](https://www.customrp.xyz) lub [strony wydań GitHub](https://github.com/maximmax42/Discord-CustomRP/releases/latest)) i rozpakuj ją w dowolnym miejscu.
  * Działa to tylko z wersjami 1.16 i starszymi.
* Otwórz `Start Second Instance.bat` lub utwórz skrót do CustomRP.exe z argumentem `--second-instance` (lub `-2`).
* Skonfiguruj program w taki sam sposób jak swoją główną instancję.
  * Wskazówka: Jeśli masz już szablon, którego chcesz użyć w drugiej instancji, możesz edytować plik bat lub skrót, aby zawrzeć ścieżkę do szablonu. Przykład: `CustomRP.exe -2 "C:\Jakiś folder\preset.crp"` (cudzysłów wokół ścieżki jest konieczny, jeśli ścieżka ma w nim spacje).
* Przed połączeniem zmień wartość okna w sposób opisany wcześniej i połącz się.

Jeśli używasz 3 lub więcej kont jednocześnie, to... po co? Ale też jeśli wystarczająco dużo z was będzie mnie błagać, dodam wsparcie dla używania większej liczby instancji.

## Uwagi.

* Jeśli nie chcesz ustawiać małego lub dużego obrazu, pozostaw wszystkie powiązane pola w programie puste.
* Jeśli duży obraz nie jest ustawiony, ustawienia małego obrazu będą ignorowane.
*** Przetłumaczono za pomocą www.DeepL.com/Translator (wersja darmowa) ***

