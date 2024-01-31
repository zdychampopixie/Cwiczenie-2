**Odpowiedzi na pytania z ćwiczenia:**

## **Losowy Podział Punktów**
#####  1. Dlaczego sieć osiąga tak niską skuteczność trenowania na wskazanym zbiorze?<br/>
***Złożoność danych:*** Zbiór danych może zawierać różnorodne kształty i rozkłady, co utrudnia klasyfikację, zwłaszcza dla prostszych modeli.<br/>
***Architektura modelu***: Prostsza architektura modelu może nie być wystarczająco zdolna do dopasowania się do złożonych danych.<br/>
***Liczba epok:*** Niewystarczająca liczba epok treningowych może nie pozwolić modelowi na efektywną naukę. *<br/>

##### 2. Czy jest coś, co można zrobić, aby klasyfikator poprawił jakość trenowania?<br/>
*Zwiększenie złożoności modelu: Dodanie warstw i neuronów może pomóc w lepszym dopasowaniu do danych.<br/>
Dopasowanie hiperparametrów: Eksperymentowanie z różnymi wartościami współczynników uczenia i innych hiperparametrów.<br/>
Zwiększenie liczby epok: Dłuższy trening może poprawić dopasowanie modelu do danych.<br/>
Techniki regularyzacji: Stosowanie dropoutu czy normalizacji warstw może zmniejszyć ryzyko przeuczenia.<br/>
Inżynieria cech: Przygotowanie danych w sposób, który ułatwia klasyfikację.*
## Podział Gaussa<br/>
**1. Dlaczego wyniki trenowania są lepsze niż w poprzednim zbiorze?**<br/>

*Rozróżnialność danych: Zmodyfikowany zbiór trenujący, wykorzystujący podział Gaussa, generuje bardziej oddzielone dane, co ułatwia naukę i klasyfikację.
Zwiększenie liczby epok: Pozwala modelowi na lepsze dopasowanie się do bardziej złożonych danych.*<br/>
**2. Czy architektura sieci ma znaczny wpływ na jakość klasyfikacji?**<br/>

*Tak, wybór architektury sieci jest kluczowy dla klasyfikacji, włączając w to liczbę warstw, neuronów i typ funkcji aktywacji.*<br/>
**3. Czy szybkość trenowania ma wpływ na jakość klasyfikacji?**<br/>

*Tak, odpowiednia szybkość trenowania jest ważna dla uniknięcia przeuczenia oraz zapewnienia odpowiedniej dokładności.*<br/>
**4. Czy rodzaj optymalizatora ma wpływ na jakość klasyfikacji?**<br/>

*Tak, wybór optymalizatora ma znaczenie dla uniknięcia problemów, takich jak zatrzymanie w minimum lokalnym, i wpływa na skuteczność uczenia się modelu.*<br/>

## Inne Zbiory
**Dlaczego wyniki trenowania dają lepsze rezultaty niż w poprzednim zbiorze**.<br/> UZASADNIĆ ODPOWIEDŹ.<br/>
*Wyniki trenowania na zbiorze geometrycznym nr 4 mogą być lepsze niż na poprzednich zbiorach, ponieważ ten zbiór jest bardziej złożony i bardziej skomplikowany niż poprzednie. Zawiera on różne kształty i klastry danych, co oznacza, że potrzebujemy bardziej zaawansowanej architektury sieci neuronowej, aby efektywnie klasyfikować te dane. Dlatego, gdy używamy bardziej zaawansowanych architektur i dostosowujemy hiperparametry, możemy osiągnąć lepszą dokładność klasyfikacji na tym zbiorze.* <br/>
**2. Czy architektura sieci ma znaczny wpływ na jakość klasyfikacji. **<br/>
*Tak, architektura sieci ma znaczny wpływ na jakość klasyfikacji. Wybór liczby warstw, liczby neuronów w warstwach, funkcji aktywacji i innych hiperparametrów może znacząco wpłynąć na zdolność sieci do nauki i klasyfikacji danych. Dlatego eksperymentując z różnymi architekturami, możemy znaleźć tę, która najlepiej pasuje do danego zadania.* <br/>
**3. Czy szybkość trenowania ma wpływ na jakość klasyfikacji. **<br/>
*Tak, szybkość trenowania może mieć wpływ na jakość klasyfikacji. Zbyt szybkie trenowanie (wysoki learning rate) może prowadzić do tego, że sieć nie będzie w stanie zbiegać do optymalnego rozwiązania i skończy się to niższą dokładnością. Zbyt wolne trenowanie (niski learning rate) może wymagać znacznie więcej czasu na osiągnięcie akceptowalnych wyników. Optymalna szybkość trenowania zależy od konkretnego zadania i zbioru danych i może być ustalona eksperymentalnie. * <br/>
**4. Czy rodzaj optymalizatora ma wpływ na jakość klasyfikacji.**<br/>
*Tak, rodzaj optymalizatora ma wpływ na jakość klasyfikacji. Różne optymalizatory mają różne strategie aktualizacji wag sieci w trakcie trenowania. Na przykład, Adam jest popularnym optymalizatorem, który jest często używany ze względu na jego skuteczność w wielu zadaniach. Jednak różne optymalizatory mogą działać lepiej lub gorzej w zależności od konkretnego zadania i hiperparametrów. Dlatego warto eksperymentować z różnymi rodzajami optymalizatorów, aby znaleźć ten, który działa najlepiej dla danego zadania.*<br/>

