+++
title = "Prywatnośc W Sieci"
date = 2017-11-10T09:31:42+01:00
draft = true
tags = ["privacy", "pl", "tutorial"]
+++
<!-- Local Variables: -->
<!-- ispell-dictionary: polish -->
<!-- End: -->

Ostatnio na zajęciach wywiązała się rozmowa na temat prywatności w sieci. Zdałem
sobie sprawę, że wiele osób uważa śledzenie działalności użytkowników internetu za
niepożądany proceder, z którym jednak nie da się nic zrobić. Czy to z braku
technicznej wiedzy lub zainteresowania tematem niektórzy przyjmują
postawę typu:

> No wszyscy w internecie szpiegują, ale nic z tym nie zrobisz. Najlepiej o tym nie myśleć.

Zgodzę się, że całkowita *prywatność*, a tym bardziej *anonimowość*
w internecie jest trudna. Jest to raczej proces i pewien sposób myślenia
(skłonności do paranoi...), niż zestaw reguł, których wystarczy się trzymać. Na
szczęście zgodnie z zasadą Pareta 80% rezultatów można osiągnąć, poświęcając 20%
procent czasu, prawda? :wink:

Postanowiłem napisać krótki poradnik pokazujący **podstawowe** czynności, które
możesz wykonać, aby utrudnić "szpiegowanie".
Nie twierdzę, że ten poradnik jest kompletny, ale lepsze to niż nic :)
Mam nadziej, że ta wiedza komuś się przyda.

## Zagrożenia

Chcesz więc obronić swoje wirtualne życie przed "szpiegowaniem". W takim
razie wypada ustalić *kto* nasz szpieguje. I **po co** to robi? Oraz w jaki
sposób.

Myślę, że najpowszechniejszym zagrożeniem dla prywatności są **reklamy**.
Niestety model biznesowy wielu serwisów internetowych opiera się głównie na
zarobkach z reklam. Na reklamach swoją potęgę zbudowała firma Google. Reklamy są
nie tylko denerwujące. Wiele z nich zawiera **skrypty śledzące użytkowników.** Po co
reklamodawcom informacje o użytkownikach? Głównie po to, żeby dostarczać
bardziej *spersonalizowane* reklamy. Jeśli Google wykryje, że szukamy informacji o
rowerach, to zacznie nam pokazywać reklamy związane z rowerami. Co gorsze, firmy
reklamowe sprzedają sobie nawzajem informacje, które zebrały.


## Pierwsza linia obrony

Zacznijmy od reklam widocznych na stronach www.

Wiele osób wie, że reklamy można blokować w przeglądarce przy pomocy
dodatków. Chyba najbardziej znanym tego typu dodatkiem jest **AdBlock**. Może
masz go zainstowanego? Tak? To go usuń.

AdBlock a szczególnie AdBlock Plus jest złym wyborem z kilku powodów:

- pokazuje pewne reklamy, które autorzy uznali za **nieinwazyjne**
- często jest nieskuteczny
- stanowi większe obciążenie dla komputera niż alternatywy
- https://www.wired.com/2016/03/heres-how-that-adblocker-youre-using-makes-money/

Z moich doświadczeń wynika, że najlepszym blokerem reklam jest **µBlock
Origin**. Jest szybki, skuteczny i nie decyduje za Ciebie, jakie
reklamy wyświetlać.

Można go zainstalować tutaj:

