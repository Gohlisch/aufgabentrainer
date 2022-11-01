<script>
    import Formula from "../../../lib/shared_components/Formula.svelte";
</script>

<h1>Größen und Einheiten</h1>
<h2>Definitionen</h2>
<p><em>Physik</em> ist die Wissenschaft von der unbelebten Materie.</p>
<p><em>Physikalische Gesetze</em> beschreiben den Zusammenhang zwischen physikalischen Größen.</p>
<p>Eine <em>physikalische Größe</em> ist eine quantifizierbare Eigenschaft eines physikalischen Objektes,
die entweder direkt messbar sind oder aus solchen berechnet werden können.</p>

Notwendig für die Defintion einer physikalischen Messgröße ist:
<ul>
    <li>Eine präzise Messvorschrift</li>
    <li>Unabhängigkeit der Messung von:
        <ul>
            <li>der messenden Person</li>
            <li>dem Ort der Messung</li>
            <li>der Zeit der Messung</li>
        </ul>
    </li>
</ul>

<h2>Kennzeichnung von physikalischen Größen</h2>
Unterscheidungsmerkmal zwischen gleichartigen physikalischen Größen ist ihr <em>Größenwert</em>, der als Produkt aus
<em>Zahlenwert</em> und <em>Einheit</em> angegeben wird.
<table>
    <caption>SI-Vorsätze</caption>
    <thead>
        <tr>
            <th>
                Potenz
            </th>
            <th>
                Name
            </th>
            <th>
                Zeichen
            </th>
        </tr>
    </thead>
    <tbody>
    <tr>
        <td>
            <Formula formula="10^24"></Formula>
        </td>
        <td>
            Yotta
        </td>
        <td>
            Y
        </td>
    </tr>
    <tr>
        <td>
            <Formula formula="10^21"></Formula>
        </td>
        <td>
            Zetta
        </td>
        <td>
            Z
        </td>
    </tr>
    <tr>
        <td>
            <Formula formula="10^18"></Formula>
        </td>
        <td>
            Exa
        </td>
        <td>
            E
        </td>
    </tr>

    <tr>
        <td>
            <Formula formula="10^15"></Formula>
        </td>
        <td>
            Peta
        </td>
        <td>
            P
        </td>
    </tr>

    <tr>
        <td>
            <Formula formula="10^12"></Formula>
        </td>
        <td>
            Tera
        </td>
        <td>
            T
        </td>
    </tr>

    <tr>
        <td>
            <Formula formula="10^9"></Formula>
        </td>
        <td>
            Giga
        </td>
        <td>
            G
        </td>
    </tr>
    <tr>
        <td>
            <Formula formula="10^6"></Formula>
        </td>
        <td>
            Mega
        </td>
        <td>
            M
        </td>
    </tr>
    <tr>
        <td>
            <Formula formula="10^3"></Formula>
        </td>
        <td>
            Kilo
        </td>
        <td>
            k
        </td>
    </tr>
    <tr>
        <td>
            <Formula formula="10^2"></Formula>
        </td>
        <td>
            Hekto
        </td>
        <td>
            h
        </td>
    </tr>
    <tr>
        <td>
            <Formula formula="10^1"></Formula>
        </td>
        <td>
            Deka
        </td>
        <td>
            da
        </td>
    </tr>
    <tr>
        <td>
            <Formula formula="10^3"></Formula>
        </td>
        <td>
            Kilo
        </td>
        <td>
            k
        </td>
    </tr>
    <tr>
        <td>
            <Formula formula={"10^{-1}"}></Formula>
        </td>
        <td>
            Dezi
        </td>
        <td>
            d
        </td>
    </tr>
    <tr>
        <td>
            <Formula formula={"10^{-2}"}></Formula>
        </td>
        <td>
            Zenti
        </td>
        <td>
            c
        </td>
    </tr>
    <tr>
        <td>
            <Formula formula={"10^{-3}"}></Formula>
        </td>
        <td>
            Milli
        </td>
        <td>
            m
        </td>
    </tr>
    <tr>
        <td>
            <Formula formula={"10^{-6}"}></Formula>
        </td>
        <td>
            Mikro
        </td>
        <td>
            μ (kleines "Mu")
        </td>
    </tr>
    <tr>
        <td>
            <Formula formula={"10^{-9}"}></Formula>
        </td>
        <td>
            Nano
        </td>
        <td>
            n
        </td>
    </tr>
    <tr>
        <td>
            <Formula formula={"10^{-12}"}></Formula>
        </td>
        <td>
            Piko
        </td>
        <td>
            p
        </td>
    </tr>
    <tr>
        <td>
            <Formula formula={"10^{-15}"}></Formula>
        </td>
        <td>
            Femto
        </td>
        <td>
            f
        </td>
    </tr>
    <tr>
        <td>
            <Formula formula={"10^{-18}"}></Formula>
        </td>
        <td>
            Atto
        </td>
        <td>
            a
        </td>
    </tr>
    </tbody>
    <tr>
        <td>
            <Formula formula={"10^{-21}"}></Formula>
        </td>
        <td>
            Zepto
        </td>
        <td>
            z
        </td>
    </tr>
    <tr>
        <td>
            <Formula formula={"10^{-24}"}></Formula>
        </td>
        <td>
            Yokto
        </td>
        <td>
            y
        </td>
    </tr>
</table>

<h2>SI-Basiseinheiten</h2>

Einheiten werden angegeben im SI-System (<span lang="fr">Système International d'Unités</span>). Die SI-Basiseinheiten
werden auf Naturkonstanten zurückgeführt.

<div>
    Die sieben SI-Basiseinheiten:
    <ul>
        <li>das Meter (m) als Einheit der Länge</li>
        <li>das Kilogramm (kg) als Einheit der Masse</li>
        <li>die Sekunde (s) als Einheit der Zeit</li>
        <li>das Ampere (A) als Einheit der elektrischen Stromstärke</li>
        <li>das Kelvin (K) als Einheit der thermodynamischen Temperatur</li>
        <li>das Mol (mol) als Einheit der Stoffmenge</li>
        <li>die Candela (cd) als Einheit der Lichtstärke</li>
    </ul>
</div>