## Rozdział 2 – Klasyfikacja obrazów

***Wpływ struktury sieci na rozpoznawanie i klasyfikację: ***<br/>Struktura sieci neuronowej ma ogromny wpływ na jej zdolność do rozpoznawania i klasyfikacji danych. Sieci o bardziej zaawansowanej strukturze, z większą liczbą warstw i neuronów, mogą nauczyć się bardziej skomplikowanych cech i złożonych wzorców w danych, co może poprawić jakość klasyfikacji. Jednak bardziej skomplikowana struktura sieci może również wymagać więcej danych i obliczeń.

***Wpływ zastosowania warstw dropout na klasyfikację:*** <br/>Warstwy dropout są używane w celu zapobiegania przeuczeniu się modelu. Poprzez losowe wyłączanie pewnych neuronów podczas treningu, warstwy dropout pomagają w generalizacji modelu, co zazwyczaj poprawia zdolność klasyfikacji na danych testowych. Wpływ warstw dropout na klasyfikację polega na zwiększeniu ogólności modelu.

***Wpływ szybkości uczenia na klasyfikację:***<br/> Szybkość uczenia (learning rate) jest ważnym parametrem treningowym. Zbyt mała wartość learning rate może spowolnić uczenie, podczas gdy zbyt duża może prowadzić do niestabilnego treningu lub przeuczenia. Optymalna wartość learning rate jest często wynikiem eksperymentów i dostosowania do konkretnego problemu.

***Wpływ jakości zbioru trenującego na uczenie:*** <br/><br/>Jakość zbioru trenującego ma ogromny wpływ na uczenie maszynowe. Zbiór trenujący powinien być reprezentatywny i dobrze zbalansowany. Nieprawidłowe lub niedostateczne dane trenujące mogą prowadzić do złych wyników klasyfikacji. Im lepsza jakość danych trenujących, tym lepiej sieć będzie w stanie się nauczyć i klasyfikować.

***Czy sieć zawsze będzie dobrze trenować?:***<br/> Nie, sieć neuronowa nie zawsze będzie dobrze trenować. Wynik treningu zależy od wielu czynników, w tym od architektury sieci, jakości danych, dostrojenia hiperparametrów i ilości dostępnych danych treningowych. Czasem może być trudno uzyskać wysoką dokładność klasyfikacji ze względu na trudność problemu lub brak odpowiednich danych.

***Czy ilość epok miała wpływ na trenowanie obrazów?: ***<br/>Tak, ilość epok (czyli liczba cykli treningu) ma wpływ na trenowanie obrazów. Zbyt mała ilość epok może prowadzić do niedotrenowania, podczas gdy zbyt duża ilość epok może prowadzić do przeuczenia. Optymalna liczba epok zależy od problemu i struktury sieci oraz jest często ustalana eksperymentalnie.

***Czy uczenie z transferem daje dobre wyniki?: ***<br/>Uczenie z transferem (transfer learning) może dawać bardzo dobre wyniki w wielu przypadkach, szczególnie gdy masz ograniczone dane treningowe. Wykorzystanie pre-trenowanych modeli, takich jak VGG16 czy ResNet, jako punktu wyjścia, może znacznie przyspieszyć i poprawić trenowanie na nowych danych. Jednak skuteczność uczenia z transferem zależy od odpowiedniego dostosowania modelu do nowego problemu oraz jakości danych treningowych.
