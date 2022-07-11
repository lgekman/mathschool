# Räkna med rationella tal

Normala [prioriteringsregler](https://sv.wikipedia.org/wiki/Operatorprioritet)
gäller, tex att gånger går före plus, men det blir krångligare med bråktal.

## Addition och subtraktion

Addition och subtraktion kan bara utföras om nämnaren är lika;

$$\frac{57}{10} + \frac{3}{10} = \frac{57 + 3}{10} = \frac{60}{10} = \frac{6}{1} = 6 $$

Om nämnaren *inte* är lika måste man förlänga bråket så att nämnaren
blir lika. Det vi helst vill ha är "minsta gemensamma nämnare" men det
är inte alltid så enkelt.

En allmän formel som dock *alltid* fungerar är att förlänga till produkten av
nämnarna;

$$\frac{a}{b} - \frac{c}{d} = \frac{a \cdot d}{b \cdot d} - \frac{c \cdot b}{d \cdot b} = \frac{a \cdot d - c \cdot b}{b \cdot d} $$

Detta blir ofta onödigt krångligt;

$$\frac{7}{10} - \frac{9}{20} = \frac{7 \cdot 20}{10 \cdot 20} - \frac{9 \cdot 10}{20 \cdot 10} = \frac{7 \cdot 20 - 9 \cdot 10}{10 \cdot 20} = \frac{50}{200} = \frac{1}{4} $$

Här kan vi se att om vi förlänger vänstra termen med $2$ så får vi en
gemensam nämnare $20$ (som faktiskt är den minsta gemensamma nämnaren);

$$\frac{7}{10} - \frac{9}{20} = \frac{7 \cdot 2}{10 \cdot 2} - \frac{9}{20} = \frac{7 \cdot 2 - 9}{20} = \frac{5}{20} = \frac{1}{4} $$

**Uppgift:** beräkna;

$$\frac{323}{228} - \frac{187}{204}$$

Använd det allmäna sättet, [faktoruppdela](
https://www.calculatorsoup.com/calculators/math/prime-factors.php)
och förenkla resultatet.

<details><summary>(facit)</summary>

$$\frac{323}{228} - \frac{187}{204} = \frac{65892}{46512} - \frac{42636}{46512} = \frac{23256}{46512} = \frac{1}{2}$$

</details>



## Multiplikation

Vid multiplikation behöver man inte bekymmra sig om gemensam nämnare;

$$ \frac{40}{3} \cdot \frac{7}{10} = \frac{40 \cdot 7}{3 \cdot 10} = \frac{280}{30} = \frac{28}{3} $$


### Fallgrop!

Om man använder miniräknare, se upp med;

$$\frac{40 \cdot 7}{3 \cdot 10} \neq 40 \times 7 \div 3 \times 10 $$

Det blev ju alldeles fel (testa!).

För att vara på den säkra sidan räkna alltid ut det extra steget;

$$\frac{40 \cdot 7}{3 \cdot 10} = \frac{280}{30} = 280 \div 30 $$

Det kanske känns jobbigt men det blir rätt. När du blir säkrare kan du
använda andra sätt. (rimmar :smile:)




