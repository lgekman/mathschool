# Grafer

Grafer är *mycket viktiga* inom matematik och statistik för att
visualisera ett problem.
Det finns många verktyg för att göra grafer, tex kalkylprogram men
även [online](http://fooplot.com/).

Man använder ett koordinatsystem;

<img src="https://upload.wikimedia.org/wikipedia/commons/f/fb/CartesianPlane.svg" width="30%" />

Bilden visar ett [Kartesiskt
koordinatsystem](https://sv.wikipedia.org/wiki/Kartesiskt_koordinatsystem)
som är det vanligaste (men det finns andra). Skärningspunkten mellan
axlarna kallas *origo*. Man kan lägga till en z-axel för att få ett
3-dimensionellt koordinatsystem (som i Minecraft). Oftast anger man $y$
som en *funktion* av $x$, den allmäna formen är då
$ y = f(x) $. Funktionerna kan vara mycket komplicerade.

Exemplel; $ y = 1 + x \sin{x^2} $

<img src="plot1.svg" width="40%" />

## Manuell graf

Om vi vill göra en graf för area av en kvadrat med sidan $x$ får vi
$y = x^2 $. Vi börjar med en värdetabell

|  $x$  |  $x^2$ |
| ----- | ------ |
|  0    |  0     |
|  0.5  |  0.25  |
|  1    |  1     |
|  1.5  |  2.25  |
|  2    |  4     |
|  3    |  9     |
|  4    |  16    |

Rita sedan ett koordinatsystem och markera koordinaterna. Förbind
sedan punkterna. Observera att det sällan är raka linjer mellan punkterna.

* Gör en graf mha värdetabellen ovan. Använd rutblock och 1 steg = 1cm.

<details><summary>(facit)</summary>

<img src="sqarea.svg" width="20%" />

</details>

<details><summary>(gnuplot)</summary>

gnuplot <<EOF
set terminal svg dynamic
set out 'plot1.svg'
unset y2tics
set key off
set tics axis
set zeroaxis linewidth 1 linetype 1 lc 0
set xtics nomirror
set ytics nomirror
set tics scale 1 1
set border 0
set xrange [-1:3]
unset x2tics
unset x2tics
plot 1 + x * sin(x*x)
EOF

gnuplot <<EOF
set terminal svg size 200,400 dynamic
set out 'sqarea.svg'
unset y2tics
set key off
set tics axis
set zeroaxis linewidth 1 linetype 1 lc 0
set xtics nomirror
set ytics nomirror
set xtics scale 1 1
set ytics scale 2 2 offset -2
set size ratio -1
set border 0
set xrange [0:4]
unset x2tics
plot x*x
EOF

</details>

