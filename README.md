# mathschool - Roliga och lärorika mattetal

Mer än ren matteträning försöker exemplen fånga intresset genom att
visa intressanta tillämpningar. Därför, *klicka på länkarna*, tex
hur [Eratosthenes](https://sv.wikipedia.org/wiki/Eratosthenes) mätte
jordens omkrets på 200-talet f.kr!

Områden;

* [Geometri](geometry/README.md)

* [Rationella tal](rational/README.md)

* [Grafer](graphs/README.md)



## Mathematical expressions and graphics

It is possible to use [LaTeX style
syntax](https://en.wikibooks.org/wiki/LaTeX/Mathematics) to render math
expressions for
[formatting](https://github.blog/changelog/2022-05-19-render-mathematical-expressions-in-markdown/)
on github.

Images are drawn with [Inkscape](https://inkscape.org/) and are
published under the [CC0 1.0](
https://creativecommons.org/publicdomain/zero/1.0/) license. Some images
are imported from free [SVG](
https://en.wikipedia.org/wiki/Scalable_Vector_Graphics) sites,
such as;

* https://commons.wikimedia.org/wiki/Category:SVG_files
* https://freesvg.org/

In such cases the link to th original image is [shown in the picture](
geometry/triangulering.md).

Graphs are usually created using [gnuplot](http://www.gnuplot.info/)
and the command to create the plot is included, for example;

<details><summary>(gnuplot)</summary>

```
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
```

</details>