- [Chrome](https://chrome.google.com/webstore/detail/ublock-origin/cjpalhdlnbpafiamejdnhcphjbkeiagm?hl=pl)
- [Firefox](https://addons.mozilla.org/pl/firefox/addon/ublock-origin/)

Po zainstalowaniu µBlock działa już całkiem nieźle, ale warto go
skonfigurować. Klikamy na przycisk µblock na pasku przeglądarki, a następnie na
opcję "Panel sterowania". Przechodzimy do zakładki "Zewnętrzne filtry".

![panel](/images/bezp-panel.png)

Teraz możesz wybrać, z jakich list filtrów chcesz korzystać. Proponuję
następujące ustawienia:

- zaznaczyć **wszystkie uBlock filters** z wyjątkiem *experimentals*
- zaznaczyć **Adblock Warning Removal List** oraz **EasyList**
- zaznaczyć **EasyPrivacy**
- zaznaczyć **Malware Domain List** oraz **Malware domains**
- koniecznie zaznaczyć **POL: polskie filtry do Adblocka i uBlocka** oraz **POL: polskie filtry do uBlocka uzupelnienie**
- resztę zostawić tak jak była (domyślnie)

Następnie klikamy u góry strony w przycisk **Aktualizuj**. Zrobione!

## Druga linia obrony

Kolejnym zagrożeniem dla prywatności są wszelkiego rodzaju skrypty śledzące.
O ich obecności nie jesteśmy w żaden sposób informowani. Przykład takiego skryptu:
Google Analytics. Zbiera on informacje ile osób i kiedy wchodziło na daną stronę.

Do zablokowania tego typu skryptów służy kolejny dodatek: **Privacy Badger**

- [Chrome](https://chrome.google.com/webstore/detail/privacy-badger/pkehgijcmpdhfbdbbnkijodmdjhbjlgp)
- [Firefox](https://addons.mozilla.org/en-US/firefox/addon/privacy-badger17/)

Tutaj nie trzeba nic skonfigurować. Po zainstalowaniu dodatek wyświetli krótką
instrukcję, z którą warto się zapoznać.



## Kłódka

![](/images/bezp-klodka.png)

Na większości stron przeglądarka wyświetla ikonę kłódki po lewej stronie adresu.
Oznacza to, że dane są wysyłane i odbierane przy pomocy *zaszyfrowanego* połączenia HTTPS. To dobrze!
Warto jednak zainstalować dodatek **HTTPS Everywhere**. Dzięki niemu przeglądarka **zawsze** wybierze bezpieczne
połączenie, nawet jeśli strona oferuje również nieszyfrowane HTTP. Dodatek ten nie wymaga konfiguracji.

- [Chrome](https://chrome.google.com/webstore/detail/https-everywhere/gcbommkclmclpchllfjekcdonpmejbdp?hl=pl)
- [Firefox](https://addons.mozilla.org/pl/firefox/addon/https-everywhere/)

## Lisek

Warto zastanowić się nad wyborem przeglądarki. Według
[netmarketshare](www.netmarketshare.com) najpopularniejszą przeglądarką w dniu
pisania tego posta jest Chrome. Chrome jest szybki i prosty, ale ma kilka
zasadniczych wad:

- Chrome **nie jest** [wolnym/otwartym oprogramowaniem](https://pl.wikipedia.org/wiki/Wolne_oprogramowanie)
- czasami zużywa [duże ilości pamięci RAM](https://blog.mozilla.org/firefox/firefox-uses-less-memory-chrome-edge-safari/), co może być kłopotliwe na starszych komputerach
- i co najważniejsze, Chrome jest dziełem Google i wysyła sporo informacji o
  użytkowniku do swoich autorów.

Firefoxa tworzy fundacja Mozilla. Jednym z celów "statutowych" Mozilli jest
dbanie o prywatność użytkowników. Celem Google jest zarabianie. Między innymi
na danych zebranych przez Chrome.

> Mozilla to organizacja non-profit wspierająca Firefoksa, oryginalną alternatywną przeglądarkę. Tworzymy produkty i zasady służące użytkownikom Internetu, nie zyskom.

Parę miesięcy temu nie ośmieliłbym się sugerować komukolwiek używania Firefoksa.
Do wersji 55 FF działał strasznie wolno. To jeden z powodów masowej migracji na Chrome.

Kilka dni temu Mozilla wydała Firefoxa 57. To jena z największych aktualizacji do tej pory.
Poza nowym interfejsem autorzy *drastycznie* poprawili wydajność. Obecnie Firefox
[**dorównuje szybkością Chrome**](https://youtu.be/YIywpvHewc0). Uważam, że warto dać liskowi szansę, to
naprawdę solidna przeglądarka.


## Wyłączanie blokowania

Blokowanie reklam i skryptów może czasem "zepsuć" jakąś stronę do tego stopnia,
że nie będzie można jej używać. Zdarza się to rzadko. Warto jednak
wiedzieć, jak wyłączyć blokowanie reklam na dla konkretnej strony.

1. Otwórz stronę, która nie działa.
2. Kliknij przycisk µBlock na pasku przeglądarki.
3. Naciśnij wielki, niebieski wyłącznik.
4. Odśwież stronę
5. Jeśli nadal nie działa, to kliknij przycisk Privacy Badger na pasku przeglądarki.
6. Kliknij "Disable Privacy Badger for this site"
7. Odśwież stronę.
8. Jeśli nie nadal nie działa to znaczy, że strona jest zepsuta, wróć później ¯\_ツ_/¯

## To tyle

Tak jak mówiłem — podstawy. Nie opisuję tu bardziej zaawansowanych metod, głównie
dlatego że są skomplikowane. Te porady mimo prostoty poprawia komfort korzystania z
internetu, utrudniając jednocześnie śledzenie użytkownika.

Jeśli masz jakieś pytania, pisz śmiało na Twitterze lub Facebooku.

<br>
