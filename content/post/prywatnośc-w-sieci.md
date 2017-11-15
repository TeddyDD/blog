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
technicznej wiedzy, lub zainteresowania tematem niektórzy przyjmują
postawę typu:

> No wszyscy w internecie szpiegują ale nic z tym nie zrobisz. Najlepiej o tym nie myśleć.

Zgodzę się, że całkowita *prywatność*, a tym bardziej *anonimowość*
w internecie jest trudna. Jest to raczej proces i pewnien sposób myślenia
(skłonności do paranoii...), niż zestaw reguł których wystarczy się trzymać. Na
szczęście zgodnie z zasadą Pareta 80% rezultatów można osiągnąć poświęcając 20%
procent czasu, prawda? :wink:

Postanowiłem napisać krótki artykuł w formie poradnika — jak się bronić przed
ciągłym śledzeniem w internecie. Nie jest to wyczerpujący materiał, nie poruszam
zaawansowanych tematów takich ja VPNy, Tor etc. Są to absolutne podstawy, które
uniemożliwią lub utrudnią skutecznie wiele prób śledzenia i które **bardzo łatwo**
zastosować. Mam nadziej, że ta wiedza komuś się przyda. Mi natomiast przyda
się rozgrzewka przed pisaniem pracy magisterskiej...

## Zagrożenia

Postanowliśmy więc obronić nasze wirtualne życie przed "szpiegowaniem". W takim
razie wypada ustalić *kto* nasz szpieguje. I **po co** to robi? Oraz w jaki
sposób.

Myślę, że najpowszechniejszym zagrożeniem dla prywatności są **reklamy**.
Niestety model biznesowy wielu serwisów internetowych opiera się głównie na
zarobkach z reklam. Na reklamach swoją potęge zbudowała firma Google. Reklamy są
nie tylko denerwujące. Wiele z nich zawiera **skrypty śledzące użytkowników.** Po co
reklamodawcom informacje o użytkownikach? Głównie po to, żeby dostarczać
bardziej *spersonalizowane* reklamy. Jeśli Google wykryje, że szukamy informacji o
rowerach, to zacznie nam pokazywać reklamy związane z rowerami. Co gorsze, firmy
reklamowe sprzedają sobie nawzajem informacje które zebrały.


## Pierwsza linia obrony

Zacznijmy od reklam widocznych na stronach www.

Jak wielu z was zapewne wie, reklamy można blokować w przeglądarce przy pomocy
dodatków. Najpopularniejszym tego typu dodatkiem jest **AdBlock**. Może częśc z
was ma go zainstalowanego? Tak? To go odinstalujcie.

AdBlock a szczególnie AdBlock Plus jest złym wyborem z kilku powodów:

- pokazuje pewne reklamy, które autorzy uznali za **nieinwazyjne**
- często jest nieskuteczny
- stanowi większe obciążenie dla komputera niż alternatywy
- https://www.wired.com/2016/03/heres-how-that-adblocker-youre-using-makes-money/

Z moich doświadczeń wynika, że obecnie najlepszym blokerem reklam jest **µBlock
Origin** (można pisać uBlock, po prostu szpanuje, że wiem jak wpisać "mi" z
klawiatury :grinning: ). Jest szybki, skuteczny i nie decyduje za nas, jakie
reklamy wyświetlać.

Można go zainstalować tutaj:

- [Chrome](https://chrome.google.com/webstore/detail/ublock-origin/cjpalhdlnbpafiamejdnhcphjbkeiagm?hl=pl)
- [Firefox](https://addons.mozilla.org/pl/firefox/addon/ublock-origin/)

Po zainstalowaniu µBlock działa już całkiem nieźle, ale warto go
skonfigurować. Klikamy na przycisk µUblock na pasku przeglądarki a następnie na
opcję "Panel sterowania". Przechodzimy do zakładki "Zewnętrzne filtry".

Teraz możemy wybrać z jakich list filtrów chcemy korzystać. Proponuję
następujące ustawienia:

- zaznaczyć **wszyskie uBlock filters** z wyjątkiem *experimentals*
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

Do zablokowania tego typu skryptów użyjemy kolejnego dodatku: **Privacy Badger**

- [Chrome](https://chrome.google.com/webstore/detail/privacy-badger/pkehgijcmpdhfbdbbnkijodmdjhbjlgp)
- [Firefox](https://addons.mozilla.org/en-US/firefox/addon/privacy-badger17/)



## Wyłączanie blokowania

<br>
