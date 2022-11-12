<script>
import Footnote from "../../../lib/shared_components/Footnote.svelte";
import Formula from "../../../lib/shared_components/Formula.svelte";
import OverflowScrollBox from "../../../lib/shared_components/OverflowScrollBox.svelte";
</script>

<h1>Lineare Differentialgleichungen 1. Ordnung</h1>

<blockquote>
    Eine <em>Differentialgleichung</em> (auch Differenzialgleichung, oft durch DGL, DG, DGl. oder Dgl. abgekürzt)
    ist eine mathematische Gleichung für eine gesuchte Funktion von einer oder mehreren Variablen, in der auch Ableitungen
    dieser Funktion vorkommen. Viele Naturgesetze können mittels Differentialgleichungen formuliert werden.[…] Eine Vielzahl
    von Phänomenen in Natur und Technik kann durch Differentialgleichungen und darauf aufbauende mathematische Modelle
    beschrieben werden.<Footnote link="https://de.wikipedia.org/wiki/Differentialgleichung#Auftreten_und_Anwendungen"/>
</blockquote>

D.h. jede Gleichung, in der auch ihre Ableitung vorkommt, ist eine Differentialgleichung. Die <em>Ordnung</em> einer
Differentialgleichung richtet sich nach der größten vorkommenden Ableitung. In einer Differentialgleichung der 1. Ordnung
sind also nur einfache Ableitung der 1. Ordnung zu finden.

Lineare Differentialgleichungen 1. Ordnung lassen sich immer in folgende
Form umstellen:
<OverflowScrollBox>
    <Formula formula={"y'={\\color{Red} f(x)}\\cdot y + {\\color{Blue} g(x)} \\vert{ {\\color{Blue}g(x)} =: \\text{Störterm}} "}/>
</OverflowScrollBox>

Konkrete Beispiele sind die folgenden:

<OverflowScrollBox>
    <Formula formula={"y'={\\color{Red} -\\sin(x)}\\cdot y + {\\color{Blue} x^3 e^{\\cos(x)}}"}/>
</OverflowScrollBox>

<OverflowScrollBox>
    <Formula formula={"y'={\\color{Red} 5}\\cdot y + {\\color{Blue} x^2}"}/>
</OverflowScrollBox>
<OverflowScrollBox>
    <Formula formula={"y'=\\frac{{\\color{Red} 5}y}{\\color{red}x} - {\\color{Blue} x \\cos(x)}"}/>
</OverflowScrollBox>
<OverflowScrollBox>
    <Formula formula={"y'={\\color{Blue} x e^{-x^2}} - {\\color{red}x}y"}/>
</OverflowScrollBox>
<OverflowScrollBox>
    <Formula formula={"y'={\\color{Blue}3} - {\\color{red}2}y"}/>
</OverflowScrollBox>

Wenn der Störterm nicht vorhanden ist, bzw. <math>0</math> ist, spricht man von einer
<em>homogenen Differentialgleichung</em>.

<!-- TODO: DGL 1 Ordnung weiter bearbeiten... -->
