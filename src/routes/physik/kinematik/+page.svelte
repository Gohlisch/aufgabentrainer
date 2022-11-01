<script>
    import Formula from "../../../lib/shared_components/Formula.svelte";
    import OverflowScrollBox from "../../../lib/shared_components/OverflowScrollBox.svelte";
</script>

<h1>Kinematik</h1>
<h2>Die Geschwindigkeit</h2>
Die <em>Durchschnittsgeschwindigkeit</em> <Formula formula={"\\overline{v}"}/>gibt an, welche Wegstrecke ein Punkt eines Körpers
innerhalb einer bestimmten <em>Zeitspanne</em> zurücklegt. Die Einheit ist <Formula formula={"\\frac{m}{s}"}/>

<OverflowScrollBox>
    <Formula formula={"\\text{Durchschnittsgeschwindigkeit} := \\frac{\\text{Wegstrecke}}{\\text{Zeitspanne}}"}/>
    <Formula formula={"\\Leftrightarrow \\overline{v}=\\frac{\\Delta s}{\\Delta t}"}/>
</OverflowScrollBox>


<details>
    <summary>Durchschnittwerte</summary>
    Durchschnittswerte werden in Physik oft mit einer Querstrich über der Variable dargestellt, wie hier <Formula formula={"\\overline{v}"}/>.
</details>

<h3>Spezialfall: Die gleichförmige Bewegung</h3>
Bei der <em>gleichförmigen Bewegungen</em> sind der zurückgelegte Weg eines Massepunktes und die dafür benötige Zeit
zueinander proportional. Der Proportionalitätsfaktor ist ein Maß für die konstante Geschwindigkeit.

<OverflowScrollBox>
    <Formula formula={"\\text{Ort zum Zeitpunkt }t = \\text{Anfangspunkt}+\\text{Geschwindigkeit}\\cdot\\text{benötigte Zeit}"}/>
    <Formula formula={"\\Leftrightarrow s(t) = s_0 + \\overline{v}(t-t_0)"}/>
</OverflowScrollBox>

<OverflowScrollBox>
    <svg viewBox="0 0 250 100" class="chart">
        <style>
            .small {
                font-size: 0.5em;
            }
        </style>

        <polyline
                fill="none"
                stroke="#000000"
                stroke-width="1"
                points="
       0,100
       250,20"/>
        <line x1="0" y1="80" x2="62" y2="80" stroke="red" stroke-width="0.5" />
        <line x1="60" y1="120" x2="62" y2="80" stroke="red" stroke-width="0.5"/>
        <line x1="62" y1="80" x2="150" y2="80" stroke="blue" stroke-width="0.5" />
        <line x1="150" y1="80" x2="150" y2="52" stroke="blue" stroke-width="0.5"/>
        <text x="20" y="78" class="small" >s₀</text>
        <text x="65" y="100" class="small" >t₀</text>
        <text x="200" y="43" class="small" >s(t)</text>
        <text x="152" y="70" class="small" >Δs</text>
        <text x="100" y="90" class="small" >Δt</text>
    </svg>
</OverflowScrollBox>

<h3>Momentangeschwindigkeit</h3>

Die <em>Momentangeschwindigkeit</em> <Formula formula="v"></Formula> ist die Durchschnittgeschwindigkeit über einen unendlich
kleines Zeitintervall. Einheit <Formula formula={"\\frac{m}{s}"}/>.

Die Geschwindigkeit v ist die Ableitung von s nach t:
<OverflowScrollBox>
    <Formula formula={"v(t)=\\dot{s}(t)=\\lim_{t \\to 0}\\frac{\\Delta s}{\\Delta t}"}/>
</OverflowScrollBox>

<h3>Die Beschleunigung</h3>

Die <em>Durchschnittsbeschleunigung</em> <Formula formula={"\\overline{a}"}/> ist der Quotient aus der
Geschwindigkeitsänderung und der zugehörigen Zeitspanne. Einheit <Formula formula="m/s^2"/>.
<OverflowScrollBox>
    <Formula formula={"\\overline{a}(t)=\\frac{\\Delta v}{\\Delta t}"}/>
</OverflowScrollBox>

Die Momentanbeschleunigung ist der Grenzwert der Durschnittsbeschleunigung:
<OverflowScrollBox>
    <Formula formula={"a(t)=\\dot{s}(t)=\\lim_{t \\to 0}\\frac{t+\\Delta t-v(t)}{\\Delta t}=\\dot{v}(t)=\\ddot{s}(t)"}/>
</OverflowScrollBox>

